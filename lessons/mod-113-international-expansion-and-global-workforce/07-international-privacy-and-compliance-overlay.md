# 7. International privacy and compliance overlay

> The US-parent / international-sub configuration is a cross-border personal-data transfer every day it operates. The GDPR / FCPA / sanctions / export-control overlay is not an add-on — it is the operating licence for the international footprint.

## Motivation

The international footprint built in [chapters 02](./02-first-international-entity-setup.md) and [03](./03-intercompany-and-transfer-pricing-structure.md) does three things, every day, from day one. First, employees in subsidiaries process personal data about customers, prospects, and each other — and that data flows back to the US parent through HRIS, CRM, ticketing, observability, and payroll aggregation. Second, the US parent sends payments, equity grants, management-fee allocations, and intercompany invoices across borders — any one of which can touch a sanctioned party, a politically exposed person, or a foreign government counterparty. Third, the technology the US parent ships into those subsidiaries — ML models, code, SaaS services, hardware — is export-controlled by the US (and sometimes by the destination country) regardless of whether the US parent sees it that way.

A US-only privacy / compliance posture, lifted and dropped into an international footprint, breaks on contact. GDPR applies to the UK employee's HR file in the US HRIS whether or not the US HRIS vendor has heard of it. The UK Bribery Act 2010 reaches a US company's UK operations even when the US FCPA ([mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md)) is the primary training reference. Export-control licensing exposure travels with the model weights the US parent syncs to a London or Bangalore engineering office.

This chapter does not re-author the privacy programme — that is [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) — or the sanctions-and-export-controls programme — that is [mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md). It owns the **international-amplification overlay**: the places where the existence of a subsidiary, an EOR relationship, or a cross-border transfer changes the obligation set in ways the US-only programme does not cover.

**Ownership boundary before we begin.** This chapter owns the overlay — the "what changes when you go international" layer on top of the privacy, anti-bribery, sanctions, and export-control programmes. The underlying regimes (GDPR substantive law, FCPA substantive law, OFAC sanctions programme, EAR / ITAR export-control regime) live in [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) and [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/). Confirm the reader has those references before applying this chapter.

## Cross-border personal-data transfers under GDPR

The GDPR (Regulation (EU) 2016/679) applies to any personal data processing of EU-resident data subjects, regardless of where the controller or processor sits. The international footprint typically creates three transfer flows, each requiring a lawful basis under GDPR Chapter V (Articles 44–50):

### Flow 1 — EU subsidiary → US parent (employee personal data)

The EU subsidiary is the controller for its employees' HR data; the US parent typically has routine access via the HRIS, equity-plan administrator, and group-management systems. Each access is a transfer of personal data from a controller inside the EU to a controller (joint or independent) outside the EU — a Chapter V event.

Lawful bases, in order of operator preference:

1. **Adequacy decision** under Article 45. The European Commission has adopted adequacy decisions for a limited set of countries (Andorra, Argentina, Canada — commercial organisations subject to PIPEDA, Faroe Islands, Guernsey, Israel, Isle of Man, Japan, Jersey, New Zealand, Republic of Korea, Switzerland, United Kingdom, Uruguay, and the United States — the last under the **EU–US Data Privacy Framework (DPF)**, Commission Implementing Decision (EU) 2023/1795, adopted 10 July 2023). For transfers *to the US*, the DPF is the operator's primary lever: self-certify the US parent under the DPF (via the Department of Commerce DPF Program at [dataprivacyframework.gov](https://www.dataprivacyframework.gov/)), publish the required privacy policy, enrol in the Independent Recourse Mechanism, and the Chapter V transfer basis is in place. The DPF has outstanding litigation and policy risk (see *Schrems I* and *Schrems II*, and the pending *Schrems III* trajectory) — build the structure assuming the DPF survives but with a fallback.
2. **Standard Contractual Clauses (SCCs)** under Article 46(2)(c). The 2021 modular SCCs under **Commission Implementing Decision (EU) 2021/914** (effective 27 September 2021) — Modules 1 (C2C), 2 (C2P), 3 (P2P), 4 (P2C). The US parent and the EU subsidiary execute SCCs for intra-group transfers (typically Module 1 for parent-sub controller-to-controller flows, Module 2 or 3 for processor flows). **Transfer Impact Assessment (TIA)** per Clause 14 is a required step — a documented analysis of the destination jurisdiction's surveillance law (US FISA § 702, EO 12333, and the DPF's redress mechanism under PPD-28 / EO 14086), the supplementary measures (encryption at rest and in transit, pseudonymisation, access controls), and the conclusion that the transfer meets essentially-equivalent protection.
3. **Binding Corporate Rules (BCRs)** under Article 47. A set of intra-group transfer rules approved by a lead EU data protection authority after a formal application. BCRs are the gold standard for large multinationals — stable, lead-DPA-approved, pre-tested — but the approval process is slow (12–24 months) and most startups do not reach the scale to justify it.
4. **Article 49 derogations.** Explicit consent, performance of a contract, important public interest. These are *derogations*, not routine transfer mechanisms — not a substitute for Chapter V compliance at operational scale.

**Operator default.** For the first US / EU footprint, the standard pattern is DPF self-certification (US parent) + SCCs (Module 1 and Module 2 as applicable) + a documented TIA for each transfer category. Review annually with the DPO ([mod-110](../mod-110-privacy-data-governance-and-sector-compliance/)).

### Flow 2 — EU subsidiary → non-US third-country processor (SaaS vendors)

Routine. The UK Ltd uses a US-hosted CRM (Salesforce), a US-hosted HRIS (Workday / Rippling), an EU-hosted but US-parent-owned observability tool (Datadog), and a US-hosted equity administrator (Carta). Each is a Chapter V transfer; each requires its own transfer mechanism.

Operator responsibilities:

- Confirm each vendor has an **Article 28 DPA** (controller / processor contract — covered in [mod-109 chapter 01](../mod-109-commercial-contracts-ip-and-legal-ops/01-customer-contract-suite-msa-sla-dpa-security-aup.md) from the sell-side perspective and [mod-109 chapter 03](../mod-109-commercial-contracts-ip-and-legal-ops/03-vendor-contract-suite-and-onboarding-workflow.md) from the buy-side).
- Confirm each vendor's **transfer mechanism** — DPF self-certification, SCCs executed, BCRs approved.
- Maintain the **Article 30 Records of Processing Activities (RoPA)** showing each cross-border transfer and the mechanism relied on. The RoPA is the primary artefact a DPA inspection asks for first.
- Document a **Transfer Impact Assessment** per vendor where SCCs are relied on (per Clause 14 of the 2021 SCCs).

### Flow 3 — Intra-group transfers between EU subsidiaries and non-EU subsidiaries

A UK Ltd and an Indian Pvt Ltd routinely exchange personal data (customer-support tickets, engineering access logs, release-management artefacts). Each exchange is a Chapter V transfer. Intra-group SCCs or BCRs cover the pattern.

**UK GDPR nuance.** Post-Brexit, the UK operates its own GDPR regime (the UK GDPR, retained via the Data Protection Act 2018 as amended by the European Union (Withdrawal) Act 2018 and subsequent regulations). The UK has its own adequacy map (UK international data transfers), its own version of SCCs (the **International Data Transfer Agreement (IDTA)** and the **UK Addendum to the EU SCCs**), and its own regulator (the Information Commissioner's Office, ICO). The practical pattern: execute EU SCCs + UK Addendum where a transfer touches both EU and UK data, or execute an IDTA where the transfer is UK-origin only. ICO guidance at [ico.org.uk](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/international-transfers/).

**Swiss transfers.** Switzerland is not an EU member but has adopted a GDPR-aligned Federal Act on Data Protection (**revFADP**, in force 1 September 2023). The Swiss FDPIC has recognised the EU SCCs with a Swiss Addendum for transfers from Switzerland.

## Country-specific privacy overlays beyond GDPR

A representative map of country-specific privacy regimes the international programme intersects:

### United Kingdom

- **UK GDPR + DPA 2018.** As above. The ICO is the regulator.
- **PECR (Privacy and Electronic Communications Regulations 2003).** Cookies, electronic marketing, and traffic data — the UK's e-privacy regime pending the long-promised ePrivacy Regulation.

### European Union (country-specific supplements)

Individual EU member states supplement the GDPR with country-specific implementation. The GDPR directly applies, but national law layers obligations:

- **Germany — BDSG (Bundesdatenschutzgesetz).** Supplements GDPR; stricter rules on **employee data processing** under BDSG § 26 (the employment-specific lawful-basis provision — distinct from GDPR Article 6(1)(b)). Works-council co-determination over data-processing systems ([chapter 05](./05-international-employment-law-variance.md)).
- **France — Loi Informatique et Libertés** (as amended). The CNIL (Commission nationale de l'informatique et des libertés) is one of the most active EU DPAs; sector-specific decisions and dossiers are published regularly.
- **Netherlands — UAVG.** Supplements GDPR; Autoriteit Persoonsgegevens (AP) is the regulator.
- **Ireland — Data Protection Act 2018.** The Irish DPC (Data Protection Commission) is the lead supervisory authority for many US-headquartered multinationals under the One-Stop-Shop mechanism; a disproportionate share of large GDPR enforcement decisions flow through Dublin.

### Switzerland

**revFADP** (in force 1 September 2023). Scope-triggers close to GDPR; cross-border transfers require adequacy, SCCs with Swiss Addendum, BCRs, or specific exceptions.

### Canada

**PIPEDA (Personal Information Protection and Electronic Documents Act)** applies to private-sector organisations in the course of commercial activities. Provincial substantial-equivalent statutes apply in Alberta (PIPA), British Columbia (PIPA), and Quebec (**Law 25**, the modernised private-sector privacy statute post-2022 reform — one of the most GDPR-aligned regimes in North America, including explicit cross-border-transfer obligations and mandatory privacy impact assessments). The Office of the Privacy Commissioner of Canada is the federal regulator. <!-- needs-research: confirm current Law 25 implementation phasing and the current PIPEDA modernisation status (the proposed Consumer Privacy Protection Act under Bill C-27 as of 2025–2026). -->

### Brazil

**LGPD (Lei Geral de Proteção de Dados Pessoais, Law 13,709/2018)**. GDPR-aligned; ANPD (Autoridade Nacional de Proteção de Dados) is the regulator. International transfers require adequacy, SCCs, specific guarantees, or consent.

### China

**PIPL (Personal Information Protection Law)**, effective 1 November 2021; the **CSL (Cybersecurity Law)** of 2017; and the **DSL (Data Security Law)** of 2021. One of the most restrictive regimes globally. Cross-border transfers of personal information from mainland China require one of: (a) security assessment by the Cyberspace Administration of China (CAC) for high-volume or sensitive transfers, (b) **Chinese Standard Contractual Clauses (China SCCs)** filed with the CAC, (c) certification by a CAC-recognised institution, or (d) specific exceptions. The security-assessment thresholds and SCC filing procedures have evolved repeatedly since 2022; verify current rules before structuring any China-touch data flow. <!-- needs-research: confirm current CAC cross-border-transfer rules, security-assessment thresholds, and SCC filing procedure as of 2025–2026 — the regime has evolved repeatedly. -->

### Singapore, Malaysia, Thailand

**PDPA (Personal Data Protection Act)** — Singapore (2012, amended 2020 and 2022), Malaysia (2010, 2024 amendment), Thailand (2019). All GDPR-adjacent but with lower penalty ceilings and local-specific overlays. Transfer-out rules vary — Singapore permits transfers to jurisdictions providing comparable protection or with contractual guarantees; Thailand's PDPA includes GDPR-like data-subject rights and consent mechanics.

### Australia

**Privacy Act 1988** and the **Australian Privacy Principles (APPs)**. APP 8 regulates cross-border transfers — the entity disclosing personal information remains accountable for the recipient's handling unless specific exceptions apply (recipient subject to comparable law, informed consent, legally-required disclosure). Significant 2024 amendment package increased penalties and introduced tiered civil penalty regime; **further Privacy Act reform** is under way with the Privacy and Other Legislation Amendment Bill 2024 and successor instruments. <!-- needs-research: confirm current Australian Privacy Act reform status and whether a statutory tort for serious privacy invasions has been enacted. -->

### Japan

**APPI (Act on the Protection of Personal Information)** — one of the oldest comprehensive privacy regimes in Asia; subject to a GDPR adequacy decision. PPC (Personal Information Protection Commission) is the regulator.

### South Korea

**PIPA (Personal Information Protection Act)** — one of the most prescriptive privacy regimes globally; subject to a GDPR adequacy decision. PIPC (Personal Information Protection Commission) is the regulator.

### India

**Digital Personal Data Protection Act, 2023 (DPDP Act)**. In force in phases from 2024 / 2025 onward; GDPR-adjacent but with its own cross-border-transfer architecture (whitelist-based rather than SCC-based). Compliance architecture and rules continue to be issued. <!-- needs-research: confirm current DPDP Act implementation phasing, notified rules, and operator obligations as of 2025–2026. -->

## The data-residency and sovereignty-cloud overlay

A number of jurisdictions impose data-residency or data-sovereignty requirements that go beyond cross-border-transfer discipline:

- **EU AI Act (Regulation (EU) 2024/1689)** and **GDPR Article 48** — restrictions on transfer in response to foreign-court or foreign-authority requests. The US CLOUD Act (18 U.S.C. §§ 2701–2713 as amended) and its interaction with GDPR is a recurring friction. Pending the US-EU CLOUD Act executive agreement, operators default to the DPF or SCC-based transfer basis.
- **China** — effective data-localisation for Critical Information Infrastructure Operators (CIIOs) under the CSL, plus the CAC's cross-border-transfer regime noted above.
- **Russia** — Federal Law 242-FZ requires that personal data of Russian citizens be initially recorded, stored, and amended in databases physically located in Russia. Operating in Russia under current sanctions is a separate decision ([mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md)); the data-residency rule remains notable for operators considering any Russian footprint.
- **Vietnam, Indonesia** — localisation requirements in specific sectors.
- **Sovereign-cloud offerings.** AWS Dedicated Local Zones / European Sovereign Cloud, Microsoft Cloud for Sovereignty, Google Sovereign Cloud, Oracle EU Sovereign Cloud — intended for operators needing in-region, in-jurisdiction, EU-personnel-operated infrastructure. Relevant for public-sector contracting in regulated European jurisdictions. <!-- needs-research: verify current state and operational availability of the major hyperscalers' sovereign-cloud offerings as of 2025–2026. -->

## FCPA-equivalents — the global anti-bribery overlay

The US **Foreign Corrupt Practices Act (FCPA)** — 15 U.S.C. §§ 78dd-1 et seq. — applies to US issuers, domestic concerns, and any person acting in US territory, regardless of nationality. The international footprint does not reduce FCPA exposure; it typically increases it (more foreign-official touch points, more intermediaries, more cash transfers abroad). The FCPA substance lives in [mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md).

Where the international footprint changes the analysis: **three jurisdictions impose their own anti-bribery statutes that reach differently from the FCPA**, and compliance to the local statute is required in addition to FCPA compliance.

### United Kingdom — Bribery Act 2010

**Bribery Act 2010** — in force 1 July 2011. Four principal offences:

- **Section 1** — bribing another person.
- **Section 2** — being bribed.
- **Section 6** — bribing a foreign public official (parallels but is distinct from the FCPA; no "foreign-official" scienter requirement equivalent to FCPA § 78dd-1(a)).
- **Section 7** — **failure of a commercial organisation to prevent bribery**. A strict-liability corporate offence; the only defence is that the organisation had **adequate procedures** in place to prevent bribery.

Important for the operator:

- **Section 7 reaches further than the FCPA.** Any "commercial organisation" that is incorporated, formed, or **carries on a business or part of a business in the UK** is in scope. A US-parent group with a UK Ltd subsidiary is a commercial organisation under the Bribery Act; a US-parent group making sales into the UK without a subsidiary may also be in scope, depending on the business-presence test.
- **"Adequate procedures" guidance.** The UK Ministry of Justice guidance (2011) sets out six principles — proportionate procedures, top-level commitment, risk assessment, due diligence, communication and training, monitoring and review. SFO deferred-prosecution agreements referencing adequate-procedures-defence are the practical benchmark.
- **Facilitation payments are prohibited.** Unlike the FCPA (which has a narrow facilitation-payments exception at 15 U.S.C. § 78dd-1(b)), the Bribery Act does not permit facilitation payments. A US-only training programme that treats small facilitation payments as acceptable fails under the Bribery Act.
- **No materiality threshold.** Even a de minimis bribe is prosecutable; prosecutorial discretion is applied under the SFO Code and Joint Prosecution Guidance.

Serious Fraud Office (SFO) is the primary enforcement authority; Crown Prosecution Service and HMRC also enforce.

### Canada — CFPOA

**Corruption of Foreign Public Officials Act (CFPOA)**, S.C. 1998, c. 34. Canadian equivalent of the FCPA. Enforced by the RCMP's International Anti-Corruption Unit; charges typically prosecuted by the Public Prosecution Service of Canada. The 2013 amendments removed the facilitation-payments exception and expanded nationality jurisdiction. Any Canadian national, Canadian company, or company incorporated in Canada is in scope regardless of where the offence occurred.

### France — Sapin II

**Loi n° 2016-1691 du 9 décembre 2016 (Sapin II)** — the French anti-corruption statute, modernising the French regime to approach UK Bribery Act standards. Key provisions for the operator:

- **Article 17 — compliance programme obligation.** Companies with ≥ 500 employees (or belonging to a group of ≥ 500 employees) and ≥ €100M revenue must implement a specified anti-corruption compliance programme covering code of conduct, internal alert mechanism, risk mapping, third-party due diligence, accounting controls, training, disciplinary measures, and internal control / evaluation. **The AFA (Agence française anticorruption)** is the regulator; AFA audits are rigorous and published.
- **Mandatory whistleblower protections** under Loi Sapin II (as amended by Loi 2022-401 implementing the EU Whistleblower Directive). Internal reporting channel required.
- **Convention judiciaire d'intérêt public (CJIP)** — France's deferred-prosecution-agreement equivalent, introduced by Sapin II.

Most startups are below the Article 17 size thresholds. The AFA threshold matters as the US-parent group approaches 500 employees group-wide with meaningful French operations.

### Other jurisdictions

- **Germany** — anti-bribery provisions under Strafgesetzbuch §§ 331–335 (public officials) and § 299 (private corruption).
- **Brazil** — Clean Companies Act (Law 12,846/2013), enforced by the CGU (Controladoria-Geral da União).
- **Italy** — Legislative Decree 231/2001.
- **Japan** — Unfair Competition Prevention Act § 18.

**Operator posture.** Run a single global anti-bribery policy that satisfies the strictest applicable regime (today, the UK Bribery Act's no-facilitation-payments / adequate-procedures / strict-liability framework). Document a single global third-party-due-diligence programme; train the full workforce (US and international) against the global policy; align the French AFA programme as the group approaches Sapin II thresholds. Hub the programme under the GC / Chief Compliance Officer per [mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md).

## Export-control overlay beyond the US EAR / ITAR

The US baseline (EAR, ITAR, OFAC sanctions programmes) is covered in [mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md). International operations amplify the exposure in three ways:

### Deemed-export and foreign-national-access risk

Under the **EAR (15 CFR Parts 730–774)**, the release of controlled technology or source code **to a foreign national in the United States** is deemed an export to the foreign national's country of nationality. Granting a UK, German, or Indian engineer access to EAR-controlled source code or model weights — even if that engineer sits in a US office — is a deemed export requiring the same licence analysis as a physical shipment to the engineer's home country. The international footprint increases the frequency of this analysis sharply: every TN / H-1B / L-1 engineer hired is a deemed-export analysis event.

### Non-US export-control regimes

The US is not the only export-control jurisdiction. Operating from an EU, UK, Japanese, Australian, or Canadian subsidiary layers a second (and sometimes third) export-control regime on the same technology:

- **EU dual-use regulation.** Regulation (EU) 2021/821 (recast of the EU dual-use export-control regulation), setting out the EU-wide dual-use export-control framework. The regulation implements the Wassenaar Arrangement and includes **cyber-surveillance item controls** that reach some AI and software products. Each EU member state operates its own competent authority (German BAFA, French Service des biens à double usage, Dutch Ministry of Foreign Affairs CDIU).
- **UK export-control regime.** Export Control Act 2002 and the Export Control Order 2008; the Export Control Joint Unit (ECJU) is the regulator. Post-Brexit UK operates its own licence regime aligned with but not identical to the EU regulation.
- **Japan.** Foreign Exchange and Foreign Trade Act (FEFTA); METI is the regulator.
- **Canada.** Export and Import Permits Act; Global Affairs Canada's Trade Controls Bureau is the regulator.
- **Australia.** Defence Trade Controls Act 2012; Defence Export Controls (DEC) is the regulator.
- **Wassenaar Arrangement.** The multilateral export-control regime (41 participating states) that establishes the common control-list baseline for dual-use goods and technologies, including some cyber-surveillance and AI-adjacent items. Each participating state implements the Wassenaar lists through its own national regime.

### AI-specific export-control pressure

Since 2022, the US has layered successive **advanced-computing and AI-model** export controls on top of the EAR baseline — the October 7, 2022 interim final rule on advanced computing items to the PRC; the October 17, 2023 updates; the January 2025 "AI Diffusion Framework" rulemaking; and successor instruments. The international footprint is directly implicated: an engineering office in a non-Group-A country, access by a Chinese-national engineer in a UK office, or a model-weights sync to an India datacentre are each events that require current-rule analysis. <!-- needs-research: confirm current state of US advanced-computing and AI-model export controls as of 2025–2026 — the regime has evolved multiple times since 2022 and the AI Diffusion Framework and successor rulings are in motion. -->

### Operator playbook

- **Nationality and location register.** Maintain a register of workforce nationality × workforce location, so every engineering-access decision has the deemed-export analysis ready.
- **Classification register.** Classify the group's technology under the EAR CCL (and the ITAR USML where applicable) — most AI / SaaS tech falls under EAR99 or a specific ECCN; the classification analysis is specialist territory (retain export-control counsel at [mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md)).
- **Access-control integration.** Technology-access systems (code repos, model-weights repos, cloud consoles) must integrate the deemed-export analysis — identity-based access rules referencing both role and nationality / location.
- **Licence-exception awareness.** Several EAR licence exceptions (TMP, BAG, CIV, GOV, APR) reduce the licensing burden for specific use cases; counsel reviews applicability per situation.

## Sanctions-screening amplification for international hires and payments

The sanctions programme ([mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md)) screens customers, vendors, and employees against OFAC's SDN list, EU consolidated financial sanctions list, UK OFSI consolidated list, UN sanctions committee lists, and country-specific lists. The international footprint amplifies the screening surface:

- **Every new international hire** is a screening event — the candidate against the relevant jurisdiction's sanctions lists (OFAC SDN, EU, UK OFSI, UN) with specific attention to the candidate's country of residence, country of nationality, and prior employers.
- **Every intercompany cash transfer** passes through a correspondent-banking chain that applies its own sanctions screening — a transfer blocked at a US correspondent bank because the receiving-side bank or beneficial-owner data triggers a secondary-sanctions hit is a predictable operational hazard when operating in sensitive jurisdictions.
- **Payroll in sanctioned jurisdictions.** Operating payroll in a country that is or becomes subject to sanctions (Russia post-2022, Belarus, Iran, Syria, North Korea, Cuba, Venezuela — the specifics evolve) is a licensing and reputational decision that must be made at the GC / board level, not at the HR level.
- **PEP screening.** Politically exposed persons require enhanced due diligence per OFAC and FinCEN guidance; the international footprint increases the probability of a PEP-adjacent counterparty.

## The country-by-country operational register

For each country in the international footprint, maintain a one-page compliance register with the following fields:

| Field | Content |
|---|---|
| Jurisdiction | Country / region |
| Privacy regime | GDPR / UK GDPR / revFADP / LGPD / PIPL / PDPA / APPI / DPDP / other; regulator; current enforcement priorities |
| Transfer mechanism to US parent | DPF / SCCs + Addendum / IDTA / Chinese SCCs / Section 408 derogation; TIA artefact reference |
| Anti-bribery statute | Bribery Act 2010 / CFPOA / Sapin II / § 299 StGB / Lei 12.846 / other; adequate-procedures evidence pack reference |
| Whistleblower regime | EU Whistleblower Directive transposition / Sarbanes-Oxley / Dodd-Frank / UK PIDA / local equivalent; internal-reporting channel reference |
| Export-control regime | EAR deemed-export analysis / EU 2021/821 / UK ECJU / FEFTA / Export and Import Permits Act / DEC |
| Sanctions overlay | OFAC + EU + UK OFSI + UN + local; screening cadence; blocked-transaction procedure |
| Data-residency obligations | None / sector-specific / full localisation (China CIIO, Russia 242-FZ); mitigations |
| Local DPO / privacy officer | Appointed / not required / regional DPO assigned |
| Last review date | ... |

This register is the operator's single artefact for the privacy / anti-bribery / sanctions / export-control status of each jurisdiction, maintained with the DPO, GC, and the compliance lead. Review quarterly or whenever a regulatory event (new country footprint, major jurisdiction regulatory change) triggers a refresh.

## Concrete example — a US Series-B startup opens UK, Germany, Canada, India

A representative overlay-build for the US Series-B footprint from [chapter 02](./02-first-international-entity-setup.md):

| Jurisdiction | Privacy | Transfer basis to US | Anti-bribery | Export | Notes |
|---|---|---|---|---|---|
| UK Ltd | UK GDPR + PECR | DPF + IDTA + TIA | **Bribery Act 2010** — Section 7 adequate-procedures programme published | UK ECJU + EAR deemed-export | ICO notification; works-council n/a |
| Germany GmbH | GDPR + BDSG; employee-data strict | DPF + EU SCCs + TIA | § 299 StGB; Sapin-II style not applicable | EU 2021/821 (BAFA) + EAR deemed-export | Betriebsrat consultation on HRIS & monitoring systems |
| Canada (ON) | PIPEDA; Quebec Law 25 if hires there | PIPEDA to US with contractual safeguards | **CFPOA** | Export and Import Permits Act + EAR | Provincial variance |
| India Pvt Ltd | DPDP Act (phased) | Pending DPDP rules — contractual safeguards + consent | Prevention of Corruption Act 1988 + FCPA via US-parent reach | India SCOMET controls + EAR | Statutory privacy officer under DPDP once effective |

The pattern is: pick up the specific obligation set per country, hook into the shared programmes (one global anti-bribery policy, one global sanctions-screening programme, one global DPO function with regional support), and document the per-country deltas in the register.

## Anti-patterns

- **Running a US-only privacy programme and treating GDPR as a vendor-DPA problem.** The US parent is the data controller for group-level HR and operations data; GDPR obligations flow to the US parent, not just to vendors.
- **Relying solely on the DPF without a fallback.** DPF has survived two rounds of CJEU scrutiny but faces a third; have SCCs executed and ready to activate if the DPF is suspended.
- **US-only anti-bribery training.** Fails the UK Bribery Act Section 7 adequate-procedures test, which requires training proportionate to the risk — a UK-subsidiary employee who completes only a US-FCPA module is not covered by adequate procedures.
- **Treating deemed-export as a theoretical issue.** Every H-1B / TN / L-1 / foreign-national hire with access to EAR-controlled technology is a licensing event. The analysis is done at hire, not at audit.
- **Operating payroll in a sanctioned country without a licence.** OFAC general and specific licences exist for narrow humanitarian / employee-wind-down purposes; relying on them without counsel review is high-risk.
- **Hoping the Chinese SCC filing survives silence.** Chinese cross-border transfers require a documented filing / assessment path. Operators who process China-origin personal data must engage specialist counsel before structuring the data flow.

## Summary

- **GDPR Chapter V transfers** are the recurring daily event in the US-parent / EU-sub configuration. DPF + SCCs + documented TIA is the operator default; UK IDTA / Swiss Addendum / Chinese SCCs apply in parallel for their respective jurisdictions.
- **Country-specific privacy regimes** (PIPEDA / Law 25, LGPD, PIPL, PDPA, APPI, PIPA, DPDP Act, Australian Privacy Act) each layer on top of GDPR with their own transfer and localisation obligations.
- **UK Bribery Act 2010, Canadian CFPOA, and French Sapin II** reach further than the FCPA on specific axes (no facilitation-payments exception, strict-liability corporate offence under Section 7, Article 17 compliance-programme mandate). Design the global anti-bribery policy to the strictest applicable regime.
- **Non-US export-control regimes** (EU 2021/821, UK ECJU, FEFTA, DEC, Canadian EIPA) and **deemed-export** rules under the EAR amplify the controlled-technology exposure of the international footprint — every foreign-national engineer is a licensing-analysis event.
- **Sanctions screening** amplifies with international hires and intercompany payments; the sanctioned-jurisdiction operational posture must be made at the GC / board level.
- **The country-by-country compliance register** is the operator's single artefact.
- **This chapter owns the overlay.** [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) owns the US privacy programme; [mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md) owns the sanctions and export-controls programme; [chapter 05](./05-international-employment-law-variance.md) owns the works-council co-determination layer that intersects with employee-data processing systems.
