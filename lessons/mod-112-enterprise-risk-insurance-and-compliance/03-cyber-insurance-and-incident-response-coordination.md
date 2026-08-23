# 3. Cyber insurance and incident-response coordination

> Cyber insurance is not "insurance you buy and forget." The policy is an incident-response operating manual, and the carrier is a live participant in a real incident. A CISO who has not walked the notification workflow with the carrier **before** an incident will lose critical hours during one.

## Motivation

Cyber policies changed shape between 2020 and 2024. Ransomware losses drove a hard market; underwriters imposed control requirements as underwriting conditions; sub-limits on ransomware and funds-transfer fraud tightened; war-and-cyber-war exclusions were rewritten; systemic-cyber-event exclusions were introduced. A cyber policy purchased three renewal cycles ago is not the cyber policy you need today, and every clause matters at claims time.

More importantly, the incident-response side of the policy has become **operational infrastructure**. Modern carriers maintain a panel of pre-approved breach counsel, forensics firms, notification vendors, and ransomware negotiators. The policy conditions coverage on using them — or requires carrier consent to use others. The 24×7 hotline number, the notification deadline, the coverage-under-reservation letter format, and the panel roster are all things that must be **socialised inside the security team before an incident**, not discovered during one.

This chapter covers the cyber-insurance layer and the incident-response coordination pattern the CISO and GC operate together with the carrier. It does **not** cover the underlying security programme (SOC 2 / ISO 27001, security engineering technique) — that substance lives in [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) and in the `security-learning` curriculum. Insurance and controls are complementary; the underwriter's application questions describe the controls the insurer expects to see.

## Coverage components

Cyber policies split into **first-party** (loss to the insured) and **third-party** (liability to others) coverage parts.

**First-party.**

- **Breach response costs.** Forensic investigation, legal counsel (breach counsel), individual and regulator notification, credit monitoring and identity-protection services for affected individuals, call-centre services, crisis-communications / PR support. Frequently the most-used part of the policy.
- **Business interruption and contingent business interruption.** Lost income during a cyber-caused outage of the insured's systems (BI) or a covered supplier's systems (CBI). Watch the **waiting period** (typically 8–24 hours before coverage attaches) and the **period of restoration** (how long income loss is covered — hours-based or days-based).
- **Cyber extortion.** Ransomware negotiation, ransom-payment reimbursement (where legal — see the OFAC discussion below), and extortion-consultant fees. Ransomware coverage is one of the most heavily sub-limited areas of the policy.
- **Data restoration.** Costs to restore or recreate data damaged, corrupted, or destroyed by a covered event.
- **Funds-transfer fraud.** Coverage for funds transferred out of the insured's account as a result of fraudulent instruction. Overlaps with Crime / Fidelity (see [chapter 02](./02-startup-insurance-stack-by-stage.md)); the seam between the two is where social-engineering losses fall.
- **Regulatory defence and fines.** Defence costs for regulatory proceedings (FTC, state AG, HHS OCR for HIPAA, EU DPA for GDPR) and, where insurable by law, the fines themselves. Insurability of fines varies by jurisdiction — some GDPR fines are held uninsurable as a matter of public policy in some EU member states. <!-- needs-research: verify current position of major EU DPAs on insurability of Article 83 GDPR fines and cite the specific national law or DPA guidance. -->

**Third-party.**

- **Network security liability.** Damages payable to third parties as a result of an unauthorised intrusion, malware transmission, DDoS, etc.
- **Privacy liability.** Damages payable to third parties for a privacy violation — breach of PII, breach of contractual privacy obligation, statutory privacy claims (CCPA private right of action for certain breaches — see [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/)).
- **Media liability.** Defamation, copyright infringement, trademark infringement in the insured's content. Increasingly relevant for AI-generated content.
- **PCI assessment defence.** Defence and (where covered) indemnity for PCI-DSS assessments arising from a card-brand-mandated forensic investigation. Coverage varies materially; read carefully.

## Sub-limits and exclusions to watch

Modern cyber policies are shaped as much by their exclusions as by their grants. Read the following at every renewal:

- **Ransomware sub-limits.** Frequently sub-limited to a fraction of the aggregate limit. A $10M aggregate policy may cap ransomware at $2M–$5M.
- **Funds-transfer-fraud sub-limits.** Typically the smallest sub-limit on the policy — often $250k–$500k for a mid-market startup.
- **Social-engineering / impersonation-fraud coverage.** Often affirmed by endorsement only; check that it is present, that it covers vendor-impersonation and payroll-diversion patterns, and that the sub-limit is meaningful.
- **War and cyber-war exclusions.** The Lloyd's Market Association introduced revised state-backed cyber-war exclusion clauses (LMA5564 through LMA5567) that expanded exclusion for state-attributed cyber operations. <!-- needs-research: confirm the LMA5567 language and any subsequent revisions or U.S.-market equivalents (ISO CG 21 06 or the corresponding cyber form endorsement) and cite. --> Attribution to a state actor is a legal question and the policyholder rarely controls it.
- **Widespread-event / systemic-cyber-event exclusions.** Some carriers now exclude coverage for losses tied to a widespread event affecting many insureds simultaneously (a large cloud-provider outage, a widespread software-supply-chain compromise). These are typically defined by count-of-insureds-affected or dollar-of-market-loss triggers.
- **Unencrypted-mobile-device exclusions.** Losses arising from unencrypted mobile devices may be excluded — a real problem if BYOD is your policy.
- **Prior-and-pending-litigation exclusions and known-circumstances exclusions.** Anything the insured knew or should have known about before the policy period is out of scope. This is why the application's no-known-incidents attestation matters.
- **Regulatory-fine exclusions for specific regulators or jurisdictions.** Some policies exclude specific regulatory regimes; read the schedule.
- **Bodily-injury and property-damage exclusions.** Cyber policies generally exclude BI and PD — those risks are covered under GL. The seam matters for cyber-physical incidents (a compromised IoT device causes injury); confirm the intercoverage answer.

## The carrier's incident-response panel

Modern cyber carriers maintain a **panel** of pre-approved incident-response providers:

- **Breach counsel** (specialised law firms — commonly Mullen Coughlin, Wilson Elser, Baker Hostetler, Alston & Bird, Constangy, Lewis Brisbois, others; the panel varies by carrier).
- **Digital-forensics firms** (Mandiant / Google Cloud, CrowdStrike, Kroll, Arete, Charles River Associates, others).
- **Notification vendors** (Epiq, Kroll, TransUnion, Experian — for large-volume individual notification, credit monitoring, call-centre).
- **PR / crisis-communications firms.**
- **Ransomware negotiators** (Coveware, GroupSense, Arete, others).

Using **off-panel** providers usually requires **carrier consent** and may result in reduced-rate reimbursement or coverage denial for the off-panel spend. The practical implication:

- At policy bind (and again at renewal), **obtain the panel roster in writing**.
- **Socialise the roster with the CISO, GC, and executive incident-response team** before an incident.
- **Pre-brief a shortlist** — the breach-counsel firm the GC would call first, the forensics firm the CISO would engage first. Some breach counsel firms will run a no-cost preparatory call to establish the relationship.
- **Add the 24×7 hotline number to the IR runbook** — laminated card in the SOC, page in the runbook, saved contact in the incident-commander's phone.

## Pre-loss touchpoints

The set of things to confirm with the carrier **before** an incident:

1. **The 24×7 incident-response hotline number.** Some carriers have separate hotlines for extortion / ransomware events.
2. **Notification deadlines.** Typically framed as "as soon as practicable" but often paired with a hard outside window (30 days is common). Late notice is a coverage-defence pathway; do not test it.
3. **Sub-limits and retentions per coverage part.** Know before the incident whether ransomware, funds-transfer, or business-interruption has a lower cap or retention than aggregate.
4. **Trigger definitions.** Many policies now require formal "incident" or "claim" declaration by breach counsel to trigger coverage — a suspected intrusion under internal investigation may not itself be a covered event.
5. **Reservation-of-rights protocol.** Understand what a coverage-under-reservation letter looks like from this carrier and how it interacts with panel-provider engagement.

## Application discipline — the security-controls crosswalk

The cyber-insurance application has become an inventory of security controls. The application is where the underwriting decision is made and where the coverage-denial argument is prepared. Common attestations (varies by carrier):

- **Multi-factor authentication (MFA)** on all remote access, all administrative access, all privileged accounts, all email access, and all VPN access.
- **Endpoint Detection and Response (EDR)** deployed on 100 % of endpoints and servers, monitored 24×7 (in-house SOC or MSSP).
- **Immutable, tested backups** with a documented Recovery Time Objective (RTO) and Recovery Point Objective (RPO); backups are air-gapped or immutable; annual restore test.
- **Written incident-response plan** tested at least annually via tabletop exercise.
- **Vendor / supply-chain risk-management programme** with tiered risk assessment, SOC 2 collection, and contractual security requirements.
- **Vulnerability-management and patch cadence** — critical patches within a stated window (7 or 14 days), high within 30 days, etc.
- **Security-awareness training** for all employees at hire and annually thereafter, including phishing simulation.
- **Email security** — DMARC / SPF / DKIM enforcement, malicious-attachment sandboxing.
- **Segmentation** — production networks isolated from corporate networks; privileged-access workstations for administrators.
- **Logging and monitoring** — centralised log aggregation, monitored alerts, retention for the incident-response and forensics window.

Each answer is a **warranty**. "Yes" on MFA when a break-glass account bypasses MFA is a misrepresentation that will surface in an incident forensic and be raised by the carrier as a coverage defence. The CISO owns the truthful sourcing; the signatory (typically the CEO, CFO, or CISO) owns the personal attestation. If a control is deployed with exceptions, document the exceptions in the application supplement — carriers understand exceptions and price for them; they do not tolerate discovery of undisclosed exceptions after loss.

## The claims workflow

A working sequence, from detection through carrier engagement:

1. **Detect and triage internally.** The internal incident-commander confirms a real incident. Do **not** yet engage the carrier or off-panel providers.
2. **Engage breach counsel first — for privilege.** Breach counsel is engaged before forensics so that forensics work product is directed by counsel and covered by attorney-client privilege and work-product doctrine. Engaging forensics directly (without counsel-direction) leaves the forensic report discoverable in later litigation.
3. **Breach counsel notifies the carrier.** Standard practice is that breach counsel sends the first notice, framed as a preservation-of-rights notification, using the carrier's required channel (hotline, portal, or email). Expect a **coverage-under-reservation letter** back within 24–72 hours acknowledging the notice and reserving the carrier's rights.
4. **Forensics engaged under breach-counsel direction.** The engagement letter names breach counsel as the party engaging the forensics firm on behalf of the insured for the purpose of providing legal advice — the standard structure to preserve privilege.
5. **Parallel workstreams.** Technical containment runs in parallel with the legal / notification / regulatory workstream. Sequencing is critical: containment cannot wait for legal, but external notification cannot precede legal review. The breach-counsel-plus-incident-commander pairing sequences the two.
6. **Ongoing carrier updates through breach counsel.** Do not let unrepresented company personnel make direct statements to the carrier about the incident. Every substantive communication runs through counsel.
7. **Notification decision.** Breach counsel makes the individual and regulator notification decision applying the relevant statutes — state breach-notification laws, HIPAA (if PHI is implicated), GLBA, GDPR Article 33 (72-hour DPA notification), CCPA Sections 1798.29 / 1798.82. Substance owned in [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/); the sequencing lives here.
8. **Public disclosure.** Where required by SEC Regulation S-K Item 106 (for public companies) or by material-event 8-K reporting (SEC 2023 cybersecurity disclosure rules — 17 CFR §§ 229.106, 249.308), the disclosure is timed and drafted under counsel supervision. <!-- needs-research: verify current 8-K Item 1.05 four-business-day materiality-triggered disclosure requirement and any subsequent SEC guidance or amendments. -->
9. **Post-incident review.** After containment and notification, a written after-action report goes to the executive team and the audit committee. Feeds the next-year application discipline and the ERM register ([chapter 01](./01-enterprise-risk-management-operating-framework.md)).

## Ransomware payment — the OFAC gate

Ransomware payment is not a straightforward "buy the decryption key" transaction. **OFAC** (Office of Foreign Assets Control) prohibits payments to Specially Designated Nationals and to persons subject to comprehensive sanctions. Many ransomware operators — Conti, LockBit affiliates, Evil Corp, and others — have been designated. A payment to a designated party without an OFAC licence is a **strict-liability violation** of the sanctions programme.

Treasury OFAC's advisories on ransomware payments — the **October 2020** advisory and the **September 2021** updated advisory — laid out the framework: victims and their agents (including insurers, incident-response firms, and financial institutions facilitating payment) can face civil enforcement even without knowledge of the sanctioned status of the recipient. Mitigating factors include a strong sanctions-compliance programme, timely and complete self-reporting to OFAC and to CISA, and cooperation with law enforcement. <!-- needs-research: cite exact URLs for the October 1, 2020 "Advisory on Potential Sanctions Risks for Facilitating Ransomware Payments" and the September 21, 2021 "Updated Advisory on Potential Sanctions Risks for Facilitating Ransomware Payments" on ofac.treasury.gov; confirm no superseding advisory since. -->

Practical implications:

- **Sanctions screening runs before any payment.** The carrier and the ransomware-negotiation firm will screen the wallet address, the ransomware family, and any identifiable actor against OFAC lists.
- **A hit is a hard stop.** Payment cannot proceed without an OFAC licence — and licences for ransomware are, by policy, presumptively denied.
- **Report to OFAC and CISA regardless of payment.** Timely voluntary self-disclosure is a mitigating factor even if payment occurs; failure to report can eliminate the mitigation.
- **The GC and outside sanctions counsel are involved before the CISO makes a payment recommendation.** See [chapter 04](./04-sanctions-and-export-controls-compliance-programme.md) for the wider sanctions programme.

## Coordination with the underlying security programme

The cyber-insurance layer sits on top of the security programme. The two must speak the same language:

- The application-warranty inventory is the **same list of controls** the security programme is building against SOC 2 Trust Services Criteria, ISO 27001 Annex A, and NIST CSF 2.0.
- **A control that the insurer will not accept ("MFA on all administrative access, no exceptions")** must be a control the security programme actually operates. If the security programme cannot commit to the standard, do not warrant it; negotiate the endorsement.
- **A gap surfaced by insurance renewal** is a real security gap. Cyber-insurance renewals are one of the most efficient control-gap discovery mechanisms available to the CISO.

Substance of the underlying security programme, including SOC 2, ISO 27001, HIPAA / GLBA / PCI-DSS sector compliance, and privacy compliance (GDPR / CCPA / state privacy laws), sits in [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/). Security-engineering depth (network security, application security, cryptography engineering) sits in the `security-learning` curriculum.

## A concrete 72-hour timeline

For orientation, a representative timeline for a mid-sized cyber incident:

- **T + 00:00.** EDR alerts on suspicious lateral movement from a compromised customer-support laptop.
- **T + 00:45.** SOC escalates to incident commander (Head of Security Engineering). Triage confirms real intrusion.
- **T + 01:30.** Incident commander notifies CISO and GC. Internal incident bridge stood up.
- **T + 02:00.** GC contacts breach-counsel panel firm (using pre-briefed contact). Verbal engagement confirmed; written engagement letter to follow.
- **T + 03:00.** Breach counsel notifies the cyber carrier via the 24×7 hotline. Case number assigned. Reservation-of-rights letter expected within 48 hours.
- **T + 04:00.** Breach counsel engages panel forensics firm on behalf of the insured. Kickoff call at T + 06:00.
- **T + 06:00.** Forensics kickoff. Scope: root-cause, blast-radius, data-exfiltration determination. Immediate containment (endpoint isolation, credential rotation) proceeds in parallel under CISO direction.
- **T + 12:00.** Preliminary containment. Compromised account credentials rotated. Affected endpoints isolated. Log collection preserved for forensics.
- **T + 24:00.** Forensics preliminary read: intrusion vector identified (phishing → credential theft → lateral movement via legacy service account without MFA). Data exfiltration under investigation.
- **T + 48:00.** Forensics preliminary determination on exfiltration scope. Breach counsel begins the state-by-state notification analysis. First carrier update. Executive-team briefing.
- **T + 72:00.** Notification decision matrix drafted. Regulatory notification timing (state AGs, HHS OCR if applicable, EU DPA if applicable) plotted against statutory deadlines. Board audit-committee notification prepared.

Every one of those decision points references a policy provision, a statute, or an internal runbook. The runbook is the artifact that lets the sequence execute on time.

## Ownership boundary

- **The cyber-insurance policy, the carrier relationship, and the incident-response coordination workflow with the carrier**: this chapter.
- **The security programme (SOC 2, ISO 27001, HIPAA, GLBA, PCI-DSS, privacy law compliance including GDPR / CCPA / state privacy laws, and the substance of breach-notification obligations)**: [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/).
- **Security-engineering depth (network, application, identity, cryptography engineering, IR engineering technique)**: `security-learning` curriculum.
- **The wider insurance stack, broker selection, and application-warranty discipline in general**: [chapter 02](./02-startup-insurance-stack-by-stage.md).
- **The sanctions-programme substance behind the OFAC ransomware-payment gate**: [chapter 04](./04-sanctions-and-export-controls-compliance-programme.md).
- **Board reporting on cyber incidents and the CISO's Caremark oversight duty**: [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).

## Summary

- **Cyber insurance is an incident-response operating manual, not a policy on the shelf.** Panel providers, hotline numbers, notification deadlines, sub-limits, and exclusions must be socialised inside the security and legal teams before an incident.
- **Coverage is shaped by exclusions.** Read the war / cyber-war (LMA5567 and successors), widespread-event, unencrypted-device, and known-circumstances exclusions at every renewal; watch the sub-limits on ransomware and funds-transfer fraud.
- **Application answers are warranties.** The MFA / EDR / backup / IR-plan / vendor-risk / patch / training attestations are the same list of controls the security programme is building; misrepresentation surfaces in the incident forensic.
- **Breach counsel is engaged first for privilege.** Counsel notifies the carrier; counsel engages forensics; every substantive carrier communication runs through counsel.
- **Ransomware payment is OFAC-screened before payment.** A hit is a hard stop; report to OFAC and CISA regardless. See [chapter 04](./04-sanctions-and-export-controls-compliance-programme.md).
- **The claims workflow runs technical containment and legal notification in parallel**, sequenced by the breach-counsel + incident-commander pair.
- **The cyber-insurance renewal is a control-gap discovery mechanism.** Treat gaps found at renewal as real security gaps to remediate.
