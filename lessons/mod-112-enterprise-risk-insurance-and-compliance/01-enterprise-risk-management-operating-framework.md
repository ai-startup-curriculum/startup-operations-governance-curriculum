# 1. The enterprise-risk-management operating framework

> ERM is the integration layer above every individual risk domain. It exists so the CEO, the executive team, and the board can see, price, and prioritise risks that move on different velocities before they mature at the worst possible moment.

## Motivation

An early-stage company already runs six or seven risk programmes — security, legal, finance, HR, product safety, privacy, business continuity — but rarely has anyone whose job is to **integrate** them. Each function optimises inside its own lane; each function's top-five risk list is invisible to the others; the board sees only the loudest event that reached it last quarter. Enterprise Risk Management (ERM) is the discipline that ties the lanes together into one register, one appetite statement, one review cadence, and one board-level conversation.

The reason this matters is not audit hygiene. It is that a working ERM process is the direct answer a startup board gives to a *Marchand v. Barnhill*, 212 A.3d 805 (Del. 2019), plaintiff who alleges the board utterly failed to oversee a mission-critical risk. A board that receives a real risk report on a real cadence sits inside the *Caremark* oversight expectation; one that does not is exposed. See [mod-111 chapter 05](../mod-111-corporate-governance-board-operations-and-officer-duties/05-fiduciary-duties-of-directors.md) for the doctrinal frame.

This chapter defines the operating framework — the taxonomy, the register, the appetite statement, the quarterly executive review, and the annual board review — that the incoming COO, CCO, or GC will stand up. Every other chapter in mod-112 is a specific risk domain that flows into this framework.

## The risk taxonomy

Adopt a fixed, small taxonomy. Nine to eleven categories is the right size — enough to force integration without collapsing everything into "operational". The reference categories:

- **Strategic.** Risks to the business model and thesis — a competitor releases a foundation model that commoditises your differentiator, a regulator bans your primary use case, a hyperscaler bundles your feature. Owner: **CEO**, with the executive team.
- **Operational.** Risks to the ability to run the company day-to-day — a key vendor outage, a critical single-point-of-failure engineer resignation, a supply-chain disruption for a hardware component. Owner: **COO** (or Head of Operations).
- **Financial.** Risks to the balance sheet and cash — runway compression, FX exposure on international payroll, treasury counterparty risk, revenue-concentration risk. Owner: **CFO**.
- **Compliance and regulatory.** Risks of law, rule, or licence violation — privacy law (GDPR / CCPA — see [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/)), sanctions and export controls (see [chapter 04](./04-sanctions-and-export-controls-compliance-programme.md)), anti-corruption (see [chapter 05](./05-fcpa-and-anti-corruption-programme.md)), employment law (see [mod-103](../mod-103-employment-law-and-contract-design/)), OSHA (see [chapter 06](./06-osha-and-workplace-safety-programme.md)). Owner: **GC / Chief Compliance Officer**.
- **Reputational.** Risks to trust with customers, employees, investors, and the public — a public safety incident, a founder-conduct issue, a product-misuse story, a data-breach headline. Owner: the executive team collectively, with a **Head of Communications** lead.
- **Cybersecurity.** Risks to confidentiality, integrity, and availability of information systems — intrusion, ransomware, insider misuse, funds-transfer fraud. Owner: **CISO** (or Head of Security). Note that cyber flows through both compliance (privacy-law notification obligations — [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/)) and insurance/incident-response ([chapter 03](./03-cyber-insurance-and-incident-response-coordination.md)).
- **AI / model risk.** Risks from AI-model behaviour — safety failures, harmful outputs, bias / disparate impact, hallucinated outputs in high-stakes decisions, model drift, prompt-injection, jailbreaks, training-data provenance. Owner: **Head of AI Safety / Head of AI Governance / Chief AI Officer** — role name varies; substance sits in the `head-of-ai-governance-learning` curriculum.
- **Geopolitical.** Risks from state action — sanctions expansions, export-control tightening, tariff regimes, data-localisation mandates, forced-technology-transfer pressure, war and civil unrest in a customer or supplier geography. Owner: **executive team collectively**, with GC or Head of International as lead.
- **People and culture.** Risks to the ability to attract, retain, and develop the workforce — key-person concentration, employment-law liability, harassment / discrimination allegations, unionisation pressure, workforce burnout. Owner: **Chief People Officer / VP People**.
- **Product / safety and physical risk.** Product liability, workplace-safety incidents (see [chapter 06](./06-osha-and-workplace-safety-programme.md)), hardware-defect exposure. Owner varies by company; commonly **Head of Product** or **VP Engineering** with the safety officer.

The exact list is less important than fixing it. Every risk in the register must map to exactly one category — dual-category risks force ambiguity in ownership.

## The risk register

The risk register is the artifact. It is a single spreadsheet or GRC-tool table with a fixed schema and a single tool of record. If a risk lives in someone's private notes or a Slack channel, it is not in the register.

Minimum schema per row:

- **ID.** Stable identifier (e.g., `R-2026-014`) that persists across reviews.
- **Statement.** One sentence, actor-verb-object form: "A ransomware attack encrypts the production Postgres cluster and demands payment." Not "Cyber risk."
- **Category.** From the taxonomy above.
- **Owner.** A named individual (role plus person), not a function.
- **Inherent likelihood.** 1–5 or Low/Medium/High/Very High — pick one scale and use it consistently. Assessed **before** existing controls.
- **Inherent impact.** Same scale, assessed **before** existing controls.
- **Controls.** The controls currently in place. Terse. Reference the control library.
- **Residual likelihood.** After controls.
- **Residual impact.** After controls.
- **Trend.** ↑ / → / ↓ vs. last review.
- **Review cadence.** Quarterly (default) or more frequent for top-N and mission-critical risks.
- **Last reviewed.** Date.
- **Notes / open actions.** Any control gap under remediation with an owner and a due date.

Keep the register in a single tool. Airtable, Notion, Google Sheets, or a purpose-built GRC platform (LogicGate, Onspring, AuditBoard, Hyperproof, Drata's risk module) all work — the platform matters less than the discipline that no one has an off-platform copy.

**The anti-pattern**: a register that is only touched the week before the quarterly review, in which the previous quarter's rows are unchanged and the executive team is doing risk assessment from cold memory in a two-hour meeting. A living register is refreshed continuously as new information arrives, and the quarterly review is a checkpoint on a running artifact, not a from-scratch assessment.

## Risk appetite and risk tolerance

Two distinct concepts that are commonly conflated:

- **Risk appetite** is the **amount and type of risk the organisation is willing to accept in pursuit of its strategy**. It is set by the **board** on management's recommendation, and it is deliberately qualitative-plus-limited-quantitative — not a stochastic bank capital limit.
- **Risk tolerance** is the **acceptable variation around a specific objective or metric**. It operationalises appetite at the metric level — "cash runway must remain above 18 months at all times" or "no single customer contract may exceed 15 % of ARR."

For a startup, the appetite statement is a short document — one to three pages. A serviceable structure:

1. **Overall risk posture.** "We are a growth-stage company; we accept meaningful strategic and product-execution risk to pursue category leadership, and we hold conservative appetite for compliance, safety, and financial-control risk that would compromise our ability to operate or fund."
2. **Category-by-category appetite.** For each risk taxonomy category, a one-paragraph statement of how much risk the company will accept. Strategic → high; compliance → low; safety → very low; cyber → low; financial → low outside runway trade-offs; AI → context-dependent, low for high-stakes deployments.
3. **Bright-line prohibitions.** Things the company will **never** do regardless of upside — knowingly violate law, ship a model that fails safety evaluation, sign a customer contract that indemnifies for unbounded consequential damages, accept payment from an OFAC-blocked party. These are the risk-tolerance zero-tolerance rules.
4. **Quantitative anchors where possible.** Runway floor, single-customer-concentration ceiling, cyber-incident severity thresholds requiring board notification, maximum uninsured retention on any single insurance line. Keep it to five or six numbers; more is theatre.

The board **adopts** the appetite statement on management's recommendation, and the audit committee **re-affirms** it annually. Documenting the adoption in the minutes is what makes it available as a legal defence later.

## The quarterly executive risk review

Cadence: quarterly. Duration: 60 to 90 minutes. Attendees: the executive team (CEO, COO, CFO, CTO, GC/CCO, CISO, Chief People Officer, Head of AI Governance if the role exists). The GC or CCO **facilitates** and the register owner drives the material.

A serviceable 60-minute agenda:

- **(5 min) Prior-quarter actions closed** — a rapid roll-up of open remediation items and their status. Anything past due is called out by name.
- **(15 min) Top-10 residual risks** — the register sorted by residual score, walked one at a time. For each: owner, current control status, trend, any changes since last review.
- **(10 min) New and escalated risks** — risks added this quarter or that moved category or severity. Where possible, tied to the event that surfaced them.
- **(10 min) Closed and retired risks** — risks that are no longer material or where residual has fallen below the tracking threshold. Retire deliberately, not by attrition.
- **(10 min) Control-effectiveness signals** — evidence that controls are actually working (or not): SOC 2 findings, security-questionnaire delta, EPLI claims, near-miss reports.
- **(10 min) Emerging-risks watchlist** — risks that are not yet on the register but should be tracked (new regulator action, market movement, geopolitical event, foundation-model release).

The output is a short minutes document — decisions taken, actions assigned with owners and dates, and any items to escalate to the board. The minutes go into the corporate record.

## The annual board / audit-committee risk review

Cadence: annual, at a scheduled audit-committee meeting; the audit committee then reports the risk conversation to the full board (see [mod-111 chapter 04](../mod-111-corporate-governance-board-operations-and-officer-duties/04-standing-committees.md) for the committee's charter role in risk oversight, and NYSE Listed Company Manual § 303A.07(b)(iii)(D) requiring the audit committee to discuss risk-assessment and risk-management policies).

Duration: 60 to 90 minutes as a discrete agenda item, plus additional time on any mission-critical risk that warrants a deep-dive.

A serviceable structure:

- **(10 min) Framework and methodology recap** — what taxonomy, what scoring, what cadence. Repeated annually because directors rotate and refreshers matter.
- **(20 min) The register, in summary form** — heat map by category; top-10 residual list; year-over-year trend.
- **(15 min) Mission-critical risks in detail** — the two or three risks that would materially threaten the company. This is the *Marchand* conversation: what is the reporting system for this risk, what is management doing about it, what does the audit committee need to see quarterly? Reference [mod-111 chapter 05](../mod-111-corporate-governance-board-operations-and-officer-duties/05-fiduciary-duties-of-directors.md) for the doctrinal setting.
- **(15 min) Appetite statement review** — re-adopt the appetite statement as-is or amended. Discuss any risks currently exceeding appetite and management's plan.
- **(10 min) Insurance and risk-transfer posture** — a summary of the insurance stack ([chapter 02](./02-startup-insurance-stack-by-stage.md)) and how it maps to residual risk. This is the moment the CFO shows the D&O programme summary alongside the register.
- **(10 min) Executive session** — the audit committee meets without management to raise questions.

The audit committee's report to the full board should be a one-page summary that any director can absorb in the pre-read pack.

## The reference frameworks

Three reference frameworks are worth knowing by name. A startup does not adopt any of them wholesale; a startup picks vocabulary and structure from them so the ERM programme is legible to auditors, insurers, and board members who came from bigger companies.

- **ISO 31000:2018 — Risk management — Guidelines.** A principles-and-process framework. Defines risk as "the effect of uncertainty on objectives" and structures the process into scope-and-context → risk assessment (identification, analysis, evaluation) → risk treatment → monitoring and review, wrapped in communication and consultation. Terse, non-prescriptive, and adaptable. Good default for a startup that wants a common vocabulary without a heavy compliance apparatus.
- **COSO Enterprise Risk Management — Integrating with Strategy and Performance (2017).** The five-component framework: (1) Governance & Culture, (2) Strategy & Objective-Setting, (3) Performance, (4) Review & Revision, (5) Information, Communication & Reporting. Twenty supporting principles. More prescriptive than ISO 31000 and more strategy-integrated; commonly the reference framework for pre-IPO and public companies because auditors and audit committees are fluent in it. Note the separate but related **COSO Internal Control — Integrated Framework (2013)** — the ICFR / SOX framework covered in [chapter 08](./08-sox-lite-to-sox-full-trajectory.md).
- **NIST SP 800-37 Rev. 2 — Risk Management Framework for Information Systems and Organizations.** Federal in origin, but the vocabulary (categorize → select → implement → assess → authorize → monitor) is widely borrowed for cybersecurity risk. Pair with **NIST Cybersecurity Framework (CSF) 2.0** (identify, protect, detect, respond, recover, plus the new "govern" function added in CSF 2.0) for the cyber-specific slice of the register.

Recommended pattern for a Series-B startup: **ISO 31000 as the enterprise-wide operating framework**, **COSO 2013 for the ICFR / SOX-lite programme** ([chapter 08](./08-sox-lite-to-sox-full-trajectory.md)), and **NIST CSF 2.0 as the cyber sub-framework** ([mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) and [chapter 03](./03-cyber-insurance-and-incident-response-coordination.md)). Migrate to **COSO ERM 2017** as the enterprise framework 12 to 18 months before the IPO decision.

## Concrete example — a Series-B AI-infrastructure startup

For orientation, a representative top-10 risk register for a Series-B AI-infrastructure company with regulated-industry customers might look like:

| ID | Statement | Category | Owner | Residual (L × I) | Trend |
|---|---|---|---|---|---|
| R-2026-001 | Foundation-model provider deprecates the primary model we serve, forcing customer migration on short notice | Strategic | CEO / CTO | 3 × 5 | ↑ |
| R-2026-002 | Production-inference cluster outage exceeds SLA; largest customer invokes contract-termination right | Operational | CTO / VP Eng | 2 × 4 | → |
| R-2026-003 | Ransomware attack encrypts production Postgres cluster and demands payment | Cybersecurity | CISO | 2 × 5 | ↑ |
| R-2026-004 | A prompt-injection exploit causes a customer-facing agent to exfiltrate other-tenant data | AI / model risk | Head of AI Safety | 3 × 4 | ↑ |
| R-2026-005 | An enterprise customer alleges HIPAA breach; regulator notification obligations trigger | Compliance | GC / CCO | 2 × 5 | → |
| R-2026-006 | An engineer working from a sanctioned jurisdiction violates OFAC absent our knowledge | Compliance / Geopolitical | GC / CCO | 1 × 5 | → |
| R-2026-007 | A key ML infra engineer (10 % of critical infra knowledge) resigns without a successor | People / Operational | CTO / VP People | 3 × 3 | → |
| R-2026-008 | Runway drops below 18 months due to slower-than-plan enterprise deal cycle | Financial | CFO | 3 × 4 | ↑ |
| R-2026-009 | A public model-misuse incident drives customer contract renegotiation | Reputational / AI | CEO / Head of Communications | 2 × 4 | → |
| R-2026-010 | Export-control tightening on advanced-compute end-users blocks a strategic customer segment | Geopolitical / Compliance | GC / CCO | 2 × 4 | ↑ |

Each row has an owner, a residual score, a trend, and — behind it in the register — a control list and any open remediation actions. The board audit committee reads this table at every annual review and drills into any risk with residual impact 5 or trend ↑.

## Summary

- **ERM is the integration layer above individual risk domains.** Its purpose is to give the executive team and the board one shared view of risk across taxonomy categories with different velocities.
- **Fix the taxonomy** — strategic / operational / financial / compliance / reputational / cybersecurity / AI / geopolitical / people / product, each with a named owner.
- **The risk register is the artifact** — one tool of record, a fixed schema, refreshed continuously, retired deliberately.
- **Risk appetite is the board's** — a short, qualitative-plus-limited-quantitative statement re-affirmed annually. Risk tolerance operationalises appetite at the metric level.
- **The quarterly executive risk review** is a 60–90-minute working meeting with agenda, owners, and minutes; the **annual audit-committee risk review** is the *Marchand* conversation with the board.
- **Pick vocabulary from ISO 31000 (enterprise), COSO 2013 (ICFR), and NIST CSF 2.0 (cyber)** — a startup does not adopt any framework wholesale but is legible to auditors and directors in these terms.
- **Documentation is the defence.** Every risk decision that materialises later — an incident, an enforcement action, a *Caremark* claim, a diligence-schedule item — will be tested against the record of what the board and management knew and when. A living register and dated minutes are that record.
