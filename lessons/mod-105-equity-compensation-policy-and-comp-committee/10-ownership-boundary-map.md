# 10. Ownership boundary map

> What this module owns, and where each adjacent question is handed off.

## Motivation

Equity-compensation policy sits between a dense set of adjacent concerns: the fundraising-finance layer that governs the economics of the option pool, 409A valuation, and dilution waterfalls; the exit layer that governs how CoC transactions execute; the employment-law layer that governs the contracts in which exec-comp lives; the hiring-ops layer that moves exec hires through a pipeline; the compensation-architecture layer that governs bands and leveling; the performance-management layer that feeds the annual comp cycle; the privacy layer that governs how comp data is handled; the corporate-governance layer that governs the comp committee as a board committee; the enterprise-risk layer that insures exec-separation disputes; and the international-workforce layer that governs per-country equity sub-plans.

Boundaries in a curriculum are a service to the learner and to the operating CEO / CFO / GC / head of people. When an equity-comp question shows up, the boundary map tells you where the answer lives.

## What this module owns

**mod-105 owns the equity-compensation policy substance and the compensation-committee operating infrastructure.** Concretely:

- **The grant-guideline table** — grant-size bands by level and function at seed / A / B / growth, with the methodology that produces them (see [chapter 01](./01-grant-guidelines-by-level-and-function.md)).
- **The IC equity-plan structure** — ISO vs. NSO vs. RSU selection, vesting default (four-year with one-year cliff), early-exercise policy, post-termination exercise window, repurchase and ROFR architecture (see [chapter 02](./02-ic-equity-plan-structure.md)).
- **Refresh, promotion, and retention grants** — the refresh cadence (annual top-up vs. four-year refresh), promotion-driven refresh sizing, retention / "evergreen" grants and the policy that governs them (see [chapter 03](./03-refresh-promotion-and-retention-grants.md)).
- **Executive compensation packages** — the design of VP+ and C-suite comp packages (cash, equity, sign-on, severance, acceleration) and the negotiation posture that governs them (see [chapter 04](./04-executive-compensation-packages.md)).
- **The compensation committee** — charter, independence progression, cadence, authority, delegation to Committee Chair, resolution and minutes architecture (see [chapter 05](./05-compensation-committee.md)).
- **The annual comp cycle** — timing (calendar vs. fiscal-year anchored), workflow (manager inputs → calibration → committee approval → delivery), budget derivation, merit vs. equity-refresh split (see [chapter 06](./06-annual-comp-cycle.md)).
- **Change-of-control equity policy** — the single-trigger vs. double-trigger landscape, the acceleration ladder by role, the "modified single trigger" for the CEO (see [chapter 07](./07-change-of-control-equity-policy.md)).
- **Executive severance and release architecture** — the exec severance ladder (cash multiplier, benefits continuation, equity acceleration, consulting-tail), the release-of-claims mechanic, the OWBPA / ADEA 21-day / 45-day / 7-day structure for exec separations (see [chapter 08](./08-executive-severance-and-release.md)).
- **Reg S-K Item 402 pre-IPO exec-comp disclosure** — the Summary Compensation Table, the Grants of Plan-Based Awards table, the Outstanding Equity Awards table, CD&A build, pay-vs.-performance disclosure, and the pre-IPO work needed to make the first 10-K comp disclosure survive scrutiny (see [chapter 09](./09-sec-reg-sk-item-402-disclosure.md)).

## What this module hands off

### To `startup-finance-fundraising-curriculum` (equity-comp ECONOMICS)

- **Option-pool sizing and dilution math** — the pre-money / post-money option-pool "shuffle", top-up at each round, dilution modeling across the preferred-stack.
- **Waterfall analysis** — common / preferred / option waterfalls at various exit values; participating-preferred vs. non-participating behavior.
- **409A valuation methodology** — valuation-firm selection, safe-harbor conditions, refresh triggers, FMV discipline for grant-pricing.
- **Rule 701 aggregate-value caps** — the $10M disclosure trigger and the aggregate-grant-value math that drives it.
- **Tax-preference and QSBS economics** — the QSBS five-year clock, the $10M / 10× basis exclusion, and the planning posture around it.
- **Early-exercise tax arithmetic** — the 83(b) election math, AMT exposure on ISO exercises, strategies for exec equity-planning.

mod-105 owns the *policy substance* (what grant, what vest, what refresh); the fundraising-finance track owns the *economics underneath* (what pool, what dilution, what valuation, what tax outcome).

### To `startup-exit-curriculum`

- **CoC transaction execution** — the 280G cleanse mechanics (the 75% stockholder vote, the disclosure statement, the exec waivers), tender-offer execution for secondary liquidity, acquirer-stock-election mechanics at closing, the stock-vs.-cash allocation and the tax posture that drives it.
- mod-105 owns the *CoC equity policy* (acceleration terms, treatment of unvested, exec severance triggers); the exit track owns the *transaction execution* when the CoC actually happens.

### To [mod-103 — Employment Law & Contract Design](../mod-103-employment-law-and-contract-design/)

- **Offer-letter architecture and worker-classification analysis** — the offer-letter structure, W-2 vs. 1099 and FLSA exempt-vs-non-exempt analysis.
- **Non-compete and non-solicit survivors in exec agreements** — the state landscape; the surviving-clauses pack when non-competes are void.
- **Pay-transparency state law** — California, New York, Washington, Colorado, Illinois and the per-state posting / disclosure obligations that constrain how comp bands are communicated.

### To [mod-104 — Hiring, Onboarding & HR Operations](../mod-104-hiring-onboarding-and-hr-operations/)

- **Executive-hiring pipeline** — retained search-partner selection, the exec interview panel, the exec offer-presentation mechanics, the 100-day onboarding plan.
- mod-104 owns the *process* of hiring an executive; mod-105 owns the *policy substance* (grant size, vesting, acceleration, severance ladder) that fills in the offer the pipeline presents.

### To [mod-106 — Compensation Architecture & Total Rewards](../mod-106-compensation-architecture-and-total-rewards/)

- **Leveling and compensation bands** — the leveling framework, cash-comp bands per level, geographic differentials, benchmarking methodology (Radford, Compensia, Aon, Carta compensation).
- **Total-rewards design** — the substantive design of the benefits program beyond equity (medical, 401(k), executive-benefit enhancements).
- mod-105 owns *equity-comp policy*; mod-106 owns *cash-comp architecture and total rewards*.

### To [mod-107 — Performance, Promotion & Offboarding](../mod-107-performance-promotion-and-offboarding/)

- **The performance-review instrument** — the review cadence, scoring instrument, calibration process that feeds the annual comp cycle.
- **Involuntary-termination operating procedure and RIF process** — PIPs, WARN Act notice, RIF selection methodology.
- **IC separation-agreement library** — the standard release-of-claims and severance-letter templates for non-exec separations.
- mod-105 keeps the *exec-separation substance* (acceleration mechanics, 280G waivers, consulting-tail design); mod-107 owns IC separation architecture.

### To [mod-108 — Culture, Employee Experience & DEI](../mod-108-culture-employee-experience-and-dei/)

- **Pay-equity program design** — the pay-equity audit, remediation methodology, ongoing monitoring.
- **DEI-weighted comp decisions** — the DEI inputs into calibration and promotion decisions.
- **Employee-wide comp communications** — the all-hands / handbook messaging about comp philosophy, transparency posture.

### To [mod-110 — Privacy, Data Governance & Sector Compliance](../mod-110-privacy-data-governance-and-sector-compliance/)

- **Comp data as sensitive personnel data** — the privacy architecture that governs comp data (GDPR / CCPA / state-privacy-law treatment).
- **HRIS data-classification** — the SSO, MFA, role-based-access, and data-classification posture for comp fields in Rippling / Workday / Carta.
- **Comp-committee materials retention and access controls** — the retention schedule and access controls for Diligent / Boardvantage board-portal comp-committee packets.

### To [mod-111 — Corporate Governance, Board Operations & Officer Duties](../mod-111-corporate-governance-board-operations-and-officer-duties/)

- **The comp committee as a board committee** — the delegation architecture, resolution templates, minutes discipline, the committee's relationship to the full board.
- **D&O and indemnification agreements for exec hires** — the officer-appointment resolution, indemnification-agreement template, D&O tower notification.
- mod-105 owns the *comp-committee charter and operating cadence*; mod-111 owns the *board-committee architecture* within which the comp committee sits.

### To [mod-112 — Enterprise Risk, Insurance & Compliance](../mod-112-enterprise-risk-insurance-and-compliance/)

- **EPLI coverage for exec-separation disputes** — employment-practices liability insurance, the coverage posture around exec separations and release disputes.
- **D&O coverage during a CoC transaction window** — the Side-A DIC tower, the tail / run-off coverage at closing, the D&O posture through the CoC window.

### To [mod-113 — International Expansion & Global Workforce](../mod-113-international-expansion-and-global-workforce/)

- **Per-country equity-plan sub-plans** — the UK EMI scheme, Canadian stock-option variations, EU per-country sub-plans, Israeli 102 trustee plans.
- **EOR vs. local-entity equity-grant interaction** — the restrictions on granting equity through an EOR vs. a local entity.
- **Per-country severance statutory minimums** — statutory severance / notice in each jurisdiction, how the exec-severance ladder stacks on top of local minimums.

### To a future `startup-people-ops-controllership` track

- **IC-level equity-administration mechanics** — Carta administrator operations, grant-letter mail-merge, 83(b) filing walk-through, option-exercise tax-advisor handoff, cap-table reconciliation to the equity plan.
- mod-105 owns the *policy substance* that governs grants; the people-ops controllership track owns the *IC-level administrative mechanics* that execute them.

## The rule the module enforces

When an equity-comp / people-economics question lands, ask:

- Is it about *equity-grant policy* (what size, what vesting, what refresh, what acceleration) at the IC or exec level? → **mod-105.**
- Is it about *comp-committee governance* (charter, cadence, delegation, minutes)? → **mod-105.**
- Is it about *option-pool sizing, dilution, 409A, Rule 701, or QSBS economics*? → **`startup-finance-fundraising-curriculum`.**
- Is it about *CoC transaction execution* (280G cleanse, tender-offer mechanics, closing allocation)? → **`startup-exit-curriculum`.**
- Is it about *offer-letter architecture, worker classification, or non-compete law*? → **mod-103.**
- Is it about the *process of hiring an executive* (search, panel, offer presentation)? → **mod-104.**
- Is it about *cash-comp bands, levels, or total-rewards benefits design*? → **mod-106.**
- Is it about *performance review, PIPs, RIFs, or IC separation agreements*? → **mod-107.**
- Is it about *pay-equity programs, DEI-weighted comp, or employee-wide comp communication*? → **mod-108.**
- Is it about *comp-data privacy, HRIS access control, or board-portal retention*? → **mod-110.**
- Is it about *the comp committee as a board committee, officer appointment, or D&O / indemnification*? → **mod-111.**
- Is it about *EPLI or D&O coverage* for exec-separation and CoC windows? → **mod-112.**
- Is it about *per-country equity sub-plans, EOR equity restrictions, or statutory severance abroad*? → **mod-113.**
- Is it about *Carta administrator operations, 83(b) filings, or cap-table reconciliation at the IC level*? → **`startup-people-ops-controllership`.**

## Summary

- This module owns the equity-compensation policy substance (grant guidelines, IC plan structure, refresh and promotion grants, exec comp, CoC equity, exec severance, Reg S-K Item 402 disclosure) and the compensation-committee operating infrastructure (charter, cadence, annual comp cycle).
- Its handoffs are precise: equity-comp economics to the fundraising-finance track; CoC transaction execution to the exit track; employment-law substance to mod-103; hiring process to mod-104; cash-comp and total rewards to mod-106; performance / IC-separation to mod-107; pay-equity and DEI to mod-108; privacy and HRIS access to mod-110; the comp committee as a board committee to mod-111; EPLI / D&O coverage to mod-112; international sub-plans to mod-113; IC-level equity administration to a future people-ops controllership track.
- The rule is simple: mod-105 owns the *policy substance* of what a grant, a package, or a committee decision should look like. Economics underneath, transaction execution, contract architecture, pipeline mechanics, benefits design, review instruments, privacy, board-committee operations, insurance, and international mechanics all live elsewhere.
- Get the boundary right and every adjacent module has a clean interface to the equity-comp decisions that drive so much of a startup's operating and economic behavior.
