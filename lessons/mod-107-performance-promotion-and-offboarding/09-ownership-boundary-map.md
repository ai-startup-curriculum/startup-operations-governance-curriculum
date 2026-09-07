# 9. Ownership boundary map

> What this module owns, and where each adjacent performance / promotion / development / offboarding question is handed off.

## Motivation

The performance / promotion / development / offboarding operating system is the single people-ops surface that most touches — and is most touched by — the adjacent modules in the Startup Operations & Governance track and its sibling tracks. It reads from the leveling framework and comp bands in [mod-106](../mod-106-compensation-architecture-and-total-rewards/); it writes performance ratings back into the annual comp cycle in the same module; it consumes the equity policy from [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/) at every severance event and every executive departure; it depends on the substantive employment-law floor from [mod-103](../mod-103-employment-law-and-contract-design/) at every PIP, termination, and RIF; and it hands off role-specific performance nuance to the CTO and GTM curricula.

Because those edges collide constantly in practice — "is the sales quota-attainment PIP an OP-track question or a GTM-track question?", "is a CoC-triggered acceleration on severance an OP-track question or an equity-policy question?", "is a WARN-Act-triggered RIF at a Series-D asset sale an OP-track question or an exit-track question?" — this chapter draws the boundary explicitly. A diligence request, an operating incident, or a new process-authoring assignment should be able to land here and find its way to the correct owner in one step.

## What this module owns

**mod-107 owns the general performance / promotion / development / offboarding operating infrastructure** for the US workforce. Concretely:

- **The performance-management operating system** — cadence tied to the annual comp cycle, review-format decision by level, calibration norms across functions and levels, the manager-training programme for review authoring and delivery, and the performance-tool selection (Lattice, Culture Amp, 15Five, Betterworks, in-house spreadsheet at seed) ([chapter 01](./01-performance-management-operating-system.md)).
- **The promotion architecture** — function-level and cross-function promotion committees, competency- / sponsor- / impact-anchored criteria, semi-annual cadence with off-cycle exceptions, the promotion-communication playbook, and the not-promoted-signal-management playbook ([chapter 02](./02-promotion-architecture.md)).
- **The development / growth-plan / L&D programme** — the semi-annual growth conversation, the individual development plan (IDP) template, the manager-coaching programme (BetterUp / Better Manager / internal), the L&D budget allocation, the L&D-tool selection (LinkedIn Learning / Udemy Business / MasterClass / Coursera for Business / Reforge), and the internal-mobility programme ([chapter 03](./03-development-growth-plans-and-l-and-d-programme.md)).
- **The Performance Improvement Plan (PIP) mechanics** — trigger criteria after informal coaching has failed, the 30 / 60 / 90-day structure with weekly check-ins, the manager and HRBP support pattern, the recover / extend / release conclusion decision, and the anti-abuse operating norms that keep the PIP a coaching instrument rather than a paper trail ([chapter 04](./04-pip-mechanics.md)).
- **The voluntary and involuntary termination playbook** — the voluntary-resignation exit interview instrument; the involuntary-decision framework across misconduct / performance / role elimination; the 15-minute delivery-day script and choreography; the severance-and-release agreement authoring under the Speak Out Act 2022, OWBPA, the state Silenced No More statutes, and the *McLaren Macomb* NLRA constraint; and the final-pay and COBRA mechanics ([chapter 05](./05-termination-playbook.md)).
- **The RIF / layoff playbook under WARN** — board authorisation, impact analysis (function / level / tenure / work-location / demographic / cost-savings), federal WARN Act and state mini-WARN determination (California, New York, New Jersey, Wisconsin, Illinois, and others), the OWBPA disclosure schedule for the age-40+ pool, the executive-communications choreography, the severance / benefits / outplacement package, and the anti-signalling operating norms ([chapter 06](./06-rif-and-layoff-playbook-under-warn.md)).
- **The executive-team offboarding playbook** — the CEO-executive difficult-conversation script (Horowitz / Hoffman canon), the board-communication choreography, the exec-severance-and-release execution with attention to CoC-acceleration mechanics / indemnification continuation / board-seat resignation, and the employee-communications playbook for an executive departure ([chapter 07](./07-executive-team-offboarding.md)).
- **The alumni / rehire-eligibility / exit-interview feedback loop** — the alumni-network programme, the exit-interview data-collection loop that closes back into the performance-and-management improvement backlog, and the three-category (eligible / eligible-with-review / not-eligible) rehire-eligibility decision framework ([chapter 08](./08-alumni-rehire-eligibility-and-feedback-loop.md)).

## What this module hands off

### To [mod-101 — Legal Entity Formation & Corporate Structure](../mod-101-legal-entity-formation-and-corporate-structure/)

- The *entity* under which employees are hired, PIPed, promoted, terminated, or laid off — Delaware C-corp or otherwise, foreign qualification for a state where the corporation employs someone, the entity's authority under the Certificate of Incorporation and bylaws to enter into severance and release agreements as an act of the corporation.
- DGCL § 142 authority for the appointment and removal of officers — the base-layer statute that mod-107 chapter 07 (executive offboarding) leans on for the board-consent choreography around C-level departures.
- DGCL § 145 indemnification framework and the DGCL § 141(f) unanimous-written-consent mechanic used to execute board authorisation for material RIFs and executive severances.

mod-107 assumes the entity exists, is qualified where the workforce is located, and that the corporation has the constitutional authority to sign severance agreements and appoint / remove officers.

### To [mod-102 — Founding-Team Legal Architecture](../mod-102-founding-team-legal-architecture/)

- **Founder-employment departure mechanics** — the founder's own separation from an operating role (which is qualitatively different from an employee termination: founders often hold a board seat, control voting shares, and are named in the corporation's constitutional documents and its investor agreements). The founder-departure playbook, the founder-side severance-and-release drafting, and the founder-board-transition choreography live in mod-102.
- **Founder equity-vesting acceleration on separation** — governed by the founder Stock Purchase Agreement and the founder-side single-trigger / double-trigger framework in mod-102 and [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/).

mod-107 handles the *non-founder* offboarding operations at scale, including the executive-team playbook for non-founder executives. Ask: is the departure about a founder? → **mod-102 and mod-105.** Is it about a non-founder employee or executive? → **mod-107.**

### To [mod-103 — Employment Law, Worker Classification & Contract Design](../mod-103-employment-law-and-contract-design/)

- **The at-will framework and the state-law exceptions.** mod-103 authors the offer-letter at-will framing that makes involuntary termination substantively permissible; mod-107 executes within that framework and defers to mod-103 for the substantive-law questions ("is a Montana pre-completion-of-probationary-period termination governed by the Montana Wrongful Discharge from Employment Act?").
- **The EEOC-protected-category framework** — Title VII, ADA, ADEA, PDA / PWFA / PUMP, EPA, GINA, USERRA, § 1981, NLRA, and the state / city expansion layer. mod-107's demographic-slice reviews on PIP openings, promotion decisions, and RIF selection lean on the mod-103 framework for what the protected categories *are*; mod-103 owns the substantive-law depth.
- **State-law variance at depth** — the mod-103 chapter 08 catalogue of California / New York / Illinois / Washington / Colorado / Massachusetts / New Jersey overlays. mod-107 references specific state statutes in the termination and RIF chapters (California Silenced No More Act SB 331, the Cal-WARN interpretation, New York WARN Labor Law §§ 860–860-i, New Jersey mandatory RIF severance, California Labor Code §§ 201–203 final-pay timing) but the *substantive* state-law analysis at authoritative depth lives in mod-103.
- **Arbitration and the EFAA carve-out for sexual harassment and sexual assault claims** — mod-107 chapter 05 references the Ending Forced Arbitration Act; the substance of the corporation's arbitration architecture and the *Epic Systems* / EFAA / PAGA landscape is authored in mod-103.
- **PIIA continuing obligations after departure** — the employee PIIA authored in mod-103 chapter 04 (confidentiality, invention assignment, non-solicit if any) survives termination; mod-107's severance-and-release agreements reaffirm continuing obligations under the mod-103 PIIA and add the release layer, but the underlying PIIA and its state-law-specific invention-assignment carve-outs live in mod-103.
- **Non-compete enforceability and the FTC-rule / state-law overlay** — mod-107 chapter 07 references non-compete scope in executive severance; mod-103 chapter 06 owns the substance.

mod-103 sets the substantive-law floor for what a lawful termination, PIP, or severance-and-release looks like; mod-107 operates the process at scale.

### To [mod-104 — Hiring, Onboarding & HR Operations](../mod-104-hiring-onboarding-and-hr-operations/)

- **The HRIS / PEO / payroll stack** (Rippling, Gusto, Justworks, TriNet, Deel, Workday, Dayforce, BambooHR) that mod-107 depends on to store performance data, execute final pay against the state-specific timing rules, deliver COBRA notices, and administer the termination workflow.
- **The benefits broker and 401(k) provider relationships** (Newfront, Sequoia, Guideline, Human Interest) that administer COBRA and benefits continuation at termination.
- **The ATS integration** for the internal-mobility programme in chapter 03 — the internal job board, the internal-first posting window, and the internal-referral flag live inside the ATS mod-104 owns.
- **The 90-day new-hire onboarding programme** — the 90-day handoff from mod-104 chapter 06 into mod-107's performance-management operating system.
- **The employee handbook** that mod-104 authors and that mod-107 relies on for the corporation's PTO-payout policy at termination, the disciplinary escalation ladder that PIPs live inside, and the workforce-conduct standards that misconduct terminations enforce.

mod-104 operates the *systems* (HRIS, ATS, benefits, handbook); mod-107 operates the *performance-and-offboarding processes* those systems execute.

### To [mod-105 — Equity-Compensation Policy & the Compensation Committee](../mod-105-equity-compensation-policy-and-comp-committee/)

- **Equity treatment on separation** — post-termination exercise (PTE) window for ISOs (default 3 months to preserve ISO status under IRC § 422(a)(2); many plans permit 12–24 months at the cost of ISO status), vested-vs-unvested treatment at termination, extended PTE windows for RIF-affected employees.
- **CoC-triggered acceleration** — single-trigger and double-trigger acceleration mechanics on executive grants, the interaction between standalone executive-severance clauses and CoC-triggered acceleration, and the material-board-decision items that surface in a CoC-window separation. mod-107 chapter 07 references the mechanics; mod-105 owns the equity-plan-document substance and the compensation-committee authority to approve.
- **Executive-severance policy at the equity layer** — severance-triggered vesting acceleration, retention-bonus and stay-bonus authorisation, and the compensation-committee delegation framework for approving executive-separation packages that exceed pre-authorised policy.
- **Retention grants and retention-bonus authorisation during a RIF** — retention grants for the surviving population that stabilises the organisation after a layoff are a comp-committee matter under mod-105, not a mod-107 matter.
- **Board-seat compensation and board-observer arrangements** — mod-107 chapter 07 notes when a departing executive's board-seat resignation is required; the compensation and equity treatment of board seats themselves is mod-105 territory.
- **409A valuation cadence** and the strike-price setting for any post-departure grants that follow a RIF or executive transition.

mod-107 gestures at the equity-treatment mechanics at every separation event; mod-105 owns the equity policy that governs.

### To [mod-106 — Compensation Architecture & Total Rewards](../mod-106-compensation-architecture-and-total-rewards/)

- **The leveling framework and comp bands** that the performance rubric in mod-107 chapter 01 rates against, and that the promotion committee in mod-107 chapter 02 promotes into.
- **The annual comp cycle** that reads the performance rating out of mod-107 chapter 01 and applies the merit-budget curve. mod-107 anchors its review cadence to the mod-106 comp-cycle calendar (October / November review → December calibration → January merit / equity refresh / promotion).
- **The merit-budget allocation** for on-cycle promotions and the mid-year promotion-budget carve-out for the off-cycle exception path — a comp-cycle mechanic under mod-106, not a mod-107 mechanic.
- **The promotion-refresh grant guideline** — what a promotion costs in cash (base + target bonus) and equity (refresh grant sized against the target level's grant guideline). mod-107 chapter 02 signals when a promotion is approved; the substantive comp-and-equity change is authored in mod-106 (cash) and mod-105 (equity).
- **The severance-package sizing benchmarks** (Compensia, Radford / Aon, Carta Executive, Pave, Option Impact / Advanced-HR) that inform the executive-severance package design in mod-107 chapter 07. mod-107 references the sizing decisions; mod-106 owns the benchmarking methodology.
- **The total-rewards architecture** — health, dental, vision, 401(k), FSA / HSA, life and disability, wellness, EAP, education-assistance — that mod-107 references at COBRA / benefits-continuation moments but does not itself design.
- **Pay-transparency internal to the corporation** — which employees see the bands, and the interaction with the promotion-communication playbook in mod-107 chapter 02.

mod-107 consumes the comp-and-benefits architecture at every performance rating, promotion decision, and severance event; mod-106 authors the architecture.

### To [mod-108 — Culture, Employee Experience & DEI](../mod-108-culture-employee-experience-and-dei/)

- **The engagement and pulse-survey programme** — the ongoing measurement of the employee experience that sits *between* the semi-annual formal reviews and the exit interviews. mod-107's exit-interview feedback loop in chapter 08 is one channel; the pulse-survey programme in mod-108 is another, and the two feed the same executive people-metrics review.
- **The values-operationalisation programme** — how the corporation's values are read into performance rubrics, promotion criteria, and hiring decisions. mod-107 authors the operating mechanics; mod-108 authors the values themselves and the culture programme that makes them load-bearing.
- **Sponsorship and mentorship programmes** — cross-cutting programmes that support the promotion architecture in mod-107 chapter 02 but that live inside the culture / DEI programme.
- **DEI programme design at depth** — diversity-recruiting, employee-resource-groups, pay-equity programme at scale, workforce-representation reporting, post-*SFFA v. Harvard* considerations for race-conscious employment programmes. mod-107's demographic-slice reviews on PIPs, promotions, RIF selection, and rehire eligibility are pattern-detection mechanisms that lean on the mod-108 DEI programme for the substantive framing.
- **Harassment-prevention training** — California AB 1825 / SB 1343 mandatory training, New York State + NYC training, Illinois SB 75, Delaware, Connecticut, Maine, Washington. mod-107 references misconduct terminations that arise from harassment investigations; mod-108 owns the prevention-training programme.

mod-107 operates the individual performance-and-offboarding decisions; mod-108 owns the corporate culture, engagement, and DEI programme in which those decisions land.

### To [mod-109 — Commercial Contracts, IP & Legal Ops](../mod-109-commercial-contracts-ip-and-legal-ops/)

- **Outside-counsel management** — the retained employment-law firm that reviews severance-and-release agreements, the state-specific counsel that reviews jurisdiction-specific separations, and the securities counsel that reviews Item 5.02 / Item 2.05 8-K disclosures on material RIFs and executive departures.
- **Legal-ops tooling** — contract lifecycle management, e-signature, and matter management that support the severance-and-release execution workflow.
- **Trade-secret and IP-assignment enforcement** at departure — the enforcement infrastructure that turns a PIIA breach into a claim. mod-107's severance-and-release confirms continuing IP obligations; mod-109 owns the enforcement layer.

### To [mod-110 — Privacy, Data Governance & Sector Compliance](../mod-110-privacy-data-governance-and-sector-compliance/)

- **Employee-data handling on departure** — CCPA / CPRA employee-data provisions, data-retention and deletion obligations for personnel files, access to systems the departing employee touched (including BYOD offboarding and remote-work data-security), and the data-processing-agreement scope with HR-service vendors (HRIS, performance-management tool, exit-interview data platform).
- **Performance-data privacy** — the performance-rating, PIP-documentation, and exit-interview record retention schedule sits inside the corporation's records-retention programme in mod-110, not in mod-107.
- **International-employee-data transfer** for cross-border performance data — GDPR consequences for exit-interview data on European employees hand off through mod-110 and mod-113.

### To [mod-111 — Corporate Governance, Board Operations & Officer Duties](../mod-111-corporate-governance-board-operations-and-officer-duties/)

- **The compensation-committee charter, independence progression, and delegation framework** — the board-committee architecture that authorises material executive severances, retention grants, and material RIF packages. mod-107 chapter 06 and chapter 07 name where board or comp-committee authorisation is required; mod-111 owns the charter substance and the officer-appointment procedure.
- **The audit-committee involvement in CFO / Controller departures** — the exchange-listing-standard independent line to the CFO (Nasdaq 5605(c)(3); NYSE 303A.07) that shapes the mod-107 chapter 07 executive-offboarding choreography for CFO transitions.
- **The nominating-and-governance committee involvement in the executive-succession process.**
- **Officer fiduciary duties** — the duty of care that runs on the CEO and the board when authorising a RIF, an executive termination, or a change in the performance-management operating system; the *Caremark* oversight duty for employment-law compliance as a mission-critical risk.
- **D&O tower coverage for the executive's period of service** — indemnification agreement continuation, tail coverage, side A / B / C treatment of a former officer. mod-107 chapter 07 references the D&O reaffirmation clause in the executive separation agreement; mod-111 (and mod-112) own the D&O programme.

### To [mod-112 — Enterprise Risk, Insurance & Compliance](../mod-112-enterprise-risk-insurance-and-compliance/)

- **Employment Practices Liability Insurance (EPLI)** — the primary insurance product that responds to the exposures identified across mod-107 (PIP-related wrongful-termination claims, RIF-related disparate-impact ADEA claims, misconduct-termination retaliation claims). mod-107 identifies the exposure surfaces; mod-112 owns the EPLI programme.
- **Fiduciary-liability coverage for benefit-plan administration** and **workers'-compensation coverage** across all states in which the corporation employs someone.
- **Incident-response and crisis-management architecture** for a specific employment-law incident (harassment complaint, discrimination charge, DOL investigation, PAGA notice) or for a material RIF that draws public and press attention.
- **The compliance-programme design** — anti-retaliation policy, whistleblower hotline, code of conduct, ethics-training programme — that layers on top of the specific mod-107 operating decisions.

### To [mod-113 — International Expansion & Global Workforce](../mod-113-international-expansion-and-global-workforce/)

- **Per-country performance-management norms** — where cultural, statutory, or works-council norms modify the review cadence, the review format, or the rating scale mod-107 authors for the US.
- **Per-country termination and severance mechanics** — statutory notice periods (radically longer than US at-will), statutory severance (unheard of in most US contexts and standard in most non-US contexts), works-council-consultation requirements, mass-dismissal notification frameworks, and per-country protected-category expansion. A "RIF" in France, Germany, or the Netherlands is not a WARN-Act question, it is a completely different regulatory question that mod-113 owns.
- **Employer-of-Record (EOR) offboarding** — the practical mechanics of executing a termination through Deel, Remote, Velocity Global, Papaya, or a regional EOR partner, including the EOR's contractual severance-execution scope.
- **Cross-border data handling** for performance data and exit-interview data — GDPR / EU-US Data Privacy Framework consequences for personnel data.

mod-107 owns the US performance-and-offboarding operating system; every cross-border question hands off to mod-113.

### To [mod-114 — Operations Function Design](../mod-114-operations-function-design/)

- **The people-function operating model** — how the HR / people-ops function is staffed at 10-, 30-, 100-, 300-, 1,000-employee inflection points. mod-107 assumes an HRBP layer exists at Series-A / Series-B; mod-114 owns the staffing model that puts the HRBP in place.
- **When to hire in-house employment counsel** vs. rely on outside firms — a mod-114 operating-model question that shapes how mod-107's severance-agreement review workflow is staffed.
- **The head-of-people to Chief People Officer progression** and the interaction with the CEO's operating team.

### To [`startup-product-gtm-curriculum`](https://github.com/anthropics/ai-infra-curriculum) (sibling track)

- **GTM-role-specific PIP and performance nuance.** Sales roles have quota-attainment thresholds that function as PIP triggers in a way that is qualitatively different from engineering or product performance-management. The distinction between a *ramp-fail* (the new hire has not yet reached full productivity in a defined ramp period, and the correct response is coaching / ramp-plan adjustment, not a PIP) and a *capability-fail* (the fully-ramped rep is consistently under-performing against quota, and a PIP is appropriate) is a GTM-track question, not a mod-107 question.
- **Sales-manager coaching cadence and the sales-specific review format** — sales enablement, deal-review cadence, forecasting-accuracy assessment, and the specific measurement instruments of sales performance.
- **GTM-specific promotion criteria and levelling** — AE / SDR / CSM / SE ladders, the enterprise-vs-mid-market-vs-SMB dimension of leveling, and the promotion-committee construction inside a GTM function.
- **Commission clawback, quota-relief, and comp-plan design on separation** — how a departing rep's commissions are handled at termination, and what the sales-commission-agreement addendum to the separation agreement looks like.

mod-107 authors the *general* performance-and-offboarding operating system; the GTM-role-specific overlay lives in the GTM curriculum.

### To [`cto-curriculum`](https://github.com/anthropics/ai-infra-curriculum) (sibling track)

- **Engineering-role-specific performance and promotion nuance.** The E1 → E7 competency ladder (or the corporation's equivalent), the staff-plus promotion criteria, the tech-lead-vs-manager track branching, and the individual-contributor senior-track (Staff / Principal / Distinguished) all live in the CTO curriculum.
- **Engineering-specific review format** — code-review quality signal, technical-scope signal, cross-team-influence signal, and the specific work-samples an engineering promotion committee reads.
- **Engineering-manager-vs-IC-track leveling parity** — the compensation parity, promotion parity, and career-transition mechanics between the two tracks.
- **On-call and incident-response performance dimensions** — the qualitative performance signals that engineering leadership reads and that do not map neatly to a general competency framework.

mod-107 authors the general performance operating system; the engineering-role-specific competency ladders and review formats live in the CTO curriculum.

### To [`startup-exit-curriculum`](https://github.com/anthropics/ai-infra-curriculum) (sibling track)

- **Transaction-related workforce reductions.** An M&A-integration-driven RIF, a buyer-side retention-pool design, a transaction-close severance mechanic, or a divestiture-driven layoff is a transaction-execution question that lives in the exit curriculum. The RIF playbook in mod-107 chapter 06 applies underneath (WARN Act, OWBPA, severance-and-release drafting still governs), but the *transaction-side* choreography — buyer-seller negotiation on retention pools, purchase-agreement carve-outs for pre-close severance obligations, allocation of severance liability between buyer and seller, seller-side CoC-acceleration triggers under equity grants — is exit-curriculum territory.
- **Retention-bonus and stay-bonus design in an M&A context** — the transaction-close retention grants, the CoC-triggered acceleration, and the double-trigger severance package that the buyer or seller conditions on close.
- **The purchase-agreement representations and warranties on the workforce** — the seller's disclosure of pending employment litigation, WARN-Act liabilities, and unpaid-comp obligations that the exit curriculum owns.

mod-107 owns the *general* RIF playbook that governs any workforce reduction; the *transaction-driven* workforce reduction hands off to the exit curriculum.

## The rule the module enforces

When a diligence request or an operating question lands, ask:

- Is it about *how performance is reviewed, rated, calibrated, or communicated* for a non-founder US employee? → **mod-107 chapter 01.**
- Is it about *how promotions are decided, communicated, or contested*? → **mod-107 chapter 02.**
- Is it about *how the corporation develops its people, allocates the L&D budget, or supports internal mobility*? → **mod-107 chapter 03.**
- Is it about *when to open a PIP, how to structure it, or how to conclude it*? → **mod-107 chapter 04.**
- Is it about *an individual voluntary or involuntary termination — the decision, the delivery-day conversation, the severance-and-release drafting, the final-pay / COBRA mechanics*? → **mod-107 chapter 05.**
- Is it about *a group workforce reduction — WARN-Act analysis, OWBPA disclosure, communications choreography, package design*? → **mod-107 chapter 06.**
- Is it about *an executive-team departure — CEO-executive conversation, board choreography, CoC / indemnification / board-seat mechanics, employee-and-external comms*? → **mod-107 chapter 07.**
- Is it about *the alumni programme, the exit-interview feedback loop, or rehire eligibility*? → **mod-107 chapter 08.**
- Is it about *a founder*? → **mod-102** (with the equity-vesting-acceleration piece in **mod-105**).
- Is it about *the substantive employment-law floor (at-will framing, protected-category framework, state-law variance, PIIA continuing obligations, arbitration, non-competes)*? → **mod-103.**
- Is it about *the HRIS / PEO / benefits-broker / ATS system layer or the employee handbook*? → **mod-104.**
- Is it about *equity-plan-document mechanics, CoC-acceleration mechanics, post-termination exercise windows, or comp-committee authority to approve executive severance*? → **mod-105.**
- Is it about *the leveling framework, comp bands, the annual comp-cycle mechanics, or the merit / promotion-refresh grant sizing*? → **mod-106.**
- Is it about *the culture, engagement, sponsorship, or DEI programme in which the performance operating system lands*? → **mod-108.**
- Is it about *the D&O tower, EPLI coverage, or the board-committee architecture*? → **mod-111** or **mod-112.**
- Is it about *another country*? → **mod-113.**
- Is it about *a sales / SDR / AE / CSM performance or PIP question*? → **`startup-product-gtm-curriculum`.**
- Is it about *an engineering ladder, staff-plus promotion, or IC-vs-manager-track question*? → **`cto-curriculum`.**
- Is it about *a workforce reduction driven by a specific transaction*? → **`startup-exit-curriculum`.**

## Summary

- This module owns the general performance / promotion / development / offboarding operating infrastructure for the US workforce — the performance-management operating system, the promotion architecture, the development-and-L&D programme, the PIP mechanics, the termination playbook, the WARN-Act-compliant RIF playbook, the executive-team offboarding playbook, and the alumni / rehire-eligibility / exit-interview feedback loop.
- Its handoffs are precise: substantive employment law to mod-103, HRIS / ATS / handbook operations to mod-104, equity policy on separation to mod-105, comp architecture and merit / promotion cash-and-equity sizing to mod-106, culture / engagement / DEI programme to mod-108, board-committee architecture and D&O / EPLI to mod-111 and mod-112, cross-border to mod-113, GTM-role-specific performance nuance to `startup-product-gtm-curriculum`, engineering-role-specific performance nuance to `cto-curriculum`, and transaction-related workforce reductions to `startup-exit-curriculum`.
- Founder departures are mod-102 (with the equity-vesting-acceleration piece in mod-105), not mod-107.
- Get this module right and every downstream people-and-operations decision has a stable operating-process floor to run on. Get its boundaries right and every diligence request or operating incident finds its correct owner in one step.
