# 8. Ownership boundary map

> The people-ops function fights over ownership. This chapter is the reference map that decides — for any culture / handbook / DEI / engagement / AI-usage / internal-comms question — whether it belongs to mod-108, to a sibling module, or to a non-role track.

## Motivation

The culture / employee-experience / DEI function sits at the centre of a busy Venn diagram. Questions arrive from the CEO, the board, functional leaders, managers, employees, and outside counsel without a natural home: is a code-review-culture value a mod-108 question or a cto-curriculum question? Does a Copilot enterprise licence sit with people-ops or with security? Does the RTO policy break when the company opens a first office in Berlin?

Without an explicit ownership map, mod-108 either overreaches — writing engineering-culture, GTM-culture, and privacy policy it is not competent to write — or under-reaches, and adjacent functions write conflicting handbook clauses, redundant engagement instruments, or shadow AI-usage rules. This chapter is the operating map. It states what mod-108 owns end-to-end, what mod-108 hands off to a specific sibling module, and what mod-108 explicitly defers to a non-role curriculum track. Use it as the tie-breaker.

## What mod-108 owns

The seven substantive chapters of mod-108 own the following, end-to-end:

- **Values, behaviours, and anti-values** — the selection framework, the behaviour-anchoring rubric, and the anti-values list — [chapter 01](./01-values-behaviours-and-anti-values.md). Every values debate the CEO wants to have starts here.
- **The employee handbook** — structure, chapter list, state supplements, update cadence, and NLRB / *Stericycle* posture — [chapter 02](./02-employee-handbook-nlrb-compliant-post-stericycle.md). The handbook is a mod-108 artefact; the *clauses inside it* often are not (see hand-offs below).
- **The DEI programme** — programme design, ERG framework, pay-equity audit cadence, post-*SFFA* posture — [chapter 03](./03-dei-programme-design-post-sffa.md).
- **The engagement measurement programme** — survey cadence, instrument selection, action-planning loop, manager-effectiveness signal — [chapter 04](./04-engagement-measurement-and-action-planning.md).
- **The remote / hybrid / RTO operating policy** — corporate posture, work-from-anywhere windows, hybrid rhythm, RTO enforcement — [chapter 05](./05-remote-hybrid-rto-operating-policy.md).
- **The AI-usage / acceptable-use policy** as it lives inside the handbook — tier framework for approved tools, red-line data classes, discipline path — [chapter 06](./06-ai-usage-and-acceptable-use-policy.md).
- **The internal-communications operating rhythm** on the culture-comms side — all-hands cadence, CEO update, AMA norms, crisis-comms playbook — [chapter 07](./07-internal-communications-operating-rhythm.md).

If a question maps to one of the above, mod-108 owns it. If it maps to one of the below, mod-108 explicitly hands off.

## What mod-108 hands off

Each sibling module owns a specific slice of adjacent work. The pattern to keep in mind: mod-108 owns the *policy layer* on the people side; sibling modules own the *legal, financial, operational, or technical layer* underneath.

### mod-101 — legal entity formation and corporate structure

- The legal entity that is the employer-of-record for each employee.
- The corporate-law question of how the handbook binds the corporation (Delaware C-corp, board resolutions authorising handbook adoption, indemnification interactions).

See [mod-101](../mod-101-legal-entity-formation-and-corporate-structure/).

### mod-102 — founding team legal architecture

- The founders' PIIA / IP-assignment agreements that the handbook's IP + confidentiality chapter cross-references.
- Any legacy founder-era side letters that alter the standard employee-agreement package.

See [mod-102](../mod-102-founding-team-legal-architecture/).

### mod-103 — employment law and contract design

- The enforceability of at-will, arbitration, non-compete, and non-solicit clauses the handbook cites.
- The state-by-state legal analysis behind the handbook state supplements.
- Standard offer-letter and employee-agreement drafting.

The handbook *cites* these clauses; mod-103 owns the drafting and legal enforceability analysis. If someone asks "can we enforce this arbitration clause in California?" that is mod-103, not mod-108. See [mod-103](../mod-103-employment-law-and-contract-design/).

### mod-104 — hiring, onboarding, and HR operations

- The hiring-loop mechanics into which values-based interview questions and diverse-slate norms plug.
- The first-90-day onboarding programme into which the handbook and values training slot.
- Recruiter operations, ATS configuration, and offer-management workflow.

mod-108 owns the *norm* ("we run a diverse slate for every director-plus opening"); mod-104 owns the *loop mechanics* that implement it. See [mod-104](../mod-104-hiring-onboarding-and-hr-operations/).

### mod-105 — equity compensation policy and comp committee

- The compensation-committee governance of any comp-equity remediation that comes out of the pay-equity audit.
- The board-level pay-equity report if the company is required to file or discloses one.
- Executive-comp equity decisions that interact with any DEI-driven adjustment.

See [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/).

### mod-106 — compensation architecture and total rewards

- The compensation architecture — levels, bands, geographic-pay strategy, annual comp cycle — into which pay-equity remediation actually lands.
- The benefits programme (health, retirement, PTO, leave) that the handbook references.
- The total-rewards philosophy statement.

The audit signal in [chapter 03](./03-dei-programme-design-post-sffa.md) triggers a remediation; the merit-cycle mechanic in mod-106 delivers it. See [mod-106](../mod-106-compensation-architecture-and-total-rewards/).

### mod-107 — performance, promotion, and offboarding

- The performance / promotion / development / offboarding operating system into which engagement-survey data on manager effectiveness feeds.
- The termination playbook against which values-violation-based terminations execute.
- The PIP mechanic that manager-effectiveness signals may trigger.
- The exit-interview instrument whose culture-themed findings feed back to mod-108.

See [mod-107](../mod-107-performance-promotion-and-offboarding/).

### mod-109 — commercial contracts, IP, and legal ops

- The customer-facing AI contract terms and IP terms that reflect (but are not) the internal AI-usage policy.
- The vendor MSAs and DPAs for the AI tools the corporation uses.
- The IP-warranty and indemnity language in customer contracts that constrains what the corporation can commit to.

The internal AI-usage policy in [chapter 06](./06-ai-usage-and-acceptable-use-policy.md) and the customer-facing AI terms are related but distinct artefacts. See [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/).

### mod-110 — privacy, data governance, and sector compliance

- The privacy / DPA / sector-compliance layer that governs what employee and customer data can flow into AI tools.
- The employee-privacy-notice content that the handbook references.
- GDPR / CCPA / HIPAA / SOC 2 / sector-specific rules that constrain the acceptable-use policy.

If the question is "can this data class go into ChatGPT?" the answer flows from mod-110's data-classification scheme, not from mod-108's opinion. See [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/).

### mod-111 — corporate governance, board operations, and officer duties

- The board-communications side of confidential comms — board decks, executive session, board-observer handling.
- The officer-fiduciary-duty layer that constrains what the CEO can and cannot say in an all-hands during a live deal or investigation.

The all-hands cadence in [chapter 07](./07-internal-communications-operating-rhythm.md) is a mod-108 artefact; the board-pack cadence is a mod-111 artefact. See [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).

### mod-112 — enterprise risk, insurance, and compliance

- The SecReview / VendorReview / risk-register process that governs Tier-1 AI tool approval.
- The insurance layer (EPLI, D&O, cyber) that responds to employment-practice and AI-usage incidents.
- The compliance controls that a SOC 2 or ISO auditor will test the AI-usage policy against.

mod-108 owns *what* the acceptable-use policy says; mod-112 owns *whether the tool clears* the security bar for use. See [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/).

### mod-113 — international expansion and global workforce

- International / EOR / permanent-establishment complexity that constrains the remote-across-borders piece of the RTO policy.
- Works-council, co-determination, and reasonable-accommodation rules for the EU, UK, and other non-US jurisdictions.
- Country-specific handbook supplements and the employer-of-record versus own-entity decision.

The corporate RTO position is a mod-108 policy; the local-law overlay on any given country is a mod-113 problem. See [mod-113](../mod-113-international-expansion-and-global-workforce/).

### mod-114 — operations function design

- The operating-function cadence — weekly business review, quarterly business review, board pack — that lives alongside the culture-comms cadence.
- The staff meeting, planning cycle, and OKR mechanics.
- The programme-management office and its rituals.

Two cadences run in parallel: the culture-comms rhythm ([chapter 07](./07-internal-communications-operating-rhythm.md)) and the ops-function rhythm (mod-114). They are choreographed but not merged. See [mod-114](../mod-114-operations-function-design/).

## What mod-108 defers to non-role tracks

Some questions look like people-ops questions but are actually technical or vertical questions that belong to a different curriculum track altogether. mod-108 does not attempt them.

- **`chief-ai-officer-learning` / `head-of-ai-governance-learning` / `ai-risk-engineer-learning`** — AI-technical, model-risk, red-teaming, and evaluation content. The AI-usage policy chapter ([chapter 06](./06-ai-usage-and-acceptable-use-policy.md)) sets *employee-behaviour rules*; it explicitly does NOT cover model-risk methodology, red-team programme design, or evaluation-suite construction.
- **`startup-product-gtm-curriculum`** — GTM / sales-culture-specific engagement, quota-culture-specific values operationalisation, sales-manager coaching nuance. mod-108 owns the corporate-level values; sales-org-specific behaviour anchoring belongs to the GTM track.
- **`cto-curriculum`** — engineering-culture-specific values operationalisation (code-review culture, on-call culture, blameless post-mortem culture, tech-writing culture). mod-108 owns the corporate values; the engineering-culture operationalisation is a cto-curriculum artefact.
- **`startup-exit-curriculum`** — culture-integration during M&A, retention comms for a target-company workforce, cross-cultural integration, cultural-diligence work. mod-108 owns the standing culture programme; exit-driven culture work is a distinct curriculum.

## Boundary worked examples

Eight vignettes. Each one arrives on the head of people's desk in a normal quarter.

**1. The head of engineering wants to codify a code-review-culture value.**
Question: mod-108 or `cto-curriculum`? Answer: mod-108 owns the value-selection framework in [chapter 01](./01-values-behaviours-and-anti-values.md) — the head of engineering should propose the underlying value through that process. The specific *operationalisation* into code-review norms (PR-turnaround SLAs, review-depth expectations, blameless-review language) belongs to the `cto-curriculum` engineering-culture material. mod-108 approves the value; cto-curriculum implements it inside the engineering org.

**2. The board asked for a diversity-slate hiring norm.**
Question: mod-108 or mod-104? Answer: mod-108 owns the norm — the DEI programme in [chapter 03](./03-dei-programme-design-post-sffa.md) is where the diverse-slate requirement is written and defended post-*SFFA*. The loop-mechanics implementation — recruiter sourcing behaviour, ATS configuration, hiring-manager training — is [mod-104](../mod-104-hiring-onboarding-and-hr-operations/). mod-108 sets policy; mod-104 makes it happen in the pipeline.

**3. The CFO wants to expense a Copilot Business enterprise licence.**
Question: mod-108 or mod-112? Answer: mod-108 owns the acceptable-use policy in [chapter 06](./06-ai-usage-and-acceptable-use-policy.md) that governs how employees may use it once approved. [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) owns the security review, vendor-risk assessment, and Tier-1 approval decision that determines whether the tool clears for enterprise use in the first place. Both are required — mod-112 first, mod-108 second.

**4. The CEO wants to run a monthly financial update to the whole company.**
Question: mod-108 or mod-114? Answer: [chapter 07](./07-internal-communications-operating-rhythm.md) owns the culture-side rhythm — the all-hands slot, the format, the norms of transparency, the AMA cadence. [mod-114](../mod-114-operations-function-design/) owns the operations-function cadence — the numbers, the WBR / QBR mechanic, the board-pack alignment. The monthly financial update lives on the culture-comms cadence but pulls its content from the ops-function cadence.

**5. Manager-effectiveness scores in engineering are the worst in the company.**
Question: who acts? Answer: mod-108 owns the engagement survey and the aggregate signal — [chapter 04](./04-engagement-measurement-and-action-planning.md) is where the finding is surfaced and the org-wide action plan is set. [mod-107](../mod-107-performance-promotion-and-offboarding/) owns the individual-manager response — the performance-side coaching, the PIP path if warranted, the promotion-committee treatment. mod-108 raises the flag; mod-107 works the individual cases.

**6. The pay-equity audit found a 3% adverse gap for women in Sales.**
Question: who remediates? Answer: [chapter 03](./03-dei-programme-design-post-sffa.md) owns the audit and the remediation trigger — the audit methodology, the finding, the decision to remediate. [mod-106](../mod-106-compensation-architecture-and-total-rewards/) owns the merit-cycle mechanic that actually lands the adjustment in employee comp. For a comp-committee-visible remediation, [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/) is looped in as governance.

**7. An engineer used personal ChatGPT to summarise a customer contract.**
Question: who investigates and disciplines? Answer: mod-108 owns the policy that was violated ([chapter 06](./06-ai-usage-and-acceptable-use-policy.md)) and the discipline framework it sets out. [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) owns the incident-response side — data-classification impact, insurance-notification triggers, customer-notification analysis. [mod-107](../mod-107-performance-promotion-and-offboarding/) owns the actual disciplinary conversation, the write-up, and (if warranted) the termination path. Three modules, one incident.

**8. The company is considering opening a first EU office.**
Question: who owns the RTO policy for the EU staff? Answer: mod-108 owns the corporate RTO position in [chapter 05](./05-remote-hybrid-rto-operating-policy.md) — the hybrid rhythm, the in-office expectation, the enforcement posture. [mod-113](../mod-113-international-expansion-and-global-workforce/) owns the local-law overlay — reasonable-accommodation rules under EU law, works-council consultation obligations, the EOR-vs-entity decision, and the country-specific handbook supplement. The corporate policy applies; the local-law overlay modifies.

## Using this map

- When a new question arrives, look first at "what mod-108 owns." If it maps, mod-108 owns it end-to-end.
- If it does not map cleanly, look at "what mod-108 hands off." Find the sibling module that owns the underlying legal, financial, operational, or technical layer.
- If the question is technical / vertical / M&A / GTM in nature, look at "what mod-108 defers to non-role tracks."
- When two modules could plausibly own it, apply the pattern: mod-108 owns the *policy layer on the people side*; the sibling module owns the *substrate underneath*. The vignettes above are the reference cases.

The point of the map is not to shrink mod-108's scope. It is to keep mod-108 competent within its scope, and to keep the corporation from writing the same policy twice in two functions that disagree with each other.
