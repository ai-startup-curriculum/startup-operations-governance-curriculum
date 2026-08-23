# 4. Sanctions and export-controls compliance

> A US-based SaaS company with a self-serve signup form is transacting across borders by default. The rule of thumb: if your product is Internet-reachable, you have OFAC and EAR exposure — and one paying customer inside a sanctioned jurisdiction is an enforcement problem.

## Motivation

Sanctions and export-controls compliance is one of the areas where a startup's intuition is most likely to be wrong. Founders assume the regime applies only to defence contractors and global banks. In fact, the OFAC country programmes reach any US person, US entity, or foreign entity with a US-territory nexus — including the transfer of software over the Internet — and the Export Administration Regulations (EAR) reach any US-origin item, technology, or software regardless of who ships it. The moment your product is downloadable, self-serve, or API-callable from anywhere on the public Internet, you are exporting; the only question is whether you know it.

Enforcement is asymmetric. OFAC penalties are strict-liability civil penalties per violation, and criminal referrals are available for wilful violations. BIS penalties under the Export Control Reform Act of 2018 are similarly severe. Both regimes include Denied Persons designations that can end the company's ability to export at all. This chapter builds the programme that keeps the company inside the lines.

Ownership boundary before we begin: this chapter owns the **sanctions and export-controls compliance programme**. Product-side geo-blocking, IP-geolocation, and payment-processor screening are implementation controls; the policy and diligence sit here. See [chapter 05](./05-fcpa-and-anti-corruption-programme.md) for the adjacent anti-corruption regime — different substance, adjacent compliance operating model.

## The regulatory landscape

Three regulators own the primary US export and sanctions regimes:

### OFAC — Office of Foreign Assets Control (Treasury)

OFAC administers economic and trade sanctions programmes based on foreign-policy and national-security goals. Primary regulations: **31 CFR Chapter V (Parts 500–599)**.

Two structural pieces:

- **Country / regional programmes.** Comprehensive sanctions on specific jurisdictions — Iran (31 CFR Part 560), Cuba (31 CFR Part 515), North Korea (31 CFR Part 510), Syria (31 CFR Part 542), the Crimea / DNR / LNR / Kherson / Zaporizhzhia regions of Ukraine (Executive Order 14065 and related regulations), and others. The Russia programme is a hybrid of country-based and list-based elements built on Executive Orders 14024, 14066, 14068, 14071, and successors. Comprehensive-sanctions programmes generally prohibit essentially all direct and indirect transactions absent an authorising general or specific licence.
- **List-based programmes.** Prohibitions on transactions with named persons and entities regardless of jurisdiction:
  - **SDN List** — Specially Designated Nationals and Blocked Persons List. Assets blocked; effectively all dealings prohibited.
  - **Consolidated Sanctions List** — a compilation of persons on OFAC lists that are **not** on the SDN List (Non-SDN Palestinian Legislative Council List, Foreign Sanctions Evaders, Sectoral Sanctions Identifications, Non-SDN Menu-Based Sanctions, etc.).
  - **Sectoral Sanctions Identifications (SSI) List** — sectoral restrictions on certain Russian energy, financial-services, and defence entities.
  - **Non-SDN Menu-Based Sanctions (NS-MBS) List** — CAATSA and related programme designations.
  - **Correspondent Account or Payable-Through Account Sanctions (CAPTA)** List.

Screening data sources are published at OFAC's sanctions-list-service portal, refreshed regularly, and available as consolidated feeds for programmatic ingestion.

### BIS — Bureau of Industry and Security (Commerce)

BIS administers the **Export Administration Regulations (EAR)**, 15 CFR Parts 730–774. The EAR govern the export, re-export, and in-country transfer of items that are "subject to the EAR" — a broad category that includes items in the United States, all US-origin items regardless of location, and certain foreign-produced items with US content or produced with US technology.

Three artefacts drive EAR compliance:

- **Commerce Control List (CCL)** — 15 CFR Part 774, Supplement 1. Items are classified by Export Control Classification Number (ECCN). Items not otherwise classified are EAR99 (subject to the EAR but not on the CCL).
- **Country Chart** — 15 CFR Part 738, Supplement 1. Cross-references ECCN entries to reasons for control (National Security, Anti-Terrorism, etc.) and destinations, yielding the licence-requirement matrix.
- **License Exceptions** — 15 CFR Part 740. Where a licence would otherwise be required, specific licence exceptions may authorise the export without individual licence application.

Recent BIS focus for AI-adjacent startups:

- **Advanced computing and semiconductor controls.** October 7, 2022, controls introduced ECCN entries covering advanced-node semiconductors and certain AI-accelerator devices, with expanded end-user and end-use restrictions targeting China. The October 17, 2023, "Interim Final Rule" and subsequent amendments refined those controls, added additional entities to the Entity List, and introduced Notified Advanced Computing thresholds. <!-- needs-research: verify the current version of 15 CFR § 744.23 and the advanced-computing / semiconductor controls after the January 2025 IFR and any 2025–2026 amendments. -->
- **Encryption controls.** 15 CFR § 740.17 (License Exception ENC) and 15 CFR § 742.15 govern the export of items with more-than-mass-market encryption. Most SaaS with standard TLS is either self-classified as mass-market or benefits from the ENC exception; **classification and — for certain items — an annual self-classification report to BIS** are typically required.
- **AI model controls.** As of the current regulatory environment, some AI models and model weights (particularly frontier-model weights above compute or capability thresholds) may fall within BIS controls or be the subject of forthcoming rulemaking. <!-- needs-research: verify whether any final rule under the Bureau of Industry and Security controlling AI model weights was published; cite EO 14110 and any successor executive orders and BIS notices. -->

BIS also maintains several list-based restrictions independent of the CCL:

- **Entity List** (15 CFR Part 744, Supplement 4) — licence requirements for exports to listed entities, often with a presumption of denial.
- **Denied Persons List** — persons prohibited from participating in any transaction subject to the EAR.
- **Unverified List** (15 CFR Part 744, Supplement 6) — parties BIS could not verify in a prior end-use check; heightened due-diligence and a suspension of certain licence exceptions.
- **Military End-User (MEU) List** and **Military-Intelligence End-User (MIEU) List** — additional licence requirements for listed entities in specific destinations.

### DDTC — Directorate of Defense Trade Controls (State)

DDTC administers the **International Traffic in Arms Regulations (ITAR)**, 22 CFR Parts 120–130. ITAR governs the export of **defense articles**, **defense services**, and **related technical data** enumerated on the **U.S. Munitions List (USML)** (22 CFR § 121.1).

Two things every startup should know:

- **Registration first, transaction second.** Under **22 CFR § 122.1**, any US person who manufactures, exports, or brokers defense articles or defense services must register with DDTC, **regardless of whether any export or brokering activity actually occurs**. Registration alone is triggered by manufacture of a USML item.
- **Deemed exports.** ITAR-controlled technical data cannot be shared with a foreign person — including a foreign-national employee inside the United States — without a licence or exemption. Hiring a foreign-national engineer to work on ITAR-controlled technology on a US-work visa alone is **not authorised**; the visa admits the person but does not authorise the technical-data disclosure. See **22 CFR § 120.17** (definition of export includes releasing technical data to a foreign person).

Corresponding "deemed export" concepts exist under the EAR (15 CFR § 734.13), covering release of controlled technology to foreign persons in the United States.

## The startup EAR / ITAR triage

A serviceable triage the first time you build the programme:

- **Does the product include encryption above mass-market strength?** If yes → EAR encryption controls apply (15 CFR § 740.17 and § 742.15). Classification exercise required; possibly annual self-classification report. Most startups land here.
- **Does the product include AI models or model access above the controlled threshold?** If yes → EAR advanced-computing / AI controls apply. Classification exercise required; end-user and destination restrictions likely. <!-- needs-research: confirm current threshold and end-user restrictions. -->
- **Does the product interact with defense customers, defense applications, or USML items?** If yes → ITAR analysis required. Registration under 22 CFR § 122.1 may be triggered even before export.
- **None of the above?** EAR still applies at the EAR99 baseline: EAR99 items cannot be exported to comprehensively-embargoed destinations without a licence, and cannot be exported to Entity-List or Denied-Persons parties.

Every startup with a public product is at minimum in the fourth bucket. Most software startups are in the first bucket (encryption). AI-heavy startups are increasingly in the second. Hardware and dual-use startups may be in the third.

## OFAC screening programme design

Screening is the mechanical heart of the sanctions programme. Design for four populations:

- **Customers.** Screen at signup and on renewal / re-onboard. For self-serve products, integrate screening into the signup flow (name, email domain, address, jurisdiction). For enterprise-sales products, screen during the sales-cycle onboarding gate.
- **Vendors.** Screen at onboarding and on a recurring basis (annually at minimum; on any material contract change).
- **Employees and contractors.** Screen at hire; re-screen on role change; integrate with [mod-104](../mod-104-hiring-onboarding-and-hr-operations/) onboarding workflow.
- **Cross-border payments.** Screen counterparty at initiation. Payment processors (Stripe, Adyen, banks) generally screen automatically, but the ultimate obligation stays with the payer. Confirm the processor's screening scope and retain evidence.

**Data sources to screen against, at minimum:**

- SDN List.
- Consolidated Sanctions List.
- SSI List.
- BIS Entity List, Denied Persons List, Unverified List, MEU List, MIEU List (yes, EAR / BIS lists are typically included in the same screening pass as OFAC lists).
- UK OFSI Consolidated List and EU Consolidated Financial Sanctions List (for any material UK / EU nexus).
- Country / regional-programme jurisdictions (Iran, Cuba, North Korea, Syria, Crimea/DNR/LNR/Kherson/Zaporizhzhia).

Screening data attributes:

- Individual: full name, aliases, dates of birth, jurisdiction of residence, identification numbers where available.
- Entity: full name, aliases, jurisdiction, DUNS or equivalent, beneficial-ownership information where accessible.

**False-positive triage.** Screening produces false positives (John Smith matches an SDN John Smith). A documented triage workflow — reviewer, evidence standard, disposition, retention — is a required control. Common triage evidence: date of birth, identification document, jurisdictional confirmation. Where triage cannot resolve to a clear negative, escalate to the compliance officer and outside counsel.

**Vendor tools.** Commercial screening providers (Refinitiv World-Check, Dow Jones RiskCenter, LexisNexis Bridger, Sanctions.io, ComplyAdvantage, Napier, others) provide list feeds, screening APIs, and false-positive-adjudication interfaces. Small companies can build a screening pipeline against OFAC's own consolidated feed; commercial tools accelerate at scale.

## BIS EAR compliance programme design

The EAR programme runs six operational steps:

1. **Classify the product.** Self-classification against the CCL, or a formal Commodity Classification (CCATS) request to BIS under **15 CFR § 748.3(e)**. Retain the classification analysis in a controlled file.
2. **Determine the licence requirement.** Apply the ECCN and the Country Chart. Determine any applicable licence exceptions (Part 740).
3. **Screen the end-user.** Against the Entity List, Denied Persons List, Unverified List, MEU List, MIEU List.
4. **Screen for red flags of a prohibited end-use.** BIS **"Know Your Customer" Guidance and Red Flag Indicators** (15 CFR Part 732, Supplement 3) identifies patterns that require heightened inquiry — vague end-use, reluctance to answer end-user questions, mismatch between the customer's business and the product being ordered, requests for non-standard shipping instructions.
5. **Apply for licences where required.** Via the **SNAP-R** electronic filing system (https://snapr.bis.doc.gov/). Retain the licence file with export records.
6. **Retain records.** Retention obligations under **15 CFR Part 762** — five years from the date of the export, re-export, or in-country transfer (or from the date of expiration of a licence, whichever is later).

For encryption-item exports, additional obligations under **15 CFR § 740.17** — annual self-classification report to BIS for certain encryption items; semi-annual reporting for certain other categories. <!-- needs-research: confirm the current § 740.17 reporting cadence and covered categories. -->

## ITAR compliance — brief

ITAR is a specialist domain; treat this section as triage, not depth.

- **Registration under 22 CFR § 122.1** is triggered by USML-item manufacture, export, or brokering. Register before any regulated activity.
- **Licensing** for defense-article exports via DDTC's **DECCS** portal (https://www.pmddtc.state.gov/deccs).
- **Deemed exports** — no ITAR-controlled technical data to a foreign-person employee without licence or exemption. This includes contractors, interns, and visiting researchers.
- **Broker registration and licensing** under 22 CFR Part 129 for parties that solicit, promote, negotiate, or otherwise facilitate defence-article transactions.

An ITAR programme, when triggered, requires dedicated ITAR compliance counsel. It is not a self-serve regime.

## The escalation pattern on a hit

A **true positive** on any list — SDN, Entity List, Denied Persons List, or a suspected in-country user in a comprehensively-embargoed jurisdiction — is a hard-stop escalation.

Standard escalation:

1. **Freeze the transaction / access.** Do not proceed further. Do not send a polite decline message; do not refund; do not confirm receipt to the counterparty until legal has reviewed. A refund of a payment that was itself a blocked property can constitute a further violation.
2. **Escalate to the Sanctions Compliance Officer** (typically the GC or CCO).
3. **Engage outside sanctions counsel.** They will assess whether blocking, rejection, licence application, or self-disclosure is required.
4. **Assess self-disclosure obligations.** OFAC's Economic Sanctions Enforcement Guidelines (31 CFR Part 501, Appendix A) treat voluntary self-disclosure as a mitigating factor. BIS treats voluntary self-disclosure under 15 CFR § 764.5 similarly.
5. **Report as required.** SDN-blocked property is reported to OFAC within 10 business days under 31 CFR § 501.603. Rejected transactions may also require reporting. Any BIS-required disclosure runs on its own timeline.

The escalation matrix belongs in a written policy, not in the head of the GC.

## The OFAC Framework — the programme baseline

Treasury OFAC's **"A Framework for OFAC Compliance Commitments"** (May 2019) is the operating baseline. It identifies **five essential components** of an effective sanctions compliance programme:

1. **Management commitment.** Senior-management ownership; adequate resources; independence of the compliance function; clear reporting lines.
2. **Risk assessment.** A documented risk assessment of the company's sanctions exposure — customer base, geographic footprint, product delivery model, third-party partners — updated at least annually and on material change.
3. **Internal controls.** Written policies and procedures; controls tailored to identified risks; screening; escalation; recordkeeping; testing.
4. **Testing and auditing.** Periodic testing of the programme's effectiveness — including sample screening reviews, mock enforcement scenarios, and independent audit.
5. **Training.** Role-appropriate training for all relevant personnel, at hire and periodically thereafter; enhanced training for sales, finance, legal, and any personnel interacting with cross-border customers or vendors.

<!-- needs-research: cite the exact URL for the May 2019 OFAC Framework document on ofac.treasury.gov. -->

Enforcement actions repeatedly cite the Framework's five components as the yardstick. A written programme that maps to those five components — and that a compliance officer can walk an examiner through — is the target state.

## Programme documentation

Standard deliverables that make the programme legible and defensible:

- **Written Sanctions Compliance Policy** — organisation-wide, signed by the CEO, refreshed annually.
- **Written Export Controls Policy** — covering EAR classification, screening, licensing, deemed exports, and recordkeeping.
- **Sanctions Compliance Officer** appointed in writing (typically the GC or CCO), with a stated reporting line and independence protections.
- **Approved vendor and channel-partner list** — vetted, dated, and refreshed.
- **Escalation matrix** — the "who does what when" for a hit.
- **Annual training curriculum** — role-appropriate, tracked completion.
- **Documented annual risk assessment** — the OFAC-Framework second component.
- **Recordkeeping** — screening records, licence files, export documentation, retained for **five years** under EAR § 762.6 and **at least five years** under OFAC recordkeeping requirements (31 CFR §§ 501.601–501.602). <!-- needs-research: verify current OFAC recordkeeping period and BIS retention period, and confirm any longer requirements for specific programmes. -->

## Ownership boundary

- **The sanctions and export-controls compliance programme, the OFAC / EAR / ITAR triage, the screening workflow, the licensing workflow, and the escalation pattern**: this chapter.
- **Anti-corruption compliance (FCPA / UK Bribery Act)**: [chapter 05](./05-fcpa-and-anti-corruption-programme.md). Different regime; adjacent operating model.
- **Ransomware-payment OFAC gate**: coordinated with [chapter 03](./03-cyber-insurance-and-incident-response-coordination.md).
- **Commercial contract terms — export-controls and sanctions representations, audit rights, deny-export clauses**: [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/).
- **International-expansion sanctions and export-controls posture, including local-country regulators (UK OFSI, EU Council, French Ministère de l'Économie et des Finances) and forced-technology-transfer regimes**: [mod-113](../mod-113-international-expansion-and-global-workforce/).
- **Hiring / onboarding integration — sanctions screening at hire, foreign-person status collection**: [mod-104](../mod-104-hiring-onboarding-and-hr-operations/).

## Summary

- **A US company with a public Internet product has sanctions and export exposure by default.** The only question is whether the programme surfaces it.
- **Three regulators** — OFAC (Treasury) for sanctions, BIS (Commerce) for the EAR, DDTC (State) for ITAR. Learn the seams.
- **Triage first.** Encryption above mass-market → EAR encryption controls. AI models above controlled threshold → EAR advanced-computing controls. Defense customers or USML items → ITAR (and registration under 22 CFR § 122.1 alone is triggered by manufacture).
- **Screen four populations** — customers, vendors, employees/contractors, cross-border payments — against SDN, Consolidated, SSI, Entity List, DPL, Unverified, MEU, MIEU, and jurisdiction lists.
- **Any true-positive hit is a hard stop.** Freeze; escalate to the Sanctions Compliance Officer and outside counsel; assess licence, block, reject, and self-disclosure.
- **The OFAC "Framework for OFAC Compliance Commitments" (2019)** — five components: management commitment, risk assessment, internal controls, testing and auditing, training. Build the programme to map cleanly to those five.
- **Recordkeeping is five years across all three regimes.** Screening records, licence files, export documentation — retained and retrievable.
- **When the triage or the escalation reaches a real question, outside sanctions counsel is not optional.** This is not a self-serve regime.
