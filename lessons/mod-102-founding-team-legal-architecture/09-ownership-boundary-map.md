# 9. Ownership boundary map

> What this module owns, and where each adjacent question is handed off.

## Motivation

Curriculum modules routinely collide at their edges — nowhere more than in the founder legal architecture, which touches the entity layer beneath it, the employee legal architecture next to it, the priced-round financing above it, and the M&A / IPO / exit further out. This chapter draws the founder-side boundary so that a question landing on the COO / GC's desk finds its way to the right module without ambiguity.

## What this module owns

**mod-102 owns the founder-side legal architecture.** Concretely:

- **The founder agreement** — the equity-split conversation with rationale, roles and decision authority, dispute resolution, walk-away and re-vesting mechanics (see [chapter 01](./01-co-founder-equity-split-and-founder-agreement.md)).
- **The founder Stock Purchase Agreement (SPA)** as a *founder-side* instrument — purchase price and consideration, 4/1 vesting default, repurchase right at cost, transfer restrictions, standard reps and covenants (see [chapter 02](./02-founders-restricted-stock-and-repurchase.md)). The *corporation-side* authorisation of the issuance (board consent, share ledger entry) is owned by [mod-101 chapter 02](../mod-101-legal-entity-formation-and-corporate-structure/02-stand-up-the-entity.md).
- **The § 83(b) election** — the founder's timely-filed § 83(b) that starts the capital-gains clock and prevents the § 83(a) ordinary-income cascade (see [chapter 03](./03-83b-election-and-founder-tax-clock.md)).
- **The mutual IP assignment (PIIA)** for founders — present-assignment language, work-for-hire + assignment backstop, Prior Inventions schedule, state-law invention-assignment carveouts (see [chapter 04](./04-piia-mutual-ip-assignment.md)).
- **The DTSA whistleblower-immunity notice and the trade-secret baseline** — the 18 U.S.C. § 1833(b)(3) notice and the "reasonable measures" program that keeps trade-secret protection viable (see [chapter 05](./05-dtsa-whistleblower-and-trade-secret-baseline.md)).
- **Founder-side conflict-of-interest analysis** — DGCL § 144 interested-director transactions from the founder-director's seat, the *Caremark* oversight duty on a founder-director, the corporate-opportunity doctrine, and the anti-loyalty-conflict baseline (moonlighting, competitive activity, pre-existing IP disputes) (see [chapter 06](./06-founder-conflict-of-interest.md)).
- **The founder-employment relationship** — employee vs. contractor classification (almost always employee for a full-time founder), the defer-salary-for-equity trade, the founder-severance and founder-departure playbook, and departed-founder equity treatment on the cap table (see [chapter 07](./07-founder-employment-relationship-and-departure.md)).
- **The founder-diligence failure teardown** — the recurring defects an incoming COO / GC inherits and the retroactive-cleanup playbook (see [chapter 08](./08-founder-diligence-failure-teardown.md)).

## What this module hands off

### To [mod-101 — Legal Entity Formation & Corporate Structure](../mod-101-legal-entity-formation-and-corporate-structure/)

- The *entity* layer: choice of jurisdiction and form, Certificate of Incorporation and Bylaws, initial board consent as an act of the corporation, adoption of the equity incentive plan, corporate record and minute book discipline, franchise-tax and annual-report cadence, foreign qualification.
- The corporation-side authorisation of founder issuances (board consent authorising the issuance, share ledger entry, DGCL § 152 consideration determination).
- The Series-A "corporate-record-in-shambles" diagnostic on the *entity* side (mod-101 chapter 06); the founder-side twin lives in [chapter 08](./08-founder-diligence-failure-teardown.md) of this module.

### To [mod-103 — Employment Law, Worker Classification & Contract Design](../mod-103-employment-law-and-contract-design/)

- The *employee* legal architecture — offer letters and employment agreements for non-founder employees, worker classification (W-2 vs. 1099) for the broader workforce, FLSA exempt / non-exempt analysis, restrictive-covenant enforceability at depth (state-by-state non-compete and non-solicit landscape, FTC non-compete rule status, California Bus. & Prof. Code § 16600), the EEOC / harassment / discrimination framework, wage-and-hour compliance in depth, wrongful-termination doctrine.
- The employee-facing PIIA is the same document as the founder PIIA in most respects; mod-103 owns the employee-specific drafting variants (offer-letter integration, remote-workforce state-law overlays, executive-vs-standard-employee variants).

mod-102 authors the founder PIIA and the DTSA notice; mod-103 extends both to the employee base.

### To [mod-104 — Hiring, Onboarding & HR Operations](../mod-104-hiring-onboarding-and-hr-operations/)

- HR operations — hiring workflow, background checks, I-9 / E-Verify, benefits enrollment, PIIA execution as a day-one HR process, employee handbook, onboarding and offboarding checklists at scale.

### To [mod-105 — Equity-Compensation Policy & the Compensation Committee](../mod-105-equity-compensation-policy-and-comp-committee/)

- **Equity-comp policy** for the broader team — grant guidelines by level and role, refresh cadence, promotion refreshes, board-level equity, ESPP, exec-comp packages.
- **409A valuation** program at cadence (formation-day 409A is deferred until real grants happen; ongoing 409A refresh is mod-105).
- **Comp committee** charter, independence progression, exec-comp approval mechanics.
- **Follow-on grants to founders** at the *policy* level — the § 144 cleansing mechanics for founder-follow-on grants live in mod-102 chapter 06, but the *design* of a founder-refresh program lives in mod-105.

### To [mod-106 — Compensation Architecture & Total Rewards](../mod-106-compensation-architecture-and-total-rewards/) and [mod-107 — Performance, Promotion & Offboarding](../mod-107-performance-promotion-and-offboarding/)

- Cash-comp architecture, benefits design, total-rewards philosophy, performance-management, promotion, and non-founder offboarding at scale.

### To `startup-finance-fundraising-curriculum`

- **Priced-round preferred-stock and cap-table mechanics** — the Certificate of Designations for each series, Investors' Rights Agreement, Voting Agreement, Right of First Refusal & Co-Sale, priced-round Stock Purchase Agreement, option-pool math and shuffle, 1x non-participating preference and variants, liquidation-waterfall analysis, anti-dilution mechanics, protective provisions.
- **Cap-table modelling** — dilution modelling, 409A valuation methodology, Rule 701 aggregate-value caps, downround waterfall analysis.
- **Convertibles and SAFEs** — instrument design, cap and discount mechanics, conversion mechanics, side-letter treatment.

The founder-side SPA lives in mod-102 chapter 02; the priced-round SPA (for preferred stock sold to investors) lives in the finance-and-fundraising track.

### To `startup-exit-curriculum`

- **Change-of-control transaction mechanics** — M&A term sheet, definitive agreement, escrow and indemnification hold-back, working-capital adjustments, earn-outs, integration.
- **Single-trigger acceleration analysis** — the founder-CoC-accel debate at term sheet, its effect on the deal economics for the acquirer, and its interaction with the priced-round documents.
- **The founder-CoC-accel implementation** — how double-trigger acceleration flows through the merger agreement, escrow release, and tax treatment.
- **IPO readiness and executive-comp restructuring** — SOX §§ 302 and 404, public-company D&O, insider-trading, § 16 reporting, Rule 10b5-1 plans, ISS / Glass Lewis governance ratings.

mod-102 documents the *baseline* CoC-acceleration design in the founder SPA (double-trigger, market-standard); the transaction-mechanics view is `startup-exit-curriculum`.

### To [mod-109 — Commercial Contracts, IP & Legal Ops](../mod-109-commercial-contracts-ip-and-legal-ops/)

- Commercial-contract architecture (MSAs, SOWs, customer contracts, vendor contracts).
- The corporation's outbound and inbound IP-licensing strategy (patent, copyright, trademark, trade-secret, open-source-license compliance in depth).
- Legal-ops tooling (contract management, e-signature, matter management).

mod-102 chapter 04 covers founder IP assignment (PIIA); mod-109 covers the corporation's broader IP program.

### To [mod-110 — Privacy, Data Governance & Sector Compliance](../mod-110-privacy-data-governance-and-sector-compliance/)

- Data-privacy program (GDPR, CCPA, HIPAA sector overlays), data-processing agreements with vendors and customers, privacy-by-design, DPIAs.
- Sector compliance (fintech, health-tech, gov-tech, AI-specific frameworks).

### To [mod-111 — Corporate Governance, Board Operations & Officer Duties](../mod-111-corporate-governance-board-operations-and-officer-duties/)

- **Board operations depth** — quarterly board pack architecture, board committees (audit, compensation, nominating and governance), board evaluations, independent-director recruitment, board-observer rights.
- **Officer fiduciary-duty depth** — duty of care, duty of loyalty, duty of good faith, entire-fairness review, business-judgment rule, controlling-stockholder analysis (MFW / Kahn / Corwin), *Caremark* oversight duty at depth, demand-futility (Aronson / Rales / Zuckerberg unified test), stockholder derivative litigation defence.
- **D&O program architecture** at depth — tower structure (Side A, Side B, Side C), captives, DIC insurance, EPLI overlay, Cyber overlay, coverage-gap analysis.
- **Special committees** and their role in interested-director transactions at scale.

mod-102 chapter 06 covers founder-specific conflict analysis (§ 144, Caremark, corporate opportunity); mod-111 owns the depth for the board-operations context.

### To [mod-112 — Enterprise Risk, Insurance & Compliance](../mod-112-enterprise-risk-insurance-and-compliance/)

- Enterprise risk management program, insurance program design across all policy lines, compliance-program design, incident-response and crisis-management architecture.

### To [mod-113 — International Expansion & Global Workforce](../mod-113-international-expansion-and-global-workforce/)

- Cross-border founder-employment considerations (a founder based outside the US), international IP protection strategy, cross-border tax coordination for founder equity.
- International workforce mechanics (Employer of Record, direct-hire, work authorisation, cross-border payroll).

### To [mod-114 — Operations Function Design](../mod-114-operations-function-design/)

- The COO / GC / CoS operating-model design — how the operations function is structured, how it interacts with the CEO and the board, how it evolves through funding stages.

## The rule the module enforces

When a diligence request or an operating question lands, ask:

- Is it about the *founders themselves* — their contract with the corporation and with each other, their equity mechanics, their IP assignments, their 83(b)s, their conflict-of-interest analysis, their employment / departure? → **mod-102.**
- Is it about the *entity* — its formation, its corporate record, its compliance calendar, its qualification footprint? → **mod-101.**
- Is it about *employees other than founders*? → **mod-103 / mod-104 / mod-105 / mod-106 / mod-107 / mod-108** depending on the specific question.
- Is it about the *economics of a priced round or a cap-table model*? → **startup-finance-fundraising-curriculum.**
- Is it about a *change-of-control transaction*? → **startup-exit-curriculum.**
- Is it about *the board's operating machinery at depth or officer-duty depth beyond the founder-specific slice*? → **mod-111.**
- Is it about *another country*? → **mod-113.**

## Summary

- This module owns the founder legal architecture. Its handoffs are precise: entity-side to mod-101, employee-side to mod-103–107, priced-round mechanics to the finance-and-fundraising track, exit mechanics to the exit track, board-operations depth to mod-111.
- The founder-side documents (founder agreement, SPA, 83(b), PIIA + DTSA, employment agreement) form a package that Series-A diligence reads as a whole. Getting each individual document right is necessary; getting them to *cohere* is what makes the founder file diligence-ready.
- The rest of the Startup Operations & Governance track builds on top of a founder team that has a coherent legal architecture. Get this module right, and every downstream module — starting with mod-103's employee-facing legal work — has firmer ground.
