# 1. The GDPR compliance programme — lawful basis, RoPA, DPIAs, DSARs, transfers, and the 72-hour breach clock

> GDPR compliance is not a document. It is a running programme — a Record of Processing Activities that reflects reality, a lawful basis declared per activity and defensible on audit, a DSAR workflow that closes in a month, a Transfer Impact Assessment the DPO can hand the supervisory authority, and a breach clock that starts when awareness lands at any authorised employee.

## Motivation

A US-headquartered Series-B SaaS corporation that acquires its first EU customers crosses a jurisdictional line most founders do not notice at the time. The customer's Data Processing Addendum pulls GDPR Article 28 processor obligations into the deal; the Shared Assessments SIG the customer runs expects an Article 30 Record of Processing Activities on request; the first data-subject access request lands on a general inbox with the Article 12(3) one-month clock already running; the customer's privacy counsel asks for the Transfer Impact Assessment that supports the Frankfurt-to-US-East-1 data flow; and the first in-product incident turns a Security team's weekend into an Article 33 72-hour notification problem the privacy office has three days to characterise, document, and file.

None of that is optional and none of it is drafted the week the first enterprise deal closes. The GDPR compliance programme is a standing operation — a RoPA kept current as systems change, a lawful-basis analysis per processing activity, a DPIA register for high-risk processing, a DSAR workflow wired into product and support, a transfer-mechanism stack with living Transfer Impact Assessments, an Article 27 EU-representative or Article 37 DPO decision on record, and a breach runbook rehearsed before it is needed.

This chapter owns the GDPR substance. The structural anatomy of the DPA itself — controller/processor characterisation, Annex I, Annex II, SCC incorporation, sub-processor list — is authored in [mod-109 chapter 01](../mod-109-commercial-contracts-ip-and-legal-ops/01-customer-contract-suite-msa-sla-dpa-security-aup.md). This chapter is the regulatory depth the DPA refers to.

## Core concepts

### Article 6 — the lawful basis per processing activity

Under GDPR Article 6, every processing activity needs a lawful basis chosen from six grounds: consent (Art. 6(1)(a)), contract (Art. 6(1)(b)), legal obligation (Art. 6(1)(c)), vital interests (Art. 6(1)(d)), public task (Art. 6(1)(e)), and legitimate interests (Art. 6(1)(f)). The basis is declared *before* processing begins, is recorded in the RoPA, is communicated to the data subject under Articles 13–14, and cannot be swapped mid-stream without transparency.

The practitioner default mapping for a B2B SaaS:

- **Delivering the Service to a signed-up customer organisation** — Art. 6(1)(b) contract. The data subject is typically the customer's end-user (employee of the customer); the corporation's lawful basis for processing that end-user's personal data runs through the customer's own processing instruction, with the corporation acting as the Article 4(8) processor.
- **Billing, account administration, mandatory record-keeping** — Art. 6(1)(c) legal obligation (tax law, accounting law) and Art. 6(1)(b) contract.
- **Service security monitoring, abuse detection, fraud prevention** — Art. 6(1)(f) legitimate interests, with the Article 6(1)(f) balancing test documented in the RoPA.
- **Product analytics and improvement using data derived from customer usage** — fact-specific. If the data is aggregated/de-identified under Recital 26, GDPR does not apply. If it remains personal data, Art. 6(1)(f) legitimate interests is the typical hook, subject to the balancing test and transparency.
- **Direct marketing to the customer organisation's commercial contacts** — Art. 6(1)(f) legitimate interests under Recital 47, with an Article 21(2) opt-out for direct marketing and the ePrivacy national-transposition overlay on electronic marketing.
- **AI training on customer prompts or outputs** — not a default. The lawful basis analysis must be run explicitly; see [chapter 09](./09-ai-vendor-and-ai-model-provider-governance-regime.md). EDPB Opinion 28/2024 is the current reference for legitimate interests as a basis for AI training and should be consulted before relying on Art. 6(1)(f) here.

Article 9 special-category data (health, biometric for unique identification, racial/ethnic, political, religious, union, genetic, sex-life, sexual-orientation) adds a *second* lawful basis requirement from the Article 9(2) list on top of Article 6. The default for a non-health SaaS is to avoid ingesting Article 9 data at all; the default for a healthtech is to structure customer processing under Art. 9(2)(h) (provision of health care) with the member-state-law overlay.

### Article 30 — the Record of Processing Activities

Article 30 requires every controller (and, in Art. 30(2), every processor) with 250+ employees or any processing that is not occasional or includes special-category data to maintain a Record of Processing Activities. The required content under Art. 30(1):

- Name and contact details of the controller, joint controllers, DPO, and representative.
- Purposes of the processing.
- Description of the categories of data subjects and the categories of personal data.
- Categories of recipients.
- Transfers of personal data to a third country, with the identification of the transfer mechanism and, where applicable, the documented safeguards.
- Envisaged time limits for erasure of the different categories of data.
- A general description of the technical and organisational security measures.

Article 30(2) imposes a parallel (shorter) record on processors. The RoPA is the single document a supervisory authority reads first in an investigation — it tells the regulator what the controller believes it is doing. A RoPA that does not match the actual data flows is worse than no RoPA: it establishes a pattern of asserted-but-not-performed compliance.

The practitioner discipline is to tie the RoPA to the data-inventory that privacy engineering maintains out of a tool (OneTrust, Transcend, Osano, a home-grown spreadsheet) with named owners per processing activity and a quarterly review cadence. Any new product feature that creates a new processing activity blocks on RoPA entry.

### Article 35 — Data Protection Impact Assessments

Article 35 requires a DPIA when processing is likely to result in a high risk to the rights and freedoms of natural persons. The non-exhaustive Art. 35(3) triggers are systematic and extensive evaluation (including profiling with legal or similarly significant effects), large-scale processing of special categories of data, and systematic monitoring of a publicly accessible area. National supervisory authorities publish Art. 35(4) lists of processing operations that require a DPIA.

The practitioner trigger list for a SaaS:

- Any new AI-in-the-loop feature that produces decisions or recommendations affecting data subjects (hiring, credit, access, content moderation, pricing).
- Any new large-scale collection or combination of personal data.
- Any new special-category processing.
- Any new systematic-monitoring feature (employee productivity, customer behavioural tracking, in-product recording).
- Any new transfer to a country without an Article 45 adequacy decision.

The DPIA documents the processing, assesses necessity and proportionality, assesses risk to data subjects, and sets out safeguards. Under Article 36, if residual risk is still high after safeguards, the controller must consult the supervisory authority *before* processing begins. The practical implication is that a late DPIA — one that surfaces an Article 36 trigger after launch — is a launch-blocker; the programme is wired so DPIAs run alongside design, not after.

### Articles 12–23 — the data-subject-rights machinery

Chapter III of the GDPR gives data subjects access (Art. 15), rectification (Art. 16), erasure (Art. 17), restriction (Art. 18), portability (Art. 20), objection (Art. 21), and a right against solely-automated decision-making with legal or similarly significant effects (Art. 22). Article 12(3) sets the clock: respond "without undue delay and in any event within one month of receipt of the request." The clock is extendable by two further months "where necessary, taking into account the complexity and number of the requests," with notice to the data subject within the first month.

The DSAR workflow is an operations problem. The practitioner implementation:

1. A single intake channel (`privacy@` plus an in-product form), routed to a DSAR tracker with SLA timers tied to the Art. 12(3) clock.
2. Identity verification under Art. 12(6) proportionate to the request.
3. Routing to the systems of record for each data category — CRM, support, billing, product database, data-warehouse, archives, backups-in-scope where Art. 17 erasure applies.
4. A one-month response (or extension notice) with the data subject's rights spelled out.
5. The Art. 12(5) posture on manifestly unfounded or excessive requests — fee or refusal, with the burden on the controller to demonstrate.
6. Where the corporation acts as processor on customer-end-user data, the DSAR is forwarded to the controller under the Art. 28 processor-obligation and the DPA (see [mod-109 chapter 01](../mod-109-commercial-contracts-ip-and-legal-ops/01-customer-contract-suite-msa-sla-dpa-security-aup.md)); the customer is the respondent and the corporation assists.

Article 22 — the right against solely-automated decisions — deserves separate treatment; see [chapter 09](./09-ai-vendor-and-ai-model-provider-governance-regime.md).

### Chapter V — international transfers

Chapter V (Articles 44–50) governs transfers of personal data from the EEA to a "third country." The transfer mechanism stack that must be in place before data leaves:

- **Article 45 adequacy decisions.** Where the European Commission has decided a third country ensures an adequate level of protection, transfers to that country proceed without additional safeguards. The current adequacy decisions include the **EU-US Data Privacy Framework** under [Commission Implementing Decision (EU) 2023/1795](https://eur-lex.europa.eu/eli/dec_impl/2023/1795/oj) for US importers that have self-certified. Adequacy decisions are subject to periodic review and to court challenge — the Schrems II (Case C-311/18) precedent is the reason the DPF is the third US adequacy mechanism rather than the first, and the practitioner default is to *layer* the DPF with SCCs rather than rely on the DPF alone. The DPF remains in force but is under renewed stress: the EU General Court upheld the adequacy decision in September 2025, that ruling is on appeal to the CJEU, and following the US Supreme Court's June 2026 decision in *Trump v. Slaughter* (which bears on FTC-commissioner independence — one of the oversight institutions underpinning the adequacy finding) the European Data Protection Board has asked the Commission to reassess. Track the Commission's review before treating sole-reliance on the DPF as safe.
- **Article 46 Standard Contractual Clauses.** [Commission Implementing Decision (EU) 2021/914](https://eur-lex.europa.eu/eli/dec_impl/2021/914/oj) provides four SCC modules (controller-to-controller, controller-to-processor, processor-to-processor, processor-to-controller). The SCCs are the default transfer mechanism outside adequacy. The UK IDTA (or UK Addendum to the EU SCCs) covers UK GDPR transfers; the Swiss FDPIC addendum covers Swiss FADP transfers.
- **Article 47 Binding Corporate Rules** — for intra-group transfers inside a multinational, with supervisory-authority approval. High fixed cost; typical only at growth stage.
- **Article 49 derogations** — narrow, case-by-case (explicit consent, contract performance, important reasons of public interest). Not a basis for systematic transfers.

Schrems II (Case C-311/18) also requires a **Transfer Impact Assessment** — a documented analysis of whether the third-country importer's local law (surveillance regime, government-access powers, judicial redress) prevents the importer from meeting its SCC obligations in practice. The EDPB **Recommendations 01/2020** (adopted June 2021) are the methodology reference. A TIA that consists of "we signed the SCCs" is not a TIA; the document must describe the data flow, the importer's local legal environment, the supplementary measures (encryption at rest and in transit under a key the importer does not hold, pseudonymisation, binding transparency commitments), and the residual-risk conclusion.

### Article 27 and Article 37 — representative and DPO

**Article 27** requires non-EU-established controllers and processors to designate an **EU representative** in writing, located in a Member State where data subjects are, unless the processing is occasional, does not include large-scale special-category or criminal-conviction data, and is unlikely to result in risk to data subjects. Most non-EU SaaS corporations with EU customers fall inside the Art. 27 requirement and must appoint a representative. The representative is named in the Article 13/14 notice.

**Article 37** requires designation of a **Data Protection Officer** when (a) processing is carried out by a public authority or body, (b) the core activities require regular and systematic monitoring of data subjects on a large scale, or (c) the core activities consist of large-scale processing of special-category data. Member state law may expand the DPO requirement. A SaaS corporation that is a pure B2B processor on small-business customer data usually does not hit the Art. 37 threshold; a corporation that is a controller processing large-scale user behavioural data or that ingests special-category data at scale (healthtech, fintech with biometric authentication, edtech with minors' data) usually does.

Where Article 37 does not apply but an operational privacy-programme owner is nonetheless needed, the practitioner pattern is to designate a privacy-programme owner (privacy counsel, General Counsel, or VP of Privacy Engineering) without calling the role a "DPO," preserving the terminological precision the regulator looks for.

### Articles 33–34 — the 72-hour breach clock

**Article 33(1)** requires the controller, in the case of a personal-data breach, to notify the competent supervisory authority *without undue delay and, where feasible, not later than 72 hours after having become aware of it.* "Aware" is interpreted broadly — awareness at any authorised employee or processor who can reasonably be expected to escalate starts the clock. Article 33(5) requires an internal breach register regardless of whether notification is required.

**Article 34** requires communication to the data subject *without undue delay* when the breach is likely to result in a high risk to the rights and freedoms of natural persons, with limited Art. 34(3) carve-outs (data was unintelligible to the attacker, subsequent measures ensure the high risk is no longer likely to materialise, communication would involve disproportionate effort — and in the last case a public communication substitutes).

**Article 33(3)** specifies the content of the notification: the nature of the breach including categories and approximate number of data subjects and records; the DPO contact; the likely consequences; the measures taken or proposed. A first notification within 72 hours is permitted to be incomplete under Art. 33(4), with information provided in phases as it becomes available.

The practitioner implication is that the 72-hour clock runs during the forensic investigation, not after. A privacy office that waits for the forensic report before filing has missed the clock. The runbook — authored in [chapter 07](./07-incident-response-and-breach-notification-playbook.md) — pre-stages the first-notice template and the escalation path so the first contact with the supervisory authority is paper-ready on day one.

## Concrete example

Vectorline Analytics, a Series-B US-headquartered B2B SaaS with 180 employees and 42 EU-customer tenants across Germany, France, Ireland, and the Netherlands, has an inherited privacy posture that was last reviewed when the corporation had 30 employees. The incoming VP of Privacy has 90 days to stand up the running programme before the next Fortune-500 enterprise diligence cycle. The 90-day plan:

- **Days 1–20.** Inventory every system that processes personal data, interview the owners, and build Draft RoPA v1. Pair each processing activity with a lawful basis under Art. 6 (and Art. 9 where applicable). Identify the EU-representative appointment under Art. 27 (Vectorline has no EU establishment, so Art. 27 applies) and short-list three Irish or Dutch representative-services vendors. Diagnose Article 37 — Vectorline does not hit the DPO threshold on current scope; designate a "Privacy Programme Owner" without calling the role a DPO.
- **Days 21–45.** Author the DPIA register. Three activities are flagged for immediate DPIA: a new in-product AI-in-the-loop forecast feature, a customer-success product-usage data warehouse that joins anonymous usage to employee email, and a deprecating-but-still-live customer-side export that reaches personal data outside the agreed Annex I scope. The AI feature's DPIA (see [chapter 09](./09-ai-vendor-and-ai-model-provider-governance-regime.md)) is the first launch-blocker in two years.
- **Days 46–60.** Author the DSAR workflow — single `privacy@` and in-product intake, DSAR tracker tied to Art. 12(3) one-month SLA, system-of-record routing map, controller-DSAR-vs-processor-DSAR branch under Art. 28, and the Art. 12(5) manifestly-unfounded posture. Fire a tabletop DSAR at the end of the two weeks.
- **Days 61–75.** Author the Transfer Impact Assessment for the Frankfurt-to-US-East-1 flow. Vectorline is DPF-self-certified on the Commerce list and carries the 2021/914 SCCs in its DPA with the UK IDTA and Swiss addendum layered on; the TIA documents the supplementary encryption-in-transit-and-at-rest posture, the key-management model where EU customer keys are held at a European KMS endpoint and never exposed to US ops, and the residual-risk conclusion. Any residual-risk finding of "high" routes to Article 36 prior-consultation review before the next sync.
- **Days 76–90.** Author the Articles 33/34 runbook, pre-stage the first-notice template, run a tabletop breach, and wire the Privacy on-call into the Security on-call. Report the 90-day completion to the audit committee ([mod-111 chapter 04](../mod-111-corporate-governance-board-operations-and-officer-duties/)); book the quarterly privacy report into the committee cadence.

At the 90-day mark, Vectorline's privacy counsel can produce the RoPA, the DPIA register, the DSAR workflow, the TIA library, the Art. 27 representative appointment, the Articles 33/34 runbook, and the quarterly report on the day the next enterprise buyer or supervisory authority asks.

## Summary

- GDPR compliance is a running programme, not a document — the components are the Article 6/9 lawful-basis analysis, the Article 30 RoPA, the Article 35 DPIA register (with Article 36 prior-consultation posture), the Articles 12–23 data-subject-rights workflow honouring the Article 12(3) one-month clock, the Chapter V transfer stack with Transfer Impact Assessments, the Article 27 representative or Article 37 DPO designation, and the Articles 33–34 breach-notification runbook.
- The lawful-basis analysis is per processing activity and recorded in the RoPA. Article 9 adds a second lawful-basis requirement for special-category data. AI training as a processing activity requires an explicit analysis — see [chapter 09](./09-ai-vendor-and-ai-model-provider-governance-regime.md).
- The RoPA is the first document a supervisory authority reads; a RoPA that does not match actual data flows is worse than no RoPA.
- DPIAs are triggered by Article 35(3) plus the supervisory-authority Art. 35(4) lists. Residual high risk invokes Article 36 prior consultation — a launch blocker that must be caught at design, not post-launch.
- The transfer stack layers Article 45 adequacy (including the DPF under Decision (EU) 2023/1795), Article 46 SCCs under Decision (EU) 2021/914 (with UK IDTA and Swiss addendum), and Article 47 BCRs where intra-group. A Transfer Impact Assessment under the Schrems II (C-311/18) framework and EDPB Recommendations 01/2020 must accompany every non-adequacy transfer.
- Article 27 representatives are near-universal for non-EU B2B SaaS with EU customers; Article 37 DPO designation is fact-specific and avoided-by-terminology where not triggered.
- The Articles 33/34 clock starts at awareness, not at forensic certainty. The runbook ([chapter 07](./07-incident-response-and-breach-notification-playbook.md)) pre-stages the first notice so the first contact with the supervisory authority is paper-ready on day one.
- The structural DPA anatomy belongs to [mod-109 chapter 01](../mod-109-commercial-contracts-ip-and-legal-ops/01-customer-contract-suite-msa-sla-dpa-security-aup.md); this chapter authors the regulatory substance the DPA refers to.
