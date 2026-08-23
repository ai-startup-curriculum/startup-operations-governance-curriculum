# mod-106 — Compensation Architecture & Total Rewards

> Job architecture, leveling, cash-and-equity bands by geography, benchmarking, the annual comp cycle, pay transparency, benefits, sales comp, and the failure modes that eat comp systems from the inside.

**Track:** Startup Operations & Governance (level 50) · **Stage:** SEED / SERIES-A / SERIES-B / GROWTH · **Pillar:** people-ops · **Hours:** 30

## Why this module exists

[mod-104](../mod-104-hiring-onboarding-and-hr-operations/) built the hiring pipeline and the HRIS / PEO stack that runs payroll and benefits enrollment. [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/) authored the equity-compensation policy — grant guidelines, refresh cadence, the compensation-committee charter, and the 409A cadence that governs strike prices. Neither of those modules answers the question this module owns: **for a given hire, what should the cash-and-equity offer actually be, and how do we produce a defensible answer at scale?**

That question decomposes into six operating decisions:

1. **A job architecture and leveling framework.** Function tracks (Engineering, Product, Design, Data / ML, Sales, Marketing, CS, Ops, Finance, People, Legal), a parallel IC and manager ladder inside each track, distinguishable level definitions (autonomy, scope, complexity, impact), and the leveling-calibration norms that keep the framework from drifting across functions or across time.
2. **A cash-and-equity band per level per geography.** A tiered geographic pay strategy (national / tier-1-and-national / tiered by cost-of-labor / cost-of-living / competitive-market / anchored to top-quartile / median / 60th-percentile), a band width (typically 20–40%) with a midpoint target, and a compression-and-inversion diagnostic.
3. **A benchmarking data source appropriate to the stage.** Carta and Pave at seed → Series-B; Radford and Compensia at Series-B → growth; and modelling tools (Figures, Pequity, Assemble) for band management and comp-cycle execution.
4. **An annual comp cycle.** Timing (typically Q1 after fiscal close), a merit / equity-refresh / promotion budget-allocation across functions and levels, a manager → HRBP → executive → comp-committee review workflow, a compensation-statement communications pattern, and an annual comp-cycle retrospective feedback loop.
5. **A pay-transparency-compliance posture.** Colorado, California, New York City / New York State, Washington, Illinois, and the fast-growing state-and-city adoption plus the EU Pay Transparency Directive (transposed by 2026-06-07) — comp-band publication, comp-decision-audit-trail requirements, gender-pay-gap reporting.
6. **A total-rewards package.** Health / dental / vision (broker vs. self-insured), 401(k) with match and vesting, commuter, parental leave, stipends (WFH / L&D / wellness), FSA / HSA / LSA, and the exec-perk overlay.

Two additional problem-spaces sit inside the module for coverage but *not* ownership:

- **The sales-comp plan** — quota-based OTE, accelerators / decelerators, ramp comp, spiffs, clawback. This module owns the *general-compensation-architecture side* (how sales comp fits into the leveling / bands / cycle machinery). The GTM-instrument side — quota-setting philosophy, territory design, comp-plan-as-behaviour-shaper — sits in `startup-product-gtm-curriculum`.
- **Comp-architecture failure modes** — level compression, tenure-vs-performance drift, cross-function inversion, promotion-inflation, geographic-arbitrage drift. Recognising and prescribing fixes for each.

Get the architecture right and the corporation makes hire-by-hire decisions in minutes with a defensible answer, passes Series-B / Series-C people diligence on comp cleanly, meets pay-transparency-law obligations across every jurisdiction it employs someone, and keeps top performers without a special-case retention spiral. Get it wrong and every hire is a bespoke negotiation, level compression prices a great engineer out at renewal, a Colorado job posting missing the pay range triggers a Division of Labor complaint, the EU salaried employees discover the sales BDR's OTE is higher than the senior engineer's total cash, and the board's compensation committee starts asking questions no one in the room can answer.

## Chapters

1. [Job architecture and the leveling framework](./01-job-architecture-and-leveling-framework.md) — function tracks, IC / manager parallel ladders, competency-based level definitions, and the leveling-calibration norms that keep drift out.
2. [Cash-and-equity bands per level per geography](./02-cash-and-equity-bands-per-level-per-geography.md) — the tiered geographic pay-strategy decision, band-width design (20–40%, midpoint-target), and the compression-and-inversion diagnostic.
3. [Benchmarking data sources by stage](./03-benchmarking-data-sources-by-stage.md) — Carta / Pave at seed → Series-B, Radford / Compensia at Series-B → growth, band-management tooling (Figures, Pequity, Assemble), and the sample-size trigger for supplementation.
4. [The annual comp cycle](./04-annual-comp-cycle.md) — timing anchor, budget allocation, the manager → HRBP → executive → comp-committee workflow, comp-statement communications, and the annual retrospective.
5. [Pay-transparency compliance across states and the EU](./05-pay-transparency-compliance.md) — Colorado, California, NYC / NY State, Washington, Illinois, other adopting jurisdictions, and the EU Pay Transparency Directive (Directive (EU) 2023/970).
6. [Total-rewards package design](./06-total-rewards-package-design.md) — health / dental / vision, 401(k), commuter, parental leave, stipends, FSA / HSA / LSA, and the exec-perk overlay.
7. [Sales-comp plan design (in coordination with GTM)](./07-sales-comp-plan-design.md) — quota-based OTE, accelerators / decelerators, ramp comp, spiff design, clawback design — with the ownership-boundary carveout back to `startup-product-gtm-curriculum`.
8. [Comp-architecture failure modes and their fixes](./08-comp-architecture-failure-modes.md) — level compression, tenure-vs-performance drift, cross-function inversion, promotion inflation, geographic-arbitrage drift.
9. [Ownership boundary map](./09-ownership-boundary-map.md) — what this module owns vs. what it hands off to mod-104, mod-105, mod-107, mod-113, `startup-product-gtm-curriculum`, `startup-finance-fundraising-curriculum` mod-111, and `cto-curriculum`.

## Exercises

- [exercise-01 — Job architecture and leveling framework authoring](./exercises/exercise-01-job-architecture-and-leveling-framework-authoring.md)
- [exercise-02 — Cash and equity band authoring by geography](./exercises/exercise-02-cash-and-equity-band-authoring-by-geography.md)
- [exercise-03 — Benchmarking source selection by stage](./exercises/exercise-03-benchmarking-source-selection-by-stage.md)
- [exercise-04 — Annual comp cycle workflow and communications](./exercises/exercise-04-annual-comp-cycle-workflow-and-communications.md)
- [exercise-05 — Pay transparency compliance across states and EU](./exercises/exercise-05-pay-transparency-compliance-across-states-and-eu.md)
- [exercise-06 — Total rewards package design and benefits broker decision](./exercises/exercise-06-total-rewards-package-design-and-benefits-broker-decision.md)
- [exercise-07 — Sales comp plan design in coordination with GTM](./exercises/exercise-07-sales-comp-plan-design-in-coordination-with-gtm.md)
- [exercise-08 — Comp architecture failure teardown and fix](./exercises/exercise-08-comp-architecture-failure-teardown-and-fix.md)

## Resources

- [resources.md](./resources.md) — federal and state pay-transparency statutes, the EU Pay Transparency Directive, ERISA / IRC benefits provisions, and benchmarking-provider documentation cited across the chapters.

## Ownership boundary (quick reference)

This module owns the **compensation-architecture and total-rewards** layer. It hands off:

- **Equity-compensation policy substance** (grant-guideline authoring, refresh cadence, the compensation-committee charter, the 409A cadence) → [mod-105 — Equity-Compensation Policy & the Compensation Committee](../mod-105-equity-compensation-policy-and-comp-committee/).
- **Benefits-broker and PEO selection / operating machinery** (broker interview, PEO-vs.-HRIS graduation, HRIS open enrollment mechanics) → [mod-104 chapter 07](../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md).
- **Performance ratings, calibration, and promotion decisions** (the calibration meeting that feeds the comp cycle's merit budget) → [mod-107 — Performance, Promotion & Offboarding](../mod-107-performance-promotion-and-offboarding/).
- **GTM-role comp plans as an incentive instrument** (quota-setting philosophy, territory design, plan-as-behaviour-shaper) → `startup-product-gtm-curriculum`.
- **Engineering-track leveling nuances** (E1 → E7 competencies, dual-ladder policy) → `cto-curriculum`.
- **Finance-org comp benchmarks the CFO owns** (Controller / VP Finance / CAO / Head of FP&A) → `startup-finance-fundraising-curriculum` mod-111.
- **International compensation** (per-country pay-transparency, per-country benefits, EOR-priced comp) → [mod-113 — International Expansion & Global Workforce](../mod-113-international-expansion-and-global-workforce/).

See [chapter 09](./09-ownership-boundary-map.md) for the full boundary map.

## Prerequisites

- [mod-103 — Employment Law, Worker Classification & Contract Design](../mod-103-employment-law-and-contract-design/) — the offer letter, the FLSA exempt / non-exempt classification, and the pay-transparency clauses the offer letter must satisfy.
- [mod-104 — Hiring, Onboarding & HR Operations](../mod-104-hiring-onboarding-and-hr-operations/) — the hiring pipeline that consumes the bands the module produces, and the HRIS / PEO / broker stack that operates the benefits programme.
- [mod-105 — Equity-Compensation Policy & the Compensation Committee](../mod-105-equity-compensation-policy-and-comp-committee/) — the equity side of the offer, the grant-guideline framework, and the compensation-committee governance.
- Comfort reading state statutes, EEOC guidance, ERISA regulations, and benchmarking-provider methodology documentation.

## What "done" looks like

By the end of this module you can, for a hypothetical multi-stage company, produce and defend:

1. A job architecture and leveling framework — function tracks, an IC / manager parallel ladder, level definitions with distinguishable competencies, and the calibration-norm playbook.
2. A cash-and-equity band per level per geography — a tiered geographic strategy, band widths, midpoint targets, and a compression / inversion diagnostic on the current comp file.
3. A benchmarking-source selection decision by stage — Carta / Pave at seed → Series-B, Radford / Compensia at Series-B → growth, plus the band-management-tool selection.
4. An annual comp-cycle operating plan — timing, budget allocation, workflow, comp-statement templates, and a retrospective instrument.
5. A pay-transparency-compliance posture across every state / city the corporation employs someone in, plus the EU Pay Transparency Directive readiness plan (by 2026-06-07).
6. A total-rewards package design — plan design, contribution strategy, 401(k) design, parental leave, stipend suite, and exec-perk overlay.
7. A sales-comp plan aligned with the corporation's GTM model, with the ownership-boundary handoff to `startup-product-gtm-curriculum` clearly marked.
8. A comp-architecture failure-mode teardown for a specific corporation's current comp file, with a prescribed fix for each failure mode.
9. A defensible ownership-boundary map — "does this comp question belong here, in mod-104, mod-105, mod-107, mod-113, GTM, finance, or CTO?"
