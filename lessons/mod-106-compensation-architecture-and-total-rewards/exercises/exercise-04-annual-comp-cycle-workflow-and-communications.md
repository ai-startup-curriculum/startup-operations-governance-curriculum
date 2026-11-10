# Exercise 04 — Annual comp cycle workflow and communications

> Estimated time: **~5 hours** · Related chapter: [04 — The annual comp cycle](../04-annual-comp-cycle.md)

## Problem statement

Marigold Compute, Inc. is a Delaware C-corp building a model-serving and GPU-scheduling platform for mid-market AI teams. The corporation closed a $110M Series-B thirteen months ago and is actively indexed as a Series-C target. Headcount is **240 employees** across eight US states (CA, CO, WA, NY, IL, TX, MA, GA) and a London satellite (11 UK employees via a UK Ltd. subsidiary spun up six months ago). Fiscal year ends December 31.

Current state of the comp cycle:

- **The 2025 comp cycle was run ad hoc** — each function lead emailed spreadsheets to the Head of People across a seven-week Q1 2025 window; the Head of People reconciled by hand; the founder-CEO approved in a single sit-down; equity-refresh notices went out between early March and late April with three separate board-resolution packages. No comp-committee written resolution covered the full merit / promotion / refresh cycle; only the exec-comp line items went through the committee.
- **The compensation committee** was stood up at Series-B close (two independent directors plus the lead Series-B director; the independent chair is a public-company CFO with pre-IPO experience). The committee ratified the grant guideline (`[mod-105 chapter 01](../../mod-105-equity-compensation-policy-and-comp-committee/01-grant-guidelines-by-level-and-function.md)`), the comp-committee charter ([mod-105 chapter 05](../../mod-105-equity-compensation-policy-and-comp-committee/05-compensation-committee.md)), and the band file (from [exercise 02](./exercise-02-cash-and-equity-band-authoring-by-geography.md)) in Q3 and Q4 2025 respectively.
- **The benchmarking stack** — Pave as primary, Radford Global Technology Survey added at Series-B close, Compensia retained for the comp-committee advisory and exec-comp calibration — was ratified under [exercise 03](./exercise-03-benchmarking-source-selection-by-stage.md).
- **The 2026 cycle** must be industrialised, calendar-driven, pay-transparency-compliant across every state in-footprint and under the EU Pay Transparency Directive for the UK subsidiary (noting the Directive applies to EU member states directly; the UK's post-Brexit position is handled separately `<!-- needs-research: current UK pay-transparency statutory position and whether UK Ltd. with no EEA workers is subject to any directive-equivalent -->`), and leave an audit-trail the Series-C process can rely on.
- **Known forcing functions for the 2026 cycle:**
    1. A 25-person 2026 hiring plan (10 engineering, 4 product, 7 GTM, 4 G&A) sits on top of the cycle's merit and refresh budgets.
    2. A Series-C close targeted in Q2 2026; the diligence team will ask for the 2025 and 2026 cycle documentation.
    3. Three pay-transparency statute updates adopted in 2025 that take effect during the 2026 cycle window (`<!-- needs-research: specific state-statute effective dates that fall inside the 2026 Q1 cycle window -->`).
    4. The UK subsidiary's first annual UK employment-law-driven pay statement, due inside the 2026 cycle window.

Your role: you are the **Head of Total Rewards** (the role split out from Head of People at Series-B close) authoring the 2026 annual-comp-cycle playbook. Produce a dated cycle calendar, sized budgets, the stage-by-stage workflow with tooling, the pay-transparency-compliant communications package, the calibration rubric with drift controls, and the documentation / audit-trail standard.

## Requirements

### Part A — Cycle calendar

Produce a dated cycle calendar for the 2026 annual comp cycle. Specify calendar dates (month and day, not "week-of") for every one of the following gates:

1. **Cycle kickoff** — the all-hands / all-manager communication launching the cycle, including the merit-budget envelope, the performance-review window, and the manager-training session dates.
2. **Performance-review conclusion deadline** — the date by which all performance reviews must be finalised so that comp recommendations are not being made against open ratings. Cross-reference [mod-107 chapter 01](../../mod-107-performance-promotion-and-offboarding/01-performance-management-operating-system.md) for the performance-management operating-system.
3. **Manager-recommendation deadline** — the date by which every manager submits merit, promotion, equity-refresh, and bonus recommendations in the tool.
4. **HRBP calibration windows** — functional-unit calibration sessions (engineering, product, GTM, G&A separately), with named facilitators.
5. **Leadership calibration** — the single cross-functional calibration with the CEO + exec team.
6. **Comp-committee review and resolution** — the formal committee meeting at which merit, equity, promotion, and executive comp are approved via written resolution. Cross-reference [mod-105 chapter 05](../../mod-105-equity-compensation-policy-and-comp-committee/05-compensation-committee.md).
7. **Board ratification** — the full-board meeting at which the comp-committee recommendations are ratified (the equity grants require full-board or committee-delegated authority under the equity plan).
8. **Comp-statement delivery window** — the window during which each employee receives their written compensation statement from their manager.
9. **Grant-notice issuance** — the date (or window) at which board-approved equity grants are papered and 83(b) windows begin.
10. **Pay-transparency reconciliation gate** — the date by which externally posted pay ranges (CA, CO, WA, NY, IL, and any 2026-effective statute) are reconciled with the newly ratified bands.

Justify the sequencing against fiscal-year-end (Dec 31), the Q1 performance-review conclusion, Compensia's market-data refresh cadence (`<!-- needs-research -->`), the board's regular Q1 meeting cycle, the three 2026-effective pay-transparency updates, and the Series-C-process timing.

### Part B — Size the budgets

Produce a sized budget envelope for the 2026 cycle. For each line, state the quantity, the dollar (or share) impact against Marigold's current 240-person base and fully-diluted cap table, and the market benchmark you are anchoring to. Flag every current-market benchmark number with `<!-- needs-research -->`.

1. **Merit budget** — stated as % of base-salary pool, with a split between standard-merit, market-adjustment (to address 2025-cycle below-band retention cases), and promotion-merit sub-pools. Cite benchmark (WTW Salary Budget Planning Survey, Mercer Compensation Planning Survey, PayScale) with `<!-- needs-research -->`.
2. **Equity-refresh pool** — stated as % of fully-diluted shares, with a target annual-refresh envelope and a reserved tranche for retention / off-cycle. Cite benchmark (Carta State of Private Markets, Compensia practice note) with `<!-- needs-research -->`. Cross-reference [mod-105 chapter 03](../../mod-105-equity-compensation-policy-and-comp-committee/03-refresh-promotion-and-retention-grants.md) for the refresh / promotion / retention mechanics.
3. **Promotion budget** — stated as % of base-salary pool for promotion increases, with an expected promotion-rate assumption (e.g., target % of eligible population promoted per cycle). Cite benchmark with `<!-- needs-research -->`.
4. **Bonus-pool achievement factor** — the 2025-performance-based achievement factor as a % of target, with the corporate-performance inputs (revenue vs. plan, gross-margin vs. plan, net-dollar retention vs. plan) feeding it.
5. **The 25-hire interaction.** State the pool reservation for new-hire grants under the 25-person 2026 hiring plan, and the interaction with the equity-refresh envelope — chapter 04 notes that an undersized new-hire reservation forces mid-cycle off-cycle grants; an oversized reservation under-allocates the refresh pool.

### Part C — Workflow and tool stack

Produce the stage-by-stage workflow for a single comp recommendation moving from manager through board ratification. Cover:

1. **Pipeline stages** — manager draft → HRBP functional calibration → leadership cross-functional calibration → comp-committee review → board resolution → statement delivery. Name the entry criteria and exit criteria for each stage.
2. **Tool stack** — the primary system of record (Pave is the ratified choice from [exercise 03](./exercise-03-benchmarking-source-selection-by-stage.md)), the performance-management-system hand-off (Lattice or 15Five — cross-reference [mod-107](../../mod-107-performance-promotion-and-offboarding/)), the market-data integrations, and the equity-grant system (Carta or Shareworks). Cross-reference [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md) for the HRIS integration.
3. **Data flow between stages.** State what fields are populated by whom at each stage (current base, performance rating, proposed base, proposed grant, proposed bonus, promotion flag, retention flag, PIP-flag from [mod-107 chapter 04](../../mod-107-performance-promotion-and-offboarding/04-pip-mechanics.md)), and how the data is locked between stages so late edits do not re-open closed decisions.
4. **Outlier-escalation path.** The explicit routing for recommendations that fall outside the Part E guardrails (e.g., >15% base increase, >2× typical refresh, out-of-cycle promotion, off-band hire-forward). Name the approver at each outlier tier.
5. **The mid-cycle-retention-request route.** State how an off-cycle retention grant proposed during the cycle window is routed differently than a within-cycle recommendation, and how the retention grant is reconciled against the within-cycle plan for the same IC.

### Part D — Pay-transparency-compliant communications

Produce the pay-transparency-compliant communications package. Cover:

1. **Written compensation statement.** The full field set every employee receives: current and new base, bonus target and 2025 actual, equity-refresh grant (shares, strike, vesting), total-rewards summary, and the manager's written rationale for any above-band or below-band exception. State who signs the statement and the delivery mechanism.
2. **Interaction with state-specific job-posting ranges.** How the internal pay bands reconcile with the ranges the corporation posts externally in CA, CO, WA, NY, IL, and any state with a 2026-effective statute. Specifically address what happens when an employee's new base is below, inside, or above the posted range for their level. Cross-reference [mod-103 chapter 03](../../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md) and [chapter 05](../05-pay-transparency-compliance.md).
3. **Internal-equity question handling.** The manager script and the HRBP escalation path when an employee asks "am I paid fairly relative to my peers?" or "what is the band for my level?" Specify which questions the manager answers directly, which get escalated, and what the corporation will and will not disclose — noting the NLRA § 7 protected-concerted-activity backdrop that bars retaliating against employees for discussing pay (cross-reference [mod-103](../../mod-103-employment-law-and-contract-design/)).
4. **UK-subsidiary pay-statement addendum.** The UK employment-law-driven pay statement due inside the cycle window — the specific UK statutory requirements (`<!-- needs-research -->`), the delivery mechanism, and the reconciliation against the US-template statement.
5. **State-variance addendum.** A short per-state note (CA, CO, WA, NY, IL, and any 2026-effective statute) flagging the specific transparency obligation that applies to compensation-cycle communications (not just job postings) and whether 2025 or 2026 law changes affect the 2026 cycle. Flag unresolved items with `<!-- needs-research -->`.

### Part E — Calibration rubric and drift controls

Produce the explicit calibration rubric the HRBP uses in the Part A calibration windows. Cover:

1. **Tenure-anchored drift control.** The threshold at which a tenure-vs-pay or tenure-vs-equity outlier triggers calibration review (e.g., 90th-percentile tenure in band but <50th-percentile total comp).
2. **Performance-anchored drift control.** The threshold at which a performance-rating-vs-merit outlier triggers calibration review (e.g., top-rated employee receiving <median merit, or bottom-rated employee receiving above-median merit).
3. **Pay-equity-anchored drift control.** The gender / race / tenure-grouping threshold at which a pay-equity disparity triggers calibration review. State whether the corporation runs the pay-equity cut pre-cycle, mid-cycle, or both, and state the attorney-client-privilege wrapper the pay-equity audit runs under (the audit output is protected work-product; cross-reference [mod-103](../../mod-103-employment-law-and-contract-design/) and the GC).
4. **The calibration rubric itself.** A tabular rubric listing (performance rating × band position × tenure band) and the expected merit / promotion / refresh outputs. Specify the override-with-justification path.
5. **Compensia's role.** Where the retained consultant plugs into the calibration process (market-data refresh, exec-comp calibration, pay-equity audit, or all three).

### Part F — Documentation and audit-trail standard

Produce the documentation and audit-trail standard the corporation will apply to the 2026 cycle. Cover:

1. **Comp-committee minutes retention.** The specific items captured in the written committee minutes (budget approval, merit-pool approval, equity-pool approval, exec-comp line items, dissents, abstentions). Cross-reference [mod-105 chapter 05](../../mod-105-equity-compensation-policy-and-comp-committee/05-compensation-committee.md).
2. **HRBP calibration-notes retention.** What is captured per calibration session (attendees, outliers reviewed, overrides approved, pay-equity findings), and the retention location (HRIS, GRC tool, shared drive).
3. **Series-C diligence evidence base.** The artefact list that would satisfy the Series-C process in Q2 2026 (board resolutions, benchmark source files, calibration rosters, individual compensation statements, grant-notice packages, pay-equity audit output under privilege).
4. **Access and privilege.** Who inside the corporation can read comp-committee minutes, calibration notes, and the merit matrix, and the specific redactions applied for broader audiences.
5. **The retention window.** State the retention window for each artifact (comp-committee minutes retained indefinitely; individual compensation statements retained per employment-record retention norms with cross-reference to `startup-finance-fundraising-curriculum` and [mod-104](../../mod-104-hiring-onboarding-and-hr-operations/) for the HRIS retention policy).

## Starter guidance

- Chapter 04 is the primary reference. The chapter's four-stage cycle (plan → recommend → calibrate → approve) maps directly to Parts A and C. Re-read the "cycle calendar," "budget sizing," "workflow," "communications," "calibration," and "audit-trail" sections before authoring.
- The 2025 ad-hoc cycle is the baseline the Head of People wants to replace, not a template to iterate on. Resist the urge to "preserve" ad-hoc practices for stakeholder comfort.
- Compensia typically delivers a market-data refresh on a Q4 cadence (`<!-- needs-research -->`); the 2026 cycle calendar should respect that cadence rather than invent a schedule the consultant cannot support.
- The corporation has five pay-transparency statutes in-footprint today (CA, CO, WA, NY, IL) plus the UK subsidiary and any 2026-effective state statutes; treat MA as a watch state and the EU Pay Transparency Directive as the forward-looking regime for any future EEA hires.
- **Do not manufacture market numbers for merit %, refresh %, or promotion rate.** Flag every one as `<!-- needs-research -->` and name the specific survey source the Head of Total Rewards will pull from.
- The Series-C process in Q2 2026 is the forcing function for the audit-trail standard in Part F. Treat the artifact list as a diligence-response pre-stage, not a documentation-for-documentation's-sake exercise.

## Deliverables

- `cycle-calendar-2026.md` — Part A (dated calendar + sequencing justification).
- `cycle-budgets-2026.md` — Part B (merit, refresh, promotion, bonus pools, new-hire-reservation interaction, with `<!-- needs-research -->` markers).
- `cycle-workflow-and-tools.md` — Part C (pipeline, tool stack, data flow, escalation, mid-cycle-retention route).
- `pay-transparency-communications-package.md` — Part D (statement, state addendum, UK addendum, manager script).
- `calibration-rubric-and-drift-controls.md` — Part E (drift controls + rubric table).
- `documentation-and-audit-trail-standard.md` — Part F (minutes, notes, Series-C evidence, access, retention).

## Acceptance criteria

The package is acceptable if:

1. Part A names specific calendar dates (month and day, not "week-of") for every one of the ten gates listed and justifies the sequencing against fiscal-year-end, Q1 performance-review conclusion, Compensia's market-data cadence, the board's Q1 meeting, the 2026-effective pay-transparency updates, and the Series-C process.
2. Part B states a specific budget-allocation plan (merit %, refresh %, promotion %, bonus achievement factor, new-hire reservation) with `<!-- needs-research -->` flags on every current-market benchmark cited.
3. Part C names the tool stack (Pave primary, PM-system hand-off, equity-grant system), specifies entry / exit criteria for each pipeline stage, specifies the outlier-escalation routing, and specifies the mid-cycle-retention route.
4. Part D includes a written compensation-statement field list, a specific reconciliation rule for each of CA / CO / WA / NY / IL posted-range interactions plus the UK-subsidiary pay statement, and a manager script for internal-equity questions with the NLRA § 7 backdrop.
5. Part E includes an explicit tabular calibration rubric (performance × band position × tenure) and three named drift controls (tenure, performance, pay-equity) with thresholds and the attorney-client-privilege wrapper on the pay-equity audit.
6. Part F names the specific artefacts retained at the committee, HRBP, and Series-C-diligence-evidence levels, the access / redaction rule for each, and the retention window per artifact.
7. Cross-references to [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md), [chapter 03](../03-benchmarking-data-sources-by-stage.md), [chapter 05](../05-pay-transparency-compliance.md), [mod-103 chapter 03](../../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md), [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md), [mod-105 chapter 03](../../mod-105-equity-compensation-policy-and-comp-committee/03-refresh-promotion-and-retention-grants.md), [mod-105 chapter 05](../../mod-105-equity-compensation-policy-and-comp-committee/05-compensation-committee.md), [mod-107 chapter 01](../../mod-107-performance-promotion-and-offboarding/01-performance-management-operating-system.md), and [mod-107 chapter 04](../../mod-107-performance-promotion-and-offboarding/04-pip-mechanics.md) are present.
8. Every current-market benchmark number and every statute-specific effective-date claim is flagged with `<!-- needs-research -->`; no benchmark is asserted as current without the marker.
9. Nothing left as `[TBD]` or `[FILL IN]`.
