# 9. Ownership boundary map

> What this module owns, and where each adjacent question is handed off.

## Motivation

Hiring, onboarding, and HR operations sit at the middle of a dense set of adjacent modules: the employment-law layer that governs the contracts the pipeline produces; the equity-comp policy that governs how grants are set; the compensation architecture that governs bands and levels; the performance-management operation that catches the onboarding programme's baton; the international-workforce module that governs cross-border hiring; and — outside this curriculum — the sales / GTM leveling framework and the engineering IC-vs.-manager track that live in adjacent role tracks.

Boundaries in a curriculum are a service to the learner and to the operating COO / head of people / GC. When a question shows up, the boundary map tells you where the answer lives.

## What this module owns

**mod-104 owns the general hiring / onboarding / HR-operations infrastructure.** Concretely:

- **The sourcing operating model by stage** — founder-led at pre-seed / seed; first recruiter at Series-A; in-house TA + fractional overlay at Series-B; in-house TA + exec-search partnership at growth. Cost-and-signal trade-offs; referral programme design; sourcer / recruiter ratio benchmarks (see [chapter 01](./01-sourcing-operating-model-by-stage.md)).
- **The ATS layer** — selection between Ashby / Greenhouse / Lever / Workable at seed → Series-B; graduation triggers; the integration stack (HRIS / PEO, LinkedIn Recruiter + Talent Insights, interview scheduling, background-check CRAs, assessment and interview-intelligence tools); the migration playbook between ATS products (see [chapter 02](./02-ats-selection-and-integration.md)).
- **Structured interviewing** — the scorecard architecture, the interview-panel design, the interviewer-training programme, the debrief-and-consensus playbook, and the anti-affinity-bias operating norms (blind resume screens, structured questions, competency-anchored scoring) (see [chapter 03](./03-structured-interviewing.md)).
- **Reference checks and background checks** — the reference-check playbook; the FCRA-compliant background-check process (standalone disclosure, authorisation, ordering, pre-adverse-action, adverse-action); state-analogue FCRAs; ban-the-box / fair-chance-act constraints; the international overlay for background checks (see [chapter 04](./04-reference-and-background-checks.md)).
- **Form I-9 and E-Verify** — the three-day rule, the acceptable-documents list, reverification, storage and retention, audit-readiness, the DHS alternative remote-examination procedure, and the E-Verify overlay (state mandates + federal-contractor obligations) (see [chapter 05](./05-i9-and-e-verify.md)).
- **The first-90-day onboarding programme** — pre-boarding, day one, first week, 30 / 60 / 90-day cadence, buddy programme, new-hire NPS (see [chapter 06](./06-first-90-day-onboarding.md)).
- **The HRIS / PEO / payroll stack** — the bundled-vs-unbundled trade; PEO selection (Justworks, TriNet, Sequoia One) at seed; HRIS selection (Rippling, Gusto, Deel HR) at Series-A / B; HCM (Workday, Dayforce, SuccessFactors) at growth; multi-state and multi-country payroll; benefits-broker selection; the SOC 2 audit boundary (see [chapter 07](./07-hris-peo-payroll-stack.md)).
- **The executive-hiring playbook** — retained exec-search partner selection (Heidrick, Spencer Stuart, True Search, Daversa, Bolster, and the boutique layer); the one-third / one-third / one-third fee cadence; the exec interview panel; the exec offer package (cash + equity + severance + officer appointment); the executive onboarding programme (100-day plan, board-relationship, CEO partnership) (see [chapter 08](./08-executive-hiring-playbook.md)).

## What this module hands off

### To [mod-103 — Employment Law, Worker Classification & Contract Design](../mod-103-employment-law-and-contract-design/)

- **W-2 vs. 1099 worker-classification analysis** — the IRS common-law test, the FLSA economic-realities test, the California ABC test.
- **FLSA exempt vs. non-exempt classification** — the salary-basis and duties tests.
- **Offer-letter drafting and pay transparency** — the offer-letter architecture, contingent conditions, and state pay-transparency requirements.
- **PIIA and NDA drafting** — the employee-facing PIIA and the NDA / MNDA suite.
- **Non-compete and alternatives** — the state landscape and the surviving-defaults clause pack.
- **EEOC-protected-category framework** — Title VII, ADA, ADEA, PDA, EPA, GINA and the state / city protected-category layer applied across the hiring lifecycle.
- **State-law variance** — California, New York, Illinois, Washington, Colorado, and elsewhere.
- **Arbitration and class-action waivers** — the enforceability landscape post-*Epic Systems*, plus the sexual-harassment / assault carveout and California PAGA.

mod-104 produces the operating pipeline; mod-103 governs the legal architecture that the pipeline's outputs (offer letter, PIIA, arbitration agreement, handbook acknowledgment) must satisfy.

### To [mod-105 — Equity-Compensation Policy & the Compensation Committee](../mod-105-equity-compensation-policy-and-comp-committee/)

- **Grant guidelines** — grant-size bands by level and role, refresh cadence, promotion-driven refreshes.
- **Exec-hire equity packages** — the substantive equity-package design (grant size, vesting, refresh, acceleration mechanics) for VP+ hires.
- **Compensation-committee governance** — charter, independence progression, delegation to a Committee Chair, resolution templates.

mod-104 covers the exec-hire *hiring process* (search, panel, offer negotiation mechanics); mod-105 covers the exec-hire *equity-policy substance* — what grant size is right at what level, what refresh cadence, what acceleration.

### To [mod-106 — Compensation Architecture & Total Rewards](../mod-106-compensation-architecture-and-total-rewards/)

- **Compensation-band architecture** — leveling framework, compensation bands per level, geographic differentials.
- **Benchmarking methodology** — data sources (Radford, Compensia, Aon, Carta compensation), survey participation, refresh cadence.
- **Total-rewards program design** — the substantive design of the benefits program (plan design decisions, contribution strategy, executive-benefits enhancements). mod-104 covers the *selection of the benefits broker* and the *operating machinery* (open enrollment, HRIS integration); mod-106 covers *what the benefits plan should look like*.

### To [mod-107 — Performance, Promotion & Offboarding](../mod-107-performance-promotion-and-offboarding/)

- **The performance-management programme** — the review cadence, the performance-review instrument, calibration.
- **Promotion criteria** — the promotion process, the promotion-committee model, the criteria per level.
- **PIPs and involuntary termination** — the PIP process, the involuntary-termination operating procedure.
- **Reductions in force (RIFs)** — the RIF process, the notice requirements (WARN Act — federal and state analogues), the separation-agreement templates.
- **Separation-agreement authoring** — the substance of separation agreements including releases, non-disparagement, severance, benefits continuation.

The onboarding programme in [chapter 06](./06-first-90-day-onboarding.md) hands off at the 90-day mark into the corporation's ongoing performance-management operation; mod-107 owns the ongoing operation.

### To [mod-108 — Culture, Employee Experience & DEI](../mod-108-culture-employee-experience-and-dei/)

- **Culture programme design** — values operationalisation, culture rituals, all-hands cadence.
- **Employee experience** — the employee-lifecycle programme beyond onboarding; engagement measurement over time; internal-mobility programme.
- **DEI programme** — the substantive DEI strategy and programme. mod-104 covers *anti-affinity-bias operating norms in the hiring pipeline*; mod-108 covers *the corporation's ongoing DEI programme* including sponsorship, retention, and belonging.

### To [mod-110 — Privacy, Data Governance & Sector Compliance](../mod-110-privacy-data-governance-and-sector-compliance/)

- **HR-data privacy architecture** — the GDPR / CCPA / state-privacy-law treatment of employee and candidate data.
- **Interview-intelligence tool consent and retention** — the recording, storage, and retention posture for interview-intelligence tools (Metaview, BrightHire, Pillar) used in hiring.
- **HRIS data-classification and access-control policy** — SSO, MFA, role-based access, data-classification for sensitive fields (SSN, comp, benefits selections, disability status).

mod-104 identifies the privacy-adjacent decisions the ATS / HRIS / interview-intelligence tools raise; mod-110 owns the privacy architecture that governs them.

### To [mod-111 — Corporate Governance, Board Operations & Officer Duties](../mod-111-corporate-governance-board-operations-and-officer-duties/) and [mod-112 — Enterprise Risk, Insurance & Compliance](../mod-112-enterprise-risk-insurance-and-compliance/)

- **Officer appointment and D&O coverage** for exec hires — the board-consent mechanics for appointing an officer, the indemnification agreement, the D&O tower notification / addition.
- **EPLI coverage** — employment-practices liability insurance, which sits at the intersection of the hiring / onboarding operation and the enterprise-risk programme.
- **CFO / GC / audit-committee interactions** — the exec-hire process for finance and legal executives interacts with the audit committee (for CFO / controller) and the board (for GC).

### To [mod-113 — International Expansion & Global Workforce](../mod-113-international-expansion-and-global-workforce/)

- **International hiring** — per-country classification (employee vs. contractor per local law), EOR selection (Deel EOR, Remote, Papaya Global, Rippling International, Oyster), work-authorisation / immigration, per-country background checks (see [chapter 04](./04-reference-and-background-checks.md) for the top-level flag).
- **International payroll and benefits** — country-specific payroll, statutory benefits, and the graduation from EOR to local entity.
- **International onboarding variance** — per-country onboarding variants (mandatory local employment contract, per-country handbook, per-country I-9 equivalents).

mod-104 covers the US hiring / onboarding / HR-ops infrastructure; mod-113 covers the international overlay.

### To `startup-product-gtm-curriculum`

- **Sales / SDR / AE / CSM leveling and ramping** — the leveling framework, ramp expectations, quota-attainment definitions, and specialised ramp / enablement programmes for GTM roles. mod-104 covers the general hiring / onboarding infrastructure; the GTM track covers the *substantive* GTM-role architecture.
- **Sales-specific onboarding curriculum** — product training, competitive training, playbook training, ride-alongs. mod-104's onboarding programme in [chapter 06](./06-first-90-day-onboarding.md) provides the general structure; the GTM track fills in the GTM-role-specific curriculum.

### To `cto-curriculum`

- **Engineering leveling and IC-vs.-manager tracks** — the engineering-specific level framework, IC track (E1 → E7), manager track, dual-ladder policy, promotion criteria per engineering level.
- **Engineering-specific interview loop design** — the substantive design of the engineering interview (coding, systems design, project deep-dive, engineering-culture interview). mod-104 covers the *general structured-interviewing framework*; the CTO track covers the *engineering-specific interview loop*.

## The rule the module enforces

When a hiring / people / HR question lands, ask:

- Is it about *finding, interviewing, or onboarding* a candidate — the *pipeline machinery* — regardless of role? → **mod-104.**
- Is it about a *contract term or classification analysis* the pipeline must produce (offer letter, PIIA, W-2 vs. 1099, FLSA exemption, non-compete)? → **mod-103.**
- Is it about *equity grants at the policy level* (band, refresh cadence, comp-committee governance)? → **mod-105.**
- Is it about *compensation bands, levels, or benchmarking methodology*? → **mod-106.**
- Is it about *performance, promotion, PIPs, RIFs, or separation agreements* after onboarding? → **mod-107.**
- Is it about *culture, engagement, or DEI programmes* beyond hiring? → **mod-108.**
- Is it about *international hiring, EOR, or cross-border payroll*? → **mod-113.**
- Is it about *sales / SDR / AE / CSM leveling or ramp*? → **`startup-product-gtm-curriculum`.**
- Is it about *engineering-specific leveling, IC-vs-manager, or the engineering interview loop*? → **`cto-curriculum`.**
- Is it about *privacy, data governance, or interview-intelligence-tool consent*? → **mod-110.**
- Is it about *officer appointment, D&O, or EPLI*? → **mod-111 / mod-112.**

## Summary

- This module owns the general hiring / onboarding / HR-operations infrastructure — the pipeline machinery, the interview architecture, the compliance workflow (background check, I-9, E-Verify), the onboarding programme, and the HRIS / PEO stack.
- Its handoffs are precise: employment-law substance to mod-103; equity-comp policy to mod-105; compensation architecture to mod-106; performance / promotion / offboarding to mod-107; culture / DEI to mod-108; privacy / data governance to mod-110; officer / D&O to mod-111 / mod-112; international to mod-113; GTM leveling to the GTM track; engineering leveling to the CTO track.
- The rest of the Startup Operations & Governance track builds on top of a working hiring / onboarding / HR-operations layer. Get this module right, and every downstream module has firmer ground to stand on.
