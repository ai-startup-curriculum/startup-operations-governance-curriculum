# 5. The SOC 2 audit-readiness programme (governance side) — scope, criteria, auditor, timeline, automation, and the boundary with security engineering

> A SOC 2 report is two documents at once. To the buyer's procurement team it is a tick-box artefact that unblocks a purchase order. To the governance team it is a public attestation that the corporation operates a described system of internal control, signed by a licensed CPA firm under AICPA attestation standards, and warranted to a sample period. The two readings have different owners, and the governance side must stand up **before** the engineering side can be audited.

## Motivation

A Series-B SaaS targeting Fortune-500 buyers hits a predictable wall. Procurement asks for "your SOC 2," the sales engineer sends a one-pager, procurement escalates to the buyer's infosec team, and the deal pauses until the independent auditor's report is in a reviewable form. At this stage there is no report, no auditor, no sample period, and no automation platform. The window from "we need SOC 2" to "we have a report a Fortune-500 infosec team will accept" is typically **6–12 months to a Type I and a further 12 months to a Type II**, and every week of that window is a week the enterprise pipeline stalls.

The SOC 2 audit-readiness programme is a governance programme first. The decisions that shape the report — Type I versus Type II, which Trust Services Criteria to scope in, which audit firm to engage, which compliance-automation platform to deploy, how the audit committee is briefed, when to bridge to ISO 27001 or HITRUST — are made by the GC, CISO, and audit-committee chair before the first engineering gap-assessment runs. The engineering of the controls themselves (identity, access, network, logging, vulnerability management, SDLC) belongs to a different curriculum. This chapter owns the programme; the `security-learning` and `ai-infra-security-solutions` curricula own the controls.

This chapter sequences the governance-side decisions so the engineering side has a stable brief to execute against.

## Core concepts

### Type I versus Type II — the AT-C 105 / AT-C 205 framing

SOC 2 is an attestation engagement performed under AICPA Statement on Standards for Attestation Engagements (SSAE) 18 — operationally the AT-C 105 (common concepts) and AT-C 205 (examination engagements) sections of AICPA Professional Standards. The report is signed by a licensed CPA firm; it is not an opinion on the corporation issued by a self-styled auditor.

Two report types matter at the governance layer:

- **SOC 2 Type I.** Attestation on the **design** of controls at a **point in time**. The auditor evaluates whether the corporation's described controls, as of a specified date, are suitably designed to meet the Trust Services Criteria selected for the engagement. Type I is a design opinion, not an effectiveness opinion. It is faster to produce — a well-prepared Series-B can often reach Type I within 6–12 months of the decision — and it is the deliverable that unblocks procurement at buyers whose infosec teams will accept a Type I as evidence of a maturing programme.
- **SOC 2 Type II.** Attestation on both **design** and **operating effectiveness** across an **observation period**. Observation windows commonly run 3 to 12 months, with **12 months the diligence default** at large enterprise buyers and the only window that supports an annual renewable attestation cycle. Type II is the report Fortune-500 infosec teams expect at renewal.

Between consecutive Type II reports there is a gap — the period between the end of one report's observation window and the start of the next. Enterprise buyers close the gap with a **bridge letter** (also called a gap letter) in which the corporation's management asserts that, between the prior report's end date and a stated current date, no material changes have occurred to the controls described in the prior report. The bridge letter is a management letter, not an auditor's opinion; counterparties know this and accept it as a stopgap for weeks, not quarters.

The sales-enablement trade-off is explicit. A Type I deliverable signed in month 9 can unblock enterprise procurement that would otherwise not accept the corporation through gatekeeping until month 18 (Type II). The governance decision is whether to invest in a Type I deliverable as a bridge, or to run straight to Type II at the cost of a longer sales freeze.

A third artefact matters at the programme boundary: the **SOC 3 report**, a general-use summary derived from the Type II that may be publicly distributed. SOC 3 is not a replacement for Type II — it carries less detail and does not identify controls in a form the buyer's infosec team will accept for a decision. Governance treats SOC 3 as marketing distribution for the restricted-use SOC 2.

The governance choice between Type I and Type II also drives a procurement-team behaviour pattern. Enterprise buyers whose infosec teams have internal "SOC 2 Type II required" policies will not budge on the type question; buyers whose infosec teams have discretion will accept Type I when the engagement letter for Type II is in evidence and the observation-window clock is running. The GC should treat these as two distinct buyer archetypes when modelling sales-pipeline conversion.

### Trust Services Criteria — Security default, the other four as customer-driven scope

The AICPA Trust Services Criteria (TSC) 2017, as periodically revised, define the five criteria categories against which a SOC 2 engagement is scoped:

- **Security** — the "common criteria" (CC-series), always included in any SOC 2 report. Covers logical and physical access, change management, risk assessment, monitoring, communication, control environment.
- **Availability** — the system is available for operation and use as committed or agreed. Scoped in where the customer contract has uptime commitments or the buyer's infosec review asks for availability coverage.
- **Confidentiality** — information designated as confidential is protected. Scoped in where the customer contract has confidentiality obligations beyond generic security.
- **Processing Integrity** — system processing is complete, valid, accurate, timely, and authorised. Scoped in for payments, trading, clearing, regulated transactional systems — rarely a default for generic SaaS.
- **Privacy** — personal information is collected, used, retained, disclosed, and disposed of to meet the entity's commitments. Scoped in where the customer deals, regulator posture, or market expectation demand a privacy TSC attestation beyond GDPR / CCPA operational compliance.

Security is the default on every SOC 2. The other four are added by customer-driven need, and each addition has a material cost. Adding **Privacy** in particular pulls into audit scope the consent, retention, deletion, and notice mechanics that are already governed by [chapter 01 on GDPR](./01-gdpr-compliance-programme.md); the TSC privacy criteria are not identical to GDPR obligations and mapping them is non-trivial. The governance question is whether the addressable buyers will insist on the Privacy TSC or whether a separate ISO 27701 or GDPR attestation serves the same procurement purpose at lower audit-scope cost.

The criteria-expansion cost has four components. First, **additional control objectives** — each added TSC category introduces category-specific criteria the control environment has to satisfy. Second, **additional evidence surface** — control owners for the new criteria produce quarterly or annual evidence packets at the automation platform. Third, **additional fieldwork hours** — the auditor samples a broader control set and the engagement fee rises accordingly. Fourth, **additional management-representation scope** — the management letter the CEO and CISO sign at report issuance covers the expanded criteria, and the board's officer-liability posture under [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/) attaches to the broader attestation.

The governance test for adding a TSC category is a simple decision: does an addressable Fortune-500 buyer's procurement questionnaire require it, or does an addressable regulator expect it? If neither, the category is deferred. "Nice to have" is not a sufficient governance basis for an expanded TSC scope.

### Audit-firm selection — Big 4, Big 4-adjacent, boutique / SOC-specialist

The market segments into three tiers. Fee bands and specific market-share claims are not stated here; <!-- needs-research: confirm current fee ranges, market share, and auditor-network data before quoting any specific figure. -->

- **Big 4.** Deloitte, PwC, EY, KPMG. Highest customer recognition — a Fortune-500 buyer's infosec team recognises the signature on sight. Dual-report capability across SOC 2, ISO 27001, HITRUST, PCI, and under some conditions FedRAMP. Review intensity is high and cycle times are long; the Big 4 are typically not the right fit for a first-time SOC 2 at Series B unless the parent-company relationship already exists.
- **Big 4-adjacent.** BDO, Grant Thornton, RSM, Crowe, Baker Tilly. Mid-market national firms with licensed CPA teams running attest engagements. Recognisable to most Fortune-500 infosec reviewers, materially more responsive to a Series-B client than a Big 4 team, and typically able to issue SOC 2 and ISO 27001 side by side.
- **Boutique / SOC-specialist.** A-LIGN, Schellman, Prescient Assurance, Coalfire, Insight Assurance, Sensiba, Johanson Group, and others. These firms specialise in attestation at venture-backed scale; many run high volumes of SOC 2 Type I and Type II engagements each year, maintain partnerships with the compliance-automation platforms, and will meet a Series-B timeline the national firms will not match. Customer recognition is strong inside the technology-buyer segment and weaker outside it — a Schellman or A-LIGN signature is fully recognised by a Fortune-500 technology-sector infosec team and may need a brief explanatory note inside a regulated-industry buyer's procurement.

Dimensions that matter across the three tiers:

- **Customer recognition.** The question the GC asks is: "will the Fortune-500 buyer's infosec team recognise this auditor on sight?" A yes unblocks procurement; a no triggers an auditor-credentials question the sales engineer has to answer.
- **Review intensity.** Big 4 engagements run heavy on documentation and management-representation questioning. Boutique SOC specialists run leaner engagements calibrated to the automation-platform evidence feed.
- **Dual-report capability.** A single auditor issuing SOC 2 + ISO 27001 + HITRUST from one evidence set reduces the audit-fatigue cost materially for the engineering team. The dual-report capability matters more as the corporation scales into healthcare, international, or federal segments.
- **Auditor-network partnerships with the automation platforms.** Boutique SOC specialists maintain formal partnerships with Vanta, Drata, Secureframe, Thoropass, and others; the partnerships drive evidence-collection efficiency during fieldwork.
- **Personnel continuity.** Who is the senior associate on the engagement, and how often does the firm rotate them? Continuity across years one and two matters more than firm brand in the operating experience.
- **Engagement-letter wording.** The engagement letter is a contract under the AICPA attestation framework and the commercial-contracting principles from [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/). The GC should read it as a commercial document: scope, deliverable, management-representation obligations, limitation of liability, termination, rework obligations on an issued-report error. A clean engagement letter at year one avoids every renewal becoming a renegotiation.
- **Independence posture.** The AICPA independence rules constrain the auditor's non-attest services to the client. A firm that is the SOC 2 auditor cannot also provide operational security consulting or implement the controls it audits. Governance maintains the independence boundary at engagement letter and tracks any service-expansion request against it.

### Audit-preparation timeline — 6-12 months to Type I, +12 months to Type II

The practitioner default timeline from decision to Type I report is 6 to 12 months. The phases:

1. **Scope and criteria selection** (weeks 0–4). GC, CISO, and audit-committee chair select Type I versus Type II, select TSC scope (Security always, plus customer-driven additions), define the system boundary (which products, which cloud accounts, which data stores, which supporting business units).
2. **Readiness assessment / gap assessment** (weeks 4–12). The chosen auditor, or a separate readiness-assessment firm, maps the current control environment against the selected TSC and produces a gap list. The governance decision is whether to run the readiness assessment with the audit firm (efficient, but reduces the firm's independence appearance) or with a separate practitioner.
3. **Remediation sprint** (weeks 8–20, overlapping with phase 2). Engineering closes the gaps — the controls themselves are designed and operated by the security-engineering function (see hand-off below). The governance side tracks remediation progress and signs off on completion.
4. **Observation window begins** (week 20, for Type II). The Type II observation window starts when the controls are in place; nothing before that date counts as sample-period evidence.
5. **Sample-period evidence collection** (weeks 20–48 for a 6-month Type II, weeks 20–72 for a 12-month Type II). The automation platform streams evidence from integrated systems; the control owners respond to sample requests; the governance side reviews the evidence completeness report on a monthly cadence.
6. **Auditor fieldwork** (typically 4–8 weeks after the observation window closes). The auditor performs sampling, interviews control owners, tests exceptions, and drafts the report. The GC manages representation letters and management-response wording on any exceptions.
7. **Report issuance.** The auditor issues the final SOC 2 report. The report is distribution-controlled under the AICPA restricted-use clause.

Pre-SOC-2-Type-I enterprise SaaS can still sell, but the window is short. The sales engineer carries a **readiness statement** — a management-signed description of the controls, the automation-platform evidence screenshots, the auditor-engagement letter, the planned report date — and uses it for a bridge period of weeks, not quarters. Procurement teams will accept a readiness statement from a credible seller for a defined window; they will not accept it as the end state.

A timeline-risk checklist the GC runs at week 0:

- Is the auditor's engagement letter signed, or merely out for signature? A verbal commitment is not an engagement.
- Is the readiness assessment firm the same as the audit firm? If so, is the independence appearance acceptable to the audit committee?
- Is the automation platform contracted with integration coverage for every in-scope system? Missing integrations become manual-evidence tickets at fieldwork.
- Is the system boundary documented in writing, with product scope, environment scope, and supporting-function scope named? Scope drift during observation is an auditor finding.
- Is the control-owner RACI published and acknowledged by each named owner? Un-acknowledged ownership becomes a sample-request-missed finding.

### Auditor-interaction mechanics during fieldwork

Fieldwork is where the governance programme meets the auditor's sampling discipline. Three mechanics shape the experience.

**Sampling.** The auditor selects samples from the population of control executions in the observation window — access reviews completed, changes deployed, incidents triaged, backups restored, new-hire security trainings completed. Sample sizes follow AICPA sampling guidance and the auditor's internal methodology; a quarterly control typically draws 2 samples in a 12-month window, a monthly control draws 3–5, a continuous control draws statistically from the population. Governance-side implications: every control must retain evidence for every execution across the observation window, not just a representative subset.

**Exception handling.** When an auditor finds a sample that does not conform to the described control — a missed access review, an unapproved production change, a late-closed incident — the finding becomes an **exception**. Exceptions do not automatically produce a qualified opinion; the auditor evaluates severity, pervasiveness, and management response. The GC manages the exception-wording negotiation: what the control description says, what the exception description says, what the management response says. Each phrase matters at buyer-review time.

**Management representation.** At report issuance the CEO and CISO sign a management-representation letter attesting to the completeness and accuracy of the disclosed information, the absence of undisclosed deficiencies, and the completeness of the description. The letter is a personal attestation; governance should treat its preparation with the same seriousness as a 10-Q officer certification.

### Internal-audit and governance-committee reporting cadence

The SOC 2 audit-readiness programme feeds a quarterly privacy-and-security report into the audit committee. The committee machinery itself — composition, charter, Caremark posture, documentation — is owned in [mod-111 chapter 04](../mod-111-corporate-governance-board-operations-and-officer-duties/04-audit-committee-and-financial-reporting.md). This chapter wires the cadence and the content.

The quarterly report's named contents:

- **Open findings list.** Open gap-assessment findings and open auditor-raised exceptions, with owner, age, and expected close date.
- **In-period incidents.** Security incidents in the quarter, scoped to the SOC 2 system boundary, with Incident Response outcomes and any auditor-reportable implications.
- **Audit progress.** Where the engagement sits against the timeline above; readiness-assessment closeout, observation-window status, fieldwork schedule, draft-report milestones.
- **Auditor change-of-personnel.** Any change in the engagement partner, senior manager, or lead associate; continuity is a governance signal.
- **Next-tier posture decisions.** ISO 27001, ISO 27701, HITRUST, FedRAMP posture decisions pending committee direction.

The report is delivered by the CISO and GC jointly; the audit-committee chair owns the committee-level follow-up. The cadence is quarterly in steady state, monthly during a Type I or Type II fieldwork window.

Two sub-artefacts travel with the report. The **management-representation letter** draft is pre-circulated to the audit committee for information, not approval — the committee sees the attestations the CEO and CISO will sign and can flag concerns before signature. The **minutes** record the committee's receipt of the report, the acknowledgement of the open-findings list, and any direction given to management on remediation pace. The minutes are the Caremark-trail artefact the board relies on under [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/); they are also a document the SOC 2 auditor may sample at fieldwork to confirm management oversight is operating.

### Compliance-automation-platform selection — Vanta, Drata, Secureframe, Thoropass, Anecdotes

The compliance-automation platform is operating infrastructure. It integrates with the corporation's identity provider, cloud provider, HRIS, code repository, endpoint fleet, and monitoring stack; it pulls evidence continuously; it maps evidence to control objectives across SOC 2, ISO 27001, HIPAA, PCI, GDPR, and NIST CSF; and it flags evidence-expiry so a missed quarterly access review surfaces before the auditor samples it.

The market includes Vanta, Drata, Secureframe, Thoropass, and Anecdotes (and others). Specific feature-parity and pricing claims between platforms are not stated here; <!-- needs-research: confirm current feature parity, integration coverage, auditor-network partnerships, and pricing before quoting any specific vendor claim. --> The governance selection dimensions:

- **Integration coverage.** AWS, GCP, Azure; GitHub, GitLab, Bitbucket; Okta, Azure AD, Google Workspace, JumpCloud; Jira, Linear; Slack; HRIS (Rippling, Gusto, BambooHR, Workday); EDR (CrowdStrike, SentinelOne, Microsoft Defender); MDM (Kandji, Jamf, Intune); cloud-WAF; vulnerability scanner. The integration-coverage question is which of the corporation's existing tools the platform reads natively, and which require manual evidence upload.
- **Auditor-network partnerships.** Which auditors the platform has formal partnerships with — a partnership reduces the evidence-handoff friction during fieldwork.
- **Control-library depth.** How many frameworks the platform supports natively — SOC 2 is table stakes; ISO 27001, HIPAA, PCI DSS, GDPR, NIST CSF, FedRAMP, HITRUST, TX-RAMP, StateRAMP coverage matters for multi-framework posture.
- **Continuous monitoring with evidence-expiry alerts.** The platform must alert the control owner that a quarterly access review is overdue before the evidence window closes. Without expiry alerting the automation is a document store, not a monitoring platform.
- **Pricing and the per-employee pricing trap.** Several platforms price per employee (or per monitored user), which scales linearly with headcount. A Series-B headcount of 120 becomes a Series-D headcount of 600, and the per-employee line is the second-largest compliance-stack cost after the audit fees. Governance should test renewal pricing at projected headcount, not current headcount, and negotiate caps at contract signature.
- **Trust-portal / customer-facing report distribution.** Platforms expose a buyer-facing portal that distributes the SOC 2 report under NDA. The portal is a sales-enablement capability as much as a compliance capability.
- **Policy-management and workforce-training coverage.** Several platforms bundle a policy library with version-controlled policy approvals and a workforce-training module (annual security-awareness training, role-based training, phishing simulation). The bundled modules reduce point-tool sprawl but can be weaker than best-of-breed alternatives; test the training-content quality before relying on it for SOC 2 CC1.4 evidence.
- **Exit and data-portability posture.** The automation platform holds years of evidence, policy history, and control-owner attestations. At renewal or switchover the exit path matters — what the platform exports, in what format, with what retention guarantees. Treat the automation platform like any critical SaaS vendor under the data-portability and vendor-exit discipline in [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/).

The platform decision is sticky. Once the corporation has 18–24 months of evidence history in a chosen platform, migrating to another platform means replaying evidence collection from the integration point and losing the historical audit trail. Governance treats the year-one platform decision as a 3–5 year commitment and negotiates the contract on that horizon.

### Boundary with security-engineering — this chapter owns the programme, not the controls

The governance side selects the controls framework. The security-engineering side designs and operates the controls. The explicit hand-off:

- **This chapter owns:** report-type decision, TSC scope, auditor selection, audit timeline, audit-committee reporting cadence, automation-platform selection, next-tier posture, trust-portal distribution, management-representation letters, exception-wording negotiation, bridge-letter management.
- **The `security-learning` / `ai-infra-security-solutions` curriculum owns:** identity and access management design; privileged-access workstation design; network segmentation and zero-trust architecture; logging, SIEM, and detection engineering; vulnerability management programme; secure-SDLC and code-review discipline; endpoint hardening and MDM policy; incident-response technical playbooks; cryptographic standards and key management; cloud-posture management.

The two sides meet at the control-objective level. Governance declares that the SOC 2 scope includes CC6.1 logical access; security-engineering designs the identity provider, the MFA posture, the privileged-access workstation set, the access-review mechanics, and the deprovisioning automation that satisfy CC6.1. The governance side approves the control description; the security-engineering side builds the control. The automation platform collects the evidence.

Treat the hand-off as a two-column RACI in the audit-readiness runbook. Any ambiguity about which side owns a given control objective becomes an auditor finding at fieldwork.

The adjacent-curriculum boundary cuts the other way as well. The **customer-contract security addendum** that wraps the SOC 2 attestation into an enforceable commitment is authored in [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/); this chapter does not re-draft contract language. The **cyber-insurance coverage** that funds breach response when a SOC 2 control fails is authored in [mod-112 chapter 03](../mod-112-enterprise-risk-insurance-and-compliance/03-cyber-insurance-and-incident-response-coordination.md); the underwriting application pulls directly from the SOC 2 control environment and the automation platform. The **board-level Caremark posture** that anchors officer duty-of-care on the compliance system is authored in [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/); this chapter feeds the posture with audit-committee reporting but does not define the duty standard. The **AI-safety technical** substance that overlays the SOC 2 control environment for AI/ML systems is authored in the `chief-ai-officer-learning` and `head-of-ai-governance-learning` curricula.

### Next-tier posture — ISO 27001, ISO 27701, HITRUST, FedRAMP

SOC 2 is the first frame, not the last. The next-tier posture decisions sit on the governance roadmap:

- **ISO 27001:2022.** The international-standard information-security management system. The 2022 revision reorganised Annex A to 93 controls across four themes (organisational, people, physical, technological). Fortune-500 buyers with international operations and EU-headquartered enterprises frequently prefer ISO 27001 to, or alongside, SOC 2. Dual SOC 2 + ISO 27001 reports from a single auditor is the efficient path.
- **ISO 27701.** The privacy-information-management-system extension to ISO 27001 — a certification path for the privacy posture that pairs naturally with ISO 27001 and frequently substitutes for the SOC 2 Privacy TSC at lower audit-scope cost.
- **HITRUST CSF.** The healthcare-sector common-security-framework certification. HITRUST uses a **certified-assessor** model — only a HITRUST-authorised external assessor can issue the certification — and the engagement is materially heavier than SOC 2. Required by many healthcare buyers at renewal; sometimes contractual at signature.
- **FedRAMP Moderate / High.** The US federal authorisation pathway for cloud services selling to federal agencies. FedRAMP is a multi-year programme with 3PAO engagement, sponsor-agency requirements, and continuous-monitoring obligations. The FedRAMP programme is undergoing significant reform — <!-- needs-research: confirm current FedRAMP programme changes, including the FedRAMP 20x pilot and any revisions to the Moderate/High baselines or JAB / agency authorisation pathways, before treating any specific pathway as canonical. -->
- **StateRAMP, TX-RAMP, and sector adjacencies.** State-government-sector analogues to FedRAMP, with varying reciprocity. Governance tracks which state contracts are in pipeline before committing to a specific state-RAMP pathway.
- **PCI DSS.** Payment-card industry standard, scoped in when the corporation touches cardholder data; the SAQ versus full-ROC decision is a scope-reduction exercise, not a standards choice.

The next-tier posture is a sales-pipeline question first — which buyers the corporation wants to sell to, which attestations unlock those buyers — and a compliance-engineering question second.

## Concrete example — Northbeam Analytics, Series B, 110 headcount

Northbeam Analytics is a fictional Series-B SaaS supplying marketing-attribution analytics to retail and financial-services enterprises. ARR $14M, 110 headcount, AWS-only infrastructure, Okta identity, GitHub source control, Datadog monitoring, Rippling HRIS, CrowdStrike EDR, Kandji MDM. The sales team is five enterprise reps; the pipeline includes two Fortune-500 retail accounts and one Fortune-500 US bank.

**Scope decision.** The GC, CISO, and audit-committee chair meet. The Fortune-500 bank procurement questionnaire asks for SOC 2 Type II; the retail buyers accept Type I as a bridge. The decision is **Type I in month 9, Type II with a 12-month observation window issued in month 21**. TSC scope is **Security + Availability + Confidentiality**. Privacy TSC is deferred; GDPR / CCPA operational compliance runs separately under [chapter 01](./01-gdpr-compliance-programme.md). Processing Integrity is out of scope — Northbeam does not operate as a system of record for regulated transactions.

**Auditor shortlist.** The GC runs a three-firm shortlist: Schellman (SOC-specialist), A-LIGN (SOC-specialist), and BDO (Big 4-adjacent). Big 4 is ruled out as cycle-incompatible at Series-B scale. The bank's infosec team confirms it recognises all three signatures. Schellman and A-LIGN both support dual SOC 2 + ISO 27001 issuance; BDO offers broader audit services if Northbeam's parent corporation later consolidates financial-statement audit work. The shortlist runs a 45-minute interview each; Schellman is selected based on partner continuity, Vanta partnership, and the engagement-letter wording.

**Automation platform.** Northbeam already uses Vanta for engineering onboarding; the GC confirms Vanta's integration coverage for Okta, AWS, GitHub, Datadog, Rippling, CrowdStrike, and Kandji; the contract is renegotiated with a headcount-cap clause on per-employee pricing and a trust-portal entitlement for buyer-facing distribution. Alternatives (Drata, Secureframe, Thoropass) are evaluated and declined on continuity grounds; <!-- needs-research: confirm current Vanta integration coverage and pricing structure before any live platform-selection decision. -->

**Timeline.**

- Month 0: scope and auditor signed.
- Months 1–3: Vanta rollout, gap assessment by Schellman, remediation backlog built; security-engineering runs the remediation sprint against the `ai-infra-security-solutions` control-design playbook.
- Month 4: observation window for Type I control-design-as-of-date begins; remediation close-out.
- Month 7: Type I fieldwork.
- Month 9: Type I report issued. Retail Fortune-500 deals close against the Type I.
- Month 9: 12-month Type II observation window begins. Audit committee receives the first monthly audit-status report.
- Month 21: Type II fieldwork closes; Type II report issued. Bank Fortune-500 renewal signed against the Type II.

**Governance reporting.** Audit committee receives quarterly status in steady state and monthly status during fieldwork windows. Quarterly report content follows the named-content list above. The CISO and GC co-present; the audit-committee chair owns escalation of any auditor finding that bears on Caremark posture, which is wired to [mod-111 chapter 04](../mod-111-corporate-governance-board-operations-and-officer-duties/04-audit-committee-and-financial-reporting.md).

**Next tier.** At month 18, the board approves a 12-month ISO 27001 posture decision, scoped for issuance alongside the year-two Type II renewal. HITRUST is deferred until the healthcare pipeline materialises; FedRAMP is not on roadmap.

**Boundary observed.** Northbeam's security-engineering lead runs the CC6, CC7, CC8 control design against the `ai-infra-security-solutions` playbooks — Okta posture hardening, AWS IAM boundary policies, GitHub branch-protection and signed commits, Datadog detection rules, CrowdStrike policy baseline, Kandji configuration profiles. The GC does not instruct the security-engineering lead on how to design MFA; the security-engineering lead does not instruct the GC on how to word the management-representation letter. The automation platform is where the two tracks meet.

**What governance measures.** At quarter-end the audit committee sees: five open findings (three from readiness assessment, two from in-period discovery), zero in-period reportable incidents, Type II observation at month 6 of 12, no auditor-personnel change, ISO 27001 posture decision pending month 18. No exceptions for samples pulled to date; two sample-period tickets open with remediation deadlines.

## Summary

- SOC 2 is an AICPA attestation engagement under AT-C 105 / AT-C 205, signed by a licensed CPA firm; Type I attests to control design at a point in time, Type II attests to design and operating effectiveness over a 3–12 month observation window, with 12 months the diligence default at large enterprise buyers.
- The practitioner default is 6–12 months from decision to Type I, plus a further 12 months to Type II; the bridge-letter mechanism covers the gap between consecutive Type II reports but is not a substitute for the report itself.
- The Trust Services Criteria 2017 (as revised) scope the engagement; Security is always included, and Availability, Confidentiality, Processing Integrity, and Privacy are added by customer-driven need — adding the Privacy TSC pulls material consent, retention, and deletion work into audit scope.
- The audit-firm market segments into Big 4 (Deloitte, PwC, EY, KPMG), Big 4-adjacent (BDO, Grant Thornton, RSM), and boutique / SOC-specialist (A-LIGN, Schellman, Prescient Assurance, Coalfire, Insight Assurance); selection is driven by customer recognition, review intensity, dual-report capability, auditor-network partnerships, and personnel continuity.
- The audit-readiness timeline runs through scope selection, readiness assessment, remediation sprint, observation-window opening, sample-period evidence collection, auditor fieldwork, and report issuance; the governance side owns the timeline itself and the auditor relationship.
- Audit-committee reporting is quarterly in steady state and monthly during fieldwork; the named contents are open-findings list, in-period incidents, audit progress, auditor change-of-personnel, and next-tier posture decisions. The committee machinery lives in [mod-111 chapter 04](../mod-111-corporate-governance-board-operations-and-officer-duties/04-audit-committee-and-financial-reporting.md).
- Compliance-automation platforms (Vanta, Drata, Secureframe, Thoropass, Anecdotes) are selected on integration coverage, auditor-network partnerships, control-library depth, continuous monitoring with evidence-expiry alerts, and pricing — negotiate per-employee pricing with a headcount cap at signature.
- The hand-off to security-engineering is explicit: the governance side owns report-type, scope, auditor, timeline, committee reporting, platform, and distribution; the `security-learning` and `ai-infra-security-solutions` curricula own the identity, access, network, logging, vulnerability management, and SDLC controls that live under each control objective.
- The two sides meet at the control-objective level via a two-column RACI; ambiguity about ownership becomes an auditor finding at fieldwork, so the RACI is published and acknowledged before the readiness assessment runs.
- The SOC 3 report is a general-use marketing summary derived from the Type II and is not a substitute for the restricted-use Type II in a buyer's procurement review.
- Next-tier posture decisions — ISO 27001:2022 and ISO 27701 for international and privacy posture, HITRUST CSF for healthcare buyers, FedRAMP Moderate / High for federal sales — are sequenced from the enterprise pipeline, with dual-report issuance from a single auditor the efficient path for SOC 2 + ISO 27001.
- Treat the SOC 2 report as sales-enablement infrastructure: a Type I in month 9 unblocks procurement that would otherwise freeze to month 21; the readiness-statement bridge works for weeks, not quarters; the trust-portal distribution is as much a sales capability as a compliance capability.
- Auditor fieldwork turns on sampling, exception handling, and management representation; the GC owns exception-wording negotiation and the management-representation letter is a personal attestation by the CEO and CISO that deserves the same seriousness as a financial-statement officer certification.
- The automation-platform decision is sticky at 3–5 years; evidence history does not migrate cleanly, so year-one platform selection locks in a 3–5 year commitment and governance negotiates the contract accordingly.
- Adjacent chapters carry adjacent substance: [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/) owns the security addendum, [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/) owns the Caremark posture and audit-committee machinery, [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) owns the cyber-insurance overlay, and the `security-learning` and `ai-infra-security-solutions` curricula own the engineering of the controls behind every CC-series criterion this chapter has named.
