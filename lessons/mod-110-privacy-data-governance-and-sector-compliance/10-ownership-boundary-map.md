# 10. The ownership-boundary map — what mod-110 owns end-to-end and what it hands off

> The privacy / data-governance / sector-compliance desk sits at the intersection of law, product, security, and the board. This chapter is the reference map that decides — for any privacy, data-governance, or sector-compliance question — whether it belongs to mod-110, to a sibling module, or to a non-role curriculum track.

## Motivation

By the close of mod-110 the corporation has nine substantive artefacts standing — a GDPR programme, a CCPA / CPRA programme, a rolling US state-privacy registration, a HIPAA / HITECH programme for the healthtech surface, a SOC 2 audit-readiness programme, a records-retention schedule, an incident-response and breach-notification playbook, a vendor-privacy-risk programme, and an AI-vendor / AI-model-provider governance regime. Every one of those artefacts has a seam with something else: with the commercial contract that carries the DPA into the customer relationship, with the board committee that signs off on quarterly privacy metrics, with the cyber-insurance tower that funds the breach response, with the security-engineering stack that makes the SOC 2 Common Criteria actually true, and with the AI-safety evaluation suite that sits behind the AI-vendor diligence questionnaire. If mod-110 is unclear about which side of each seam it owns, the privacy function either overreaches into insurance underwriting, board-reporting cadence, and model-risk engineering it cannot credibly deliver, or under-reaches and lets substantive regulatory analysis get rewritten by a vendor-contract redline, an insurance broker's threat-landscape slide, or a model-safety reviewer's opinion.

The problem is structural. Privacy and data governance is the youngest of the mature compliance disciplines, and in most startups it is the discipline most prone to being absorbed by whichever adjacent function is louder — legal, security, or the audit committee. The map in this chapter is the tie-breaker. It states what mod-110 owns end-to-end, what mod-110 hands off to a specific sibling module, and what mod-110 defers to a non-role curriculum track. It is written to be quoted back at the person who wants to route work incorrectly. When a sales director insists that "the DPA auto-renew is obviously a privacy question, so it lives with the DPO," this chapter is the citation that returns it to mod-109. When an auditor insists that "the firewall rule is obviously a SOC 2 question, so the compliance team owns it," this chapter is the citation that returns it to security-learning. When the CFO insists that "the cyber tower limit is obviously a privacy exposure, so it lives with the DPO," this chapter is the citation that returns it to mod-112.

The map is also an authority-conserving tool. mod-110 has a finite number of hours and a non-renewable supply of auditor- and regulator-grade attention. Every hour the DPO spends redlining an insurance policy exclusion, debating a WAF rule, or writing an agentic-safety evaluation is an hour not spent on the Article 30 record, the quarterly purge, or the next breach-notification tabletop — all of which are irreducibly mod-110's. Keeping to the boundary is not organisational pedantry; it is how the privacy programme stays defensible at the moment it is tested.

## Core concepts

### What mod-110 owns end-to-end

The nine substantive chapters of mod-110 own the following, end-to-end:

- **GDPR / UK GDPR regulatory substance** — [chapter 01](./01-gdpr-compliance-programme.md). Article 6 lawful-basis analysis, Article 9 special-category handling, Article 28 processor obligations, Article 30 record of processing, Articles 12–22 data-subject rights, Articles 33–34 breach notification, Articles 44–50 cross-border transfer, Article 35 DPIA methodology, and the Schrems II transfer-impact-assessment regime.

- **CCPA / CPRA compliance programme** — [chapter 02](./02-ccpa-cpra-compliance-programme.md). The California-resident consumer-rights operation, the "sale" and "share" analysis, the sensitive-personal-information category, the Global Privacy Control signal, and the CPPA regulator posture.

- **US state-privacy rolling-registration-plus-common-baseline programme** — [chapter 03](./03-us-state-privacy-landscape-and-rolling-registration.md). The common-baseline framework that absorbs Virginia, Colorado, Connecticut, Utah, Texas, Oregon, and every state that passes a Washington-privacy-act-flavoured statute next quarter, plus the Illinois BIPA, the Washington My Health My Data Act, and sector-specific outliers.

- **HIPAA / HITECH healthtech programme** — [chapter 04](./04-hipaa-compliance-for-healthtech.md). The Covered-Entity-versus-Business-Associate determination, the BAA substance, the HIPAA Privacy Rule, the HIPAA Breach Notification Rule 60-day / 500-record thresholds, and the HITECH enforcement posture.

- **SOC 2 audit-readiness programme (governance side)** — [chapter 05](./05-soc-2-audit-readiness-programme.md). The Trust Services Criteria scoping, the Type I-to-Type II graduation, the auditor-selection decision, the control-owner map, the quarterly evidence cadence, and the governance-level readiness that stands up on audit.

- **Records-retention schedule** — [chapter 06](./06-records-retention-schedule.md). The retention matrix by data class, the purge calendar, the legal-hold overlay, and the records-destruction evidence.

- **Incident-response and breach-notification playbook** — [chapter 07](./07-incident-response-and-breach-notification-playbook.md). The severity-triage rubric, the regulator-notification clock mechanics (72 hours for GDPR, state-by-state for the US, 60 days for HIPAA), the controller-to-processor notification ladder, and the forensic-and-counsel mobilisation.

- **Vendor-privacy-risk programme** — [chapter 08](./08-vendor-privacy-risk-programme.md). The privacy-tier framework for vendors, the DPIA / TIA requirement by tier, the sub-processor-approval workflow, the vendor privacy-questionnaire, and the ongoing-monitoring cadence.

- **AI-vendor / AI-model-provider governance regime** — [chapter 09](./09-ai-vendor-and-model-provider-governance.md). The substantive privacy posture against foundation-model providers — no-training clauses, retention posture, zero-data-retention / enterprise-tenancy analysis, prompt / completion data-flow mapping, secondary-use prohibitions, model-provider sub-processor mapping, and the substantive questions the vendor has to answer before it is approved.

**Named routing rule.** If a privacy / data-governance / sector-compliance question is substantive — what does the law require, what does the regulator expect, what evidence stands up on audit — this module answers. Full stop. The question of which commercial vehicle carries the answer, which board committee ratifies it, which insurance policy funds it, or which engineering control implements it lives elsewhere.

### Hand-offs to sibling modules

The pattern to keep in mind: mod-110 owns the *privacy / data-governance / sector-compliance / SOC 2 governance layer*; sibling modules own the *corporate, employment, equity, internal-policy, commercial-contract, board-reporting, insurance, international, or procurement layer* adjacent to it.

- **[mod-101](../mod-101-legal-entity-formation-and-corporate-structure/)** — the Delaware C-corp substrate the privacy posture operates from; officer authority to make data-processing commitments on behalf of the corporation; board resolutions approving material privacy-policy changes, HIPAA Covered-Entity status elections, or cross-border transfer architectures.

- **[mod-103](../mod-103-employment-law-and-contract-design/)** — the PIIA, the DTSA whistleblower notice, and the employment-contract substrate the employee-data processing posture sits on. mod-110 maps the employee data class and the lawful basis for processing it; mod-103 owns the contract terms that make the processing lawful in the employment relationship.

- **[mod-104](../mod-104-hiring-onboarding-and-hr-operations/)** — the HRIS / PEO stack as the single largest employee-data processor in the corporation. mod-110 writes the data-inventory entry and the vendor-DPA substance; mod-104 owns the operational configuration of the HRIS and the day-to-day hiring-loop mechanics that feed data into it.

- **[mod-105](../mod-105-equity-compensation-policy-and-comp-committee/)** — equity-record retention via the cap table and the 409A files. The retention schedule in [chapter 06](./06-records-retention-schedule.md) covers equity records at a high level; mod-105 owns the substantive equity-record keeping and the 409A documentation.

- **[mod-108](../mod-108-culture-employee-experience-and-dei/)** — the internal AI acceptable-use policy and the employee data-class matrix. mod-110 maps the privacy consequences of the matrix (which data classes can go to which tool, under what lawful basis); mod-108 owns the internal-behaviour policy that governs how employees actually use AI tools.

- **[mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/)** — the DPA, the AI-DPA, the vendor contract, and the Security Addendum as *contract instruments*. mod-110 owns the regulatory substance that determines what must be in each instrument; mod-109 owns the structural anatomy of the document itself, the fallback-position matrix, and the deal-desk routing.

- **[mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/)** — board reporting, the audit committee, the AI-risk sub-committee, and the Caremark compliance-system architecture. mod-110 [chapter 05](./05-soc-2-audit-readiness-programme.md) sets the cadence and composition of the privacy / compliance board report; mod-111 owns the committee process that receives it.

- **[mod-112](../mod-112-enterprise-risk-insurance-and-compliance/)** — the cyber-insurance tower, the incident-response coordination with carrier and broker counsel, and the FCPA / sanctions / export-controls programme. mod-110 [chapter 07](./07-incident-response-and-breach-notification-playbook.md) runs the incident; mod-112 owns the insurance side of the response and the risk-transfer architecture that funds it.

- **[mod-113](../mod-113-international-expansion-and-global-workforce/)** — international privacy regimes beyond GDPR: UK GDPR operational specifics, Switzerland revFADP, Canada PIPEDA and Quebec Law 25, Brazil LGPD, China PIPL, Singapore PDPA, Japan APPI, South Korea PIPA, India DPDP, and the Australian Privacy Act. mod-110 [chapter 01](./01-gdpr-compliance-programme.md) owns the EU / UK GDPR core; mod-113 owns the rest-of-world overlay.

- **[mod-114](../mod-114-operations-function-design/)** — procurement and systems-selection for OneTrust / Vanta / Drata / Transcend-class tooling. mod-110 specifies the capability requirements; mod-114 owns the vendor-selection cadence and the operational rollout.

### Hand-offs to non-role curriculum tracks

Some questions look like privacy or compliance questions but are in fact security-engineering or AI-safety-technical questions that belong to a different curriculum track. mod-110 does not attempt them.

- **`security-learning` / `ai-infra-security-solutions`** — the security-engineering controls behind the SOC 2 Common Criteria, the HIPAA Security Rule, ISO 27001 Annex A, and NIST SP 800-53. mod-110 [chapter 05](./05-soc-2-audit-readiness-programme.md) owns the governance side of SOC 2 — the audit cadence, the control-owner map, the auditor relationship, the board-reporting of the report. The *engineering substance* of each control — how the firewall is configured, how encryption keys are rotated, how IAM least-privilege is enforced, how the SIEM is tuned, how the vulnerability-management programme runs — is a security-learning artefact.

- **`chief-ai-officer-learning` / `head-of-ai-governance-learning` / `ai-risk-engineer-learning`** — AI-safety technical content. mod-110 [chapter 09](./09-ai-vendor-and-model-provider-governance.md) owns the privacy and data-governance posture against AI model providers. The AI-safety-technical substance — evaluation-suite design, red-teaming methodology, model interpretability, agentic-system safety, model-risk engineering, hallucination-rate measurement, prompt-injection defence — is an AI-governance-role artefact, not a privacy artefact.

- **`startup-exit-curriculum`** — privacy / compliance diligence workstreams at M&A or IPO: the privacy representations and warranties in the definitive agreement, the privacy-dedicated section of the data-room index, the regulator-inquiry disclosure schedule, and the transition-services-agreement treatment of in-flight data-subject requests. mod-110 owns the *standing* privacy programme that the diligence workstream reads from; the transaction-side diligence process itself belongs to a distinct curriculum.

### The "when in doubt" default

If the question is about what the law or regulator substantively requires, or about what evidence stands up on audit, **mod-110 answers**.

If it is about the commercial-contract vehicle that carries the answer, the board-reporting cadence that ratifies it, the insurance policy that funds it, the security-engineering control that implements it, or the AI-safety-technical substance that sits behind the AI-vendor diligence, **it belongs elsewhere**.

When two modules could plausibly own the question, apply the pattern: mod-110 owns the *regulatory substance and audit evidence*; the sibling or non-role track owns the *vehicle, cadence, funding, control, or technical substance* that surrounds it.

## Concrete example

Eleven vignettes. Each one arrives on the DPO's desk in a normal quarter. Each requires routing.

- **"The DPA auto-renew clause."** [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/) [chapter 01](../mod-109-commercial-contracts-ip-and-legal-ops/01-customer-contract-suite-msa-sla-dpa-security-aup.md) owns. Auto-renew is a commercial-contract term, not a privacy-regulatory requirement. mod-110 is consulted on whether the renewed DPA still reflects current regulatory substance; mod-109 owns the clause.

- **"The controller's lawful basis for direct marketing."** mod-110 [chapter 01](./01-gdpr-compliance-programme.md) owns. Article 6(1)(f) legitimate-interests balancing test, the PECR / ePrivacy overlay, the DPIA that evidences it. Pure regulatory substance.

- **"The SOC 2 Type II auditor selection."** mod-110 [chapter 05](./05-soc-2-audit-readiness-programme.md) owns on the governance side (which firm, what Trust Services Criteria, what report-reader audience); `security-learning` owns on the control-engineering side (does the environment actually meet the Common Criteria at an engineering level, and what remediation is needed before fieldwork).

- **"The application firewall rule for a web-app vulnerability."** `security-learning` owns. mod-110 cares that a WAF exists as a CC6.6 control; the specific rule is an engineering artefact.

- **"The eval suite for a RAG-based customer-support agent."** `chief-ai-officer-learning` / `head-of-ai-governance-learning` own. mod-110 cares that evaluations exist and that their results feed the AI-vendor file; it does not design the suite.

- **"The board report on quarterly privacy metrics."** mod-110 [chapter 05](./05-soc-2-audit-readiness-programme.md) wires the cadence, composition, and content of the report; [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/) [chapter 04](../mod-111-corporate-governance-board-operations-and-officer-duties/04-audit-committee-and-risk-committee.md) owns the committee process that receives it.

- **"The cyber-liability policy limit and sub-limit structure."** [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) [chapter 03](../mod-112-enterprise-risk-insurance-and-compliance/03-cyber-insurance-and-technology-eo.md) owns. mod-110 provides the exposure analysis (regulated data classes, affected-record projections, notification-cost estimate) the underwriter reads; mod-112 constructs the tower.

- **"The Illinois BIPA posture for a biometric authentication feature."** mod-110 [chapter 03](./03-us-state-privacy-landscape-and-rolling-registration.md) owns. BIPA is a US state statute with a private right of action and statutory damages; the written-consent and retention-schedule mechanics sit in mod-110 end-to-end.

- **"The vendor-DPA no-training clause with the foundation-model provider."** [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/) [chapter 06](../mod-109-commercial-contracts-ip-and-legal-ops/06-ai-vendor-contracts-and-ai-dpa-pattern.md) owns the structural anatomy of the clause (walk-away position, carve-out for abuse monitoring, interaction with the enterprise-tenancy warranty); mod-110 [chapter 09](./09-ai-vendor-and-model-provider-governance.md) owns the substantive privacy posture (which data classes can be sent at all, what the no-training clause has to cover to be sufficient, what the regulator expects).

- **"The HIPAA BAA template content list for a new Covered Entity customer."** mod-110 [chapter 04](./04-hipaa-compliance-for-healthtech.md) owns the substance (which Privacy-Rule and Security-Rule provisions must flow down, which permitted uses and disclosures are in scope, the breach-notification 60-day clock); [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/) [chapter 01](../mod-109-commercial-contracts-ip-and-legal-ops/01-customer-contract-suite-msa-sla-dpa-security-aup.md) owns the document mechanics (ordering with the MSA, incorporation by reference, precedence).

- **"The international hire's deemed-export analysis."** [mod-113](../mod-113-international-expansion-and-global-workforce/) owns. Export-control treatment of technology access by a foreign-national employee is a country-overlay question, not a privacy question.

## Using this map

- When a new question arrives, look first at "what mod-110 owns end-to-end." If it maps to one of the nine chapters, mod-110 owns it end-to-end. Do not sub-contract the substantive analysis to legal, security, or the broker.

- If the question does not map cleanly, walk the hand-off list and route to the sibling module that owns the underlying corporate, employment, contractual, governance, insurance, international, or procurement layer. Keep only the regulatory-substance and audit-evidence slice in mod-110.

- If the question is engineering (firewall, IAM, encryption, SIEM), AI-safety-technical (eval, red team, interpretability, agent safety), or transactional (M&A / IPO privacy diligence), it belongs to a non-role track. Coordinate at the seam and resist the urge to redraft the answer inside mod-110.

- When two owners are plausible, apply the pattern: **mod-110 owns the regulatory substance and the audit evidence; the sibling or non-role track owns the vehicle, cadence, funding, control, or technical substance that surrounds it.**

## Summary

- mod-110 owns nine substantive artefacts end-to-end: the GDPR / UK GDPR programme, the CCPA / CPRA programme, the US state-privacy rolling registration, the HIPAA / HITECH programme, the SOC 2 governance-side audit readiness, the records-retention schedule, the incident-response and breach-notification playbook, the vendor-privacy-risk programme, and the AI-vendor / AI-model-provider governance regime.

- The named routing rule: if the question is about what the law substantively requires, what the regulator expects, or what evidence stands up on audit, mod-110 answers.

- mod-110 hands off along a consistent seam: entity and officer authority to mod-101; employee-data contract substrate to mod-103; the HRIS processor to mod-104; equity records to mod-105; the internal AI-usage policy to mod-108; the DPA / AI-DPA / Security Addendum as *documents* to mod-109; board reporting and the audit committee to mod-111; the cyber tower and insurance-side incident coordination to mod-112; international privacy regimes beyond GDPR to mod-113; procurement of OneTrust / Vanta / Drata / Transcend-class tooling to mod-114.

- mod-110 defers security-engineering control substance (SOC 2 Common Criteria engineering, HIPAA Security Rule implementation, ISO 27001 Annex A, NIST SP 800-53) to `security-learning` / `ai-infra-security-solutions`.

- mod-110 defers AI-safety-technical content (evaluation-suite design, red-teaming methodology, model interpretability, agentic-system safety, model-risk engineering) to `chief-ai-officer-learning` / `head-of-ai-governance-learning` / `ai-risk-engineer-learning`.

- mod-110 defers transaction-side privacy diligence (M&A / IPO reps and warranties, data-room index, regulator-inquiry disclosure schedules) to `startup-exit-curriculum`.

- The controlling pattern when ownership is disputed: mod-110 owns the *regulatory substance and audit evidence*; the sibling or non-role track owns the *vehicle, cadence, funding, control, or technical substance* that surrounds it.

- Three seams are frequently confused and worth stating twice: (i) the DPA-as-document is mod-109, the privacy-regulatory analysis behind it is mod-110; (ii) the cyber-insurance tower is mod-112, the exposure analysis it is underwritten against is mod-110; (iii) the SOC 2 control implementation is security-learning, the SOC 2 governance-and-readiness programme is mod-110.

- The eleven vignettes are the reference cases. When a new question arrives, find the vignette it most closely resembles and route accordingly.

- The map exists so that mod-110 stays assertive about its scope without overreaching. Privacy is the discipline most prone to being absorbed by louder adjacent functions; the map is the tool for pushing back when the residual is not actually mod-110's.
