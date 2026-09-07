# 10. Ownership boundary map

> What this module owns, and where each adjacent employment-and-people question is handed off.

## Motivation

The employee-facing legal architecture in this module is the ground floor for every downstream people-and-operations module. It sits between the founder-side legal architecture (mod-102), the HR operations and hiring workflow (mod-104), the equity-comp policy and comp committee (mod-105), the total-rewards architecture (mod-106), the performance-and-offboarding operations (mod-107), the culture-and-DEI program (mod-108), the commercial-contracts-and-IP layer (mod-109), the privacy-and-data-governance layer (mod-110), the corporate-governance layer (mod-111), the enterprise-risk-and-insurance layer (mod-112), and the international-workforce layer (mod-113).

Adjacent modules routinely collide at their edges. This chapter draws the boundary so that a diligence question, an operating incident, or a new-hire-package question finds its way to the right module without ambiguity.

## What this module owns

**mod-103 owns the employee-facing legal architecture** for the US workforce that is not a founder. Concretely:

- **Worker classification** — the W-2 vs. 1099 decision, the IRS common-law test, the FLSA economic-realities test, the California ABC test and its analogues, the audit surface, and the misclassification exposure ([chapter 01](./01-w2-vs-1099-worker-classification.md)).
- **FLSA exempt vs. non-exempt classification** — the salary-basis test, the five duties tests, the misclassification exposure ([chapter 02](./02-flsa-exempt-vs-non-exempt.md)).
- **Offer-letter architecture** — at-will framing, Montana carve-out, start date, position and reporting line, compensation summary, contingent conditions, pay-transparency disclosure, references to standalone PIIA / arbitration / relocation / bonus agreements ([chapter 03](./03-offer-letter-architecture-and-pay-transparency.md)).
- **Employee PIIA** — the employee-side variant of the founder PIIA from mod-102: pre-employment carveouts, present-assignment language, DTSA whistleblower-immunity notice, applicable state-law invention-assignment carveouts ([chapter 04](./04-employee-piia.md)).
- **NDA and MNDA layer** — mutual and one-way NDAs for customer, vendor, candidate, recruit, and investor conversations; standard exceptions and dispute-resolution clauses ([chapter 05](./05-nda-and-mnda-layer.md)).
- **Non-competes and their alternatives** — the FTC rule status, state-level bans and restrictions, and the practitioner default (narrow non-solicits, garden leave, trade-secret carveouts) ([chapter 06](./06-non-compete-landscape-and-alternatives.md)).
- **EEOC-protected-category framework across the employment lifecycle** — federal statutory core (Title VII, ADA, ADEA, PDA/PWFA/PUMP, EPA, GINA, USERRA, § 1981, NLRA) and the state-and-city expansion layer, applied to recruiting, interviewing, hiring, comp-setting, performance, promotion, and offboarding decisions ([chapter 07](./07-eeoc-protected-category-framework.md)).
- **State-law variance** — the nine recurring axes and the California / New York / Illinois / Washington / Colorado layers; the highest-common-denominator vs. per-state operating-policy decision ([chapter 08](./08-state-law-variance.md)).
- **Arbitration and class-action waivers** — post-*Epic Systems* enforceability, the EFAA carve-out, the PAGA bifurcation, *McLaren Macomb*, mass-arbitration risk, and current drafting patterns ([chapter 09](./09-arbitration-and-class-action-waivers.md)).

## What this module hands off

### To [mod-101 — Legal Entity Formation & Corporate Structure](../mod-101-legal-entity-formation-and-corporate-structure/)

- The *entity* that is doing the hiring — jurisdiction and form, Certificate of Incorporation and Bylaws, board consent authorising specific hires, EIN, foreign qualification for a state where the corporation now employs someone, franchise-tax and annual-report cadence.
- The corporation's authority to enter into employment agreements as an act of the corporation.

mod-103 assumes the entity exists and is qualified where its employees work.

### To [mod-102 — Founding-Team Legal Architecture](../mod-102-founding-team-legal-architecture/)

- The *founder-side* legal architecture — founder agreement, founder Stock Purchase Agreement, § 83(b) election, founder PIIA, DTSA whistleblower notice as it applies to founders, founder-side conflict-of-interest baseline, the founder-employment relationship and departure playbook, the retroactive-cleanup workstream for missing founder documents.
- The founder PIIA is the parent of the employee PIIA authored in mod-103 chapter 04; the mutuality, present-assignment language, and DTSA notice mechanics are the same across both.

Ask: is the question about a founder? → mod-102. Is it about an employee who is not a founder? → mod-103.

### To [mod-104 — Hiring, Onboarding & HR Operations](../mod-104-hiring-onboarding-and-hr-operations/)

- **Recruiting-workflow operations** — sourcing, ATS selection and configuration, structured-interview program design at scale, offer-approval workflow, offer-management tooling.
- **Background-check operations** — vendor selection, FCRA / state-law-compliant workflow, individualised-assessment tooling, adverse-action tracking.
- **Onboarding operations** — I-9 / E-Verify workflow beyond the day-one legal document, day-1 through day-90 onboarding checklist, orientation program, systems provisioning.
- **Employee handbook** — the master handbook that layers on top of the offer letter; policy authoring at depth (harassment prevention, IT-acceptable-use, remote-work, expense-reimbursement, PTO, etc.).
- **HRIS selection and payroll operations** — vendor selection, configuration, integration.
- **Benefits enrollment operations** — benefits vendor management, open-enrollment workflow, ACA compliance.
- **Employee-relations casework** — investigations, PIPs, separation-agreement workflow at scale.
- **AI-driven hiring tools and algorithmic decision-making** — NYC Local Law 144, Colorado AI Act SB 24-205, EEOC algorithmic-hiring guidance, ATS vendor's AI-feature usage.

mod-103 authors the *documents*; mod-104 operates the *processes* those documents are used within.

### To [mod-105 — Equity-Compensation Policy & the Compensation Committee](../mod-105-equity-compensation-policy-and-comp-committee/)

- **Grant-guideline architecture** — new-hire grants by level and role, refresh-cadence design, promotion-refresh grants, board-level equity, ESPP.
- **409A valuation cadence** — the ongoing 409A refresh program.
- **Compensation-committee** — charter, independence progression, exec-comp approval mechanics.
- **Equity-plan document** — the corporation's equity incentive plan document as approved by the board and stockholders.
- **Rule 701 aggregate-value math and Rule 701 disclosure documents.**

mod-103 references equity in the offer letter's compensation summary; the equity-comp policy and its design live in mod-105.

### To [mod-106 — Compensation Architecture & Total Rewards](../mod-106-compensation-architecture-and-total-rewards/)

- **Cash-comp architecture** — level-and-role framework, band design, pay-equity architecture, pay-transparency policy internal to the corporation (which employees see the bands), geographic differentials, market-comp benchmarking cadence.
- **Total-rewards program design** — health/dental/vision, 401(k), FSA/HSA, life and disability, wellness, commuter, EAP, education-assistance.
- **International compensation and benefits** (hands further to mod-113 for the cross-border layer).

mod-103's offer letter references the compensation architecture; mod-106 authors the architecture.

### To [mod-107 — Performance, Promotion & Offboarding](../mod-107-performance-promotion-and-offboarding/)

- **Performance-management program** — review cadence, calibration, rating system, competency framework.
- **Promotion process** — criteria, calibration, promotion-committee mechanics.
- **Performance improvement plans (PIPs)** — structure, cadence, documentation, escalation.
- **Reduction-in-force operations** — selection-criteria design, adverse-impact analysis, WARN and mini-WARN compliance, notification cadence, severance-benefit design, OWBPA-compliant group release.
- **Separation-agreement authoring** — release language, non-disparagement / confidentiality with *McLaren Macomb* carve-outs, reference / cooperation clauses.
- **Non-founder offboarding operations** — exit interview, systems deprovisioning, benefits transition, references program.

mod-103 sets the substantive framework for what a lawful termination looks like; mod-107 operates the process at scale, including the separation-agreement authoring that mod-103 gestures toward.

### To [mod-108 — Culture, Employee Experience & DEI](../mod-108-culture-employee-experience-and-dei/)

- **DEI program design** — diversity-recruiting, employee-resource-groups, pay-equity program at depth, workforce-representation reporting, post-*SFFA v. Harvard* considerations for race-conscious employment programs.
- **Harassment-prevention training** — California AB 1825 / SB 1343 mandatory training, NY State / NYC mandatory training, national program design.
- **Culture-and-values operationalisation** — employee engagement, pulse surveys, culture rituals.

mod-103 identifies the statutory anti-discrimination framework; mod-108 operationalises the corporation's culture and DEI response.

### To [mod-109 — Commercial Contracts, IP & Legal Ops](../mod-109-commercial-contracts-ip-and-legal-ops/)

- **Commercial-contract architecture** — MSAs, SOWs, customer contracts, vendor contracts, reseller and partner agreements.
- **Outbound and inbound IP-licensing strategy** — patent, copyright, trademark, trade-secret at scale; open-source-license compliance program.
- **Legal-ops tooling** — contract lifecycle management, e-signature, matter management, outside-counsel management.

The customer / vendor NDA architecture is scoped in mod-103 chapter 05 as it relates to the employee-facing paper (candidate, recruit, investor NDAs); mod-109 owns the customer and vendor NDA architecture at commercial scale.

### To [mod-110 — Privacy, Data Governance & Sector Compliance](../mod-110-privacy-data-governance-and-sector-compliance/)

- **Data-privacy program** — GDPR, CCPA / CPRA, other US state consumer-privacy statutes, HIPAA sector overlays, sector-specific frameworks (fintech, health-tech, gov-tech, AI-specific).
- **Employer-side employee-data handling** — CCPA / CPRA employee-data provisions, employee-monitoring frameworks, BYOD, remote-work data-security, cross-border employee-data transfer.
- **BIPA compliance at depth** — the biometric-data compliance program including HR-adjacent biometric touchpoints (time-and-attendance, facility access, ID verification), which mod-103 chapter 08 identifies for Illinois but leaves the depth to mod-110.
- **Data-protection agreements (DPAs) with HR-service vendors** (HRIS, payroll, benefits, background-check, ATS vendors as data processors of employee personal data).

mod-103 flags where privacy law meets the employment relationship; mod-110 owns the privacy program.

### To [mod-111 — Corporate Governance, Board Operations & Officer Duties](../mod-111-corporate-governance-board-operations-and-officer-duties/)

- **Officer-fiduciary-duty depth** — duty of care, duty of loyalty, duty of good faith, business-judgment rule, entire-fairness review, *Caremark* oversight duty at depth, especially for employment-law compliance as mission-critical risk.
- **Board-committee architecture** — compensation committee (which mod-105 references but mod-111 owns at depth), audit committee (which frequently owns whistleblower-hotline / ethics oversight), nominating-and-governance committee.
- **D&O insurance and EPLI overlay** — Directors and Officers coverage tower structure, EPLI (Employment Practices Liability Insurance) which is the primary insurance product that responds to the exposures identified in this module.

mod-103 identifies the risk surfaces; mod-111 owns the board-governance and D&O-insurance response.

### To [mod-112 — Enterprise Risk, Insurance & Compliance](../mod-112-enterprise-risk-insurance-and-compliance/)

- **Enterprise risk management program** — including HR / employment-liability as a risk category.
- **Insurance program design across all policy lines** — including EPLI in depth, fiduciary-liability coverage for benefit-plan administration, workers'-compensation across all states, unemployment-insurance registration and premium optimisation, cyber coverage for HR-data-breach scenarios.
- **Compliance-program design** — the anti-corruption, anti-retaliation, whistleblower-hotline, code-of-conduct, and training program that layer on top of the substantive law identified in this module.
- **Incident-response and crisis-management architecture** — including for employment-law incidents (harassment complaint, discrimination charge, DOL investigation, PAGA notice).

### To [mod-113 — International Expansion & Global Workforce](../mod-113-international-expansion-and-global-workforce/)

- **Per-country worker classification** — the country-specific "employee vs. contractor" tests (which are different from the US tests) and the exposure profile.
- **Employer-of-Record (EOR) vs. direct-hire vs. subsidiary architecture** — the strategic and cost trade-offs of the international-workforce entry pattern.
- **Cross-border payroll, benefits, tax-withholding, and social-security obligations.**
- **Work-authorisation and visa mechanics** — H-1B, L-1, O-1, TN, E-3, and other US work-authorisation programs; US-side inbound; outbound work authorisation in the destination country.
- **Per-country employment agreements** — including probationary-period, notice-period, works-council-consultation, and termination-notice rules that are radically different from US at-will employment.
- **International IP-assignment mechanics** — including moral-rights waivers and the country-specific present-assignment analysis.
- **International restrictive covenants** — non-compete enforceability outside the US.
- **International anti-discrimination and privacy overlays** — GDPR, per-country works-council, per-country protected-category expansion.

mod-103 owns the US employee-facing architecture; every cross-border question hands off to mod-113.

### To [mod-114 — Operations Function Design](../mod-114-operations-function-design/)

- **COO / GC / CoS operating-model design** — how the operations function is structured, how it interacts with the CEO and the board, how it evolves through funding stages.
- **When to hire in-house employment counsel vs. rely on outside firms.**
- **The people-operations function** — how HR is staffed at 10-, 30-, 100-, 300-employee inflection points.

### To a possible future labour-organising module (deferred)

- **Union / labor-organising layer** — the NLRA § 7 / § 8 doctrine at depth, election procedures, collective-bargaining, contract administration, unfair-labor-practice defense, strike-and-lockout planning.
- **Public-sector labor law analog** — where the corporation ever has government-contract-workforce components.

mod-103 references *McLaren Macomb* and the NLRA carve-outs from arbitration; the depth of union / labor-organising work is a future module if the market signal warrants.

## The rule the module enforces

When a diligence request or an operating question lands, ask:

- Is it about *worker classification, wage-hour, contract design, restrictive covenants, discrimination, or arbitration for a non-founder US employee*? → **mod-103.**
- Is it about a *founder*? → **mod-102.**
- Is it about the *entity itself*? → **mod-101.**
- Is it about *how the HR process runs*, rather than what the substantive law requires? → **mod-104** (recruiting, onboarding, HR operations, employee handbook, background-check operations).
- Is it about *equity-comp policy design*, rather than the offer-letter reference to equity? → **mod-105.**
- Is it about *cash-comp architecture, benefits program design, or total rewards*? → **mod-106.**
- Is it about *performance, promotion, PIPs, RIFs, or separation-agreement authoring*? → **mod-107.**
- Is it about *DEI program design, culture, or harassment-prevention training operations*? → **mod-108.**
- Is it about *customer / vendor / partner contracts or the broader IP program*? → **mod-109.**
- Is it about *privacy, data governance, sector compliance, or the biometric-data compliance program at depth*? → **mod-110.**
- Is it about *board operations, officer fiduciary duties, or the D&O / EPLI insurance program*? → **mod-111 / mod-112.**
- Is it about *another country*? → **mod-113.**
- Is it about the *operations function's own design*? → **mod-114.**

## Summary

- This module owns the US employee-facing legal architecture — worker classification, wage-and-hour, offer letters, PIIAs, NDAs, restrictive covenants, EEOC / state-law protected-category compliance, and arbitration provisions.
- Its handoffs are precise: founder-side to mod-102, entity-side to mod-101, HR operations to mod-104, equity-comp policy to mod-105, total rewards to mod-106, performance and offboarding to mod-107, culture and DEI to mod-108, commercial contracts and IP program to mod-109, privacy and biometrics depth to mod-110, board / officer / D&O depth to mod-111 and mod-112, cross-border to mod-113, operations-function-design to mod-114.
- The union / labor-organising layer is deferred to a future module; mod-103 references the NLRA carve-outs required for other purposes (arbitration provisions, confidentiality clauses) but does not author a labor-relations program.
- Get this module right and every downstream people-and-operations module has a stable substantive-law floor to operate on. The employee-facing legal architecture is the ground floor for hiring, comp, performance, and offboarding at scale.
