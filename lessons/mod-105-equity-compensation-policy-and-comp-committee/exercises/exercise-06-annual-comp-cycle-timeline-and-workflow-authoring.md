# Exercise 06 — Annual comp cycle timeline and workflow authoring

> Estimated time: **~5 hours** · Related chapter: [06 — The annual comp cycle](../06-annual-comp-cycle.md)

## Problem statement

Lantern Signal, Inc. is a Delaware C-corp Series-B infrastructure-analytics company with ~140 employees distributed across seven states — California, Colorado, Washington, New York, Texas, Georgia, and Massachusetts. Fiscal year ends December 31. The 2024 comp cycle was run ad hoc: engineering, product, GTM, and G&A managers each emailed spreadsheets to the CPO over a six-week stretch in Q1 2025; the CPO manually reconciled them, the CEO rubber-stamped the merit pool, and grant notices went out piecemeal between early March and late April with no formal comp-committee resolution on file.

The $48M Series-B closed in Q3 2024. A standing compensation committee of the board was stood up at close (two independents plus the lead Series-B director). Compensia was retained in Q4 2024 as the corporation's independent compensation consultant and has delivered an initial market-data refresh keyed to the corporation's chosen peer group. The Head of People has been in seat since Q2 2024 and has made the 2025 cycle her top operating priority: it must be industrialised, calendar-driven, pay-transparency-compliant across all four regulated states, and leave a documentation trail that the pre-IPO audit team can rely on 18–24 months from now.

Your role: you are the Head of Total Rewards (or an outside operating advisor engaged by the Head of People) authoring the 2025 annual-comp-cycle playbook. Produce a dated cycle calendar, sized budgets, a stage-by-stage workflow with tooling, pay-transparency-compliant communications, calibration guardrails, and the documentation / audit-trail standard.

## Requirements

### Part A — Cycle calendar

Produce a dated cycle calendar for the 2025 annual comp cycle. Specify calendar dates (not relative "week-of" references) for every one of the following gates:

1. **Cycle kickoff** — the all-hands / all-manager communication launching the cycle, including the merit-budget envelope, the performance-review window, and the manager-training session dates.
2. **Performance-review conclusion deadline** — the date by which all performance reviews must be finalised so that comp recommendations are not being made against open ratings.
3. **Manager-recommendation deadline** — the date by which every manager submits merit, promotion, equity-refresh, and bonus recommendations in the tool.
4. **HRBP calibration windows** — functional-unit calibration sessions (engineering, product, GTM, G&A separately), with named facilitators.
5. **Leadership calibration** — the single cross-functional calibration with the CEO + exec team.
6. **Comp-committee review and resolution** — the formal committee meeting at which merit, equity, promotion, and executive comp are approved via written resolution.
7. **Comp-statement delivery to employees** — the window during which each employee receives their written compensation statement from their manager.
8. **Grant-notice issuance** — the date (or window) at which board-approved equity grants are papered and 83(b) windows begin.

Justify the sequencing against fiscal-year-end (Dec 31), the Q1 performance-review conclusion, Compensia's market-data refresh cadence, and the board's regular Q1 meeting cycle. Cross-reference [`../06-annual-comp-cycle.md`](../06-annual-comp-cycle.md) and [`../05-compensation-committee.md`](../05-compensation-committee.md).

### Part B — Size the budgets

Produce a sized budget envelope for the 2025 cycle. For each line, state the quantity, the dollar (or share) impact against Lantern Signal's current ~140-person base and fully-diluted cap table, and the market benchmark you are anchoring to. Flag every current-market benchmark number with `<!-- needs-research -->`.

1. **Merit budget** — stated as % of base-salary pool, with a split between standard-merit, market-adjustment, and promotion-merit sub-pools. Cite benchmark (WTW Salary Budget Planning Survey, Mercer Compensation Planning Survey, PayScale) with `<!-- needs-research -->`.
2. **Equity-refresh pool** — stated as % of fully-diluted shares, with a target annual-refresh envelope and a reserved tranche for retention / off-cycle. Cite benchmark (Carta State of Private Markets, Compensia practice note) with `<!-- needs-research -->`.
3. **Promotion budget** — stated as % of base-salary pool for promotion increases, with an expected promotion-rate assumption (e.g., target % of eligible population promoted per cycle). Cite benchmark with `<!-- needs-research -->`.
4. **Bonus-pool achievement factor** — if the corporation runs a corporate / individual bonus plan, the 2024-performance-based achievement factor as a % of target, with the corporate-performance inputs feeding it. Cross-reference [`../03-refresh-promotion-and-retention-grants.md`](../03-refresh-promotion-and-retention-grants.md).

### Part C — Workflow and tool stack

Produce the stage-by-stage workflow for a single comp recommendation moving from manager through comp-committee approval. Cover:

1. **Pipeline stages** — manager draft → HRBP functional calibration → leadership cross-functional calibration → comp-committee review → board resolution → statement delivery. Name the entry criteria and exit criteria for each stage.
2. **Tool stack** — the primary system of record (Pave, Lattice, CompTool, or HRIS-native Rippling / Gusto / Justworks), the market-data integration (Pave benchmark, Radford, Compensia pull), and the equity-grant system (Carta, Shareworks). Justify the chosen stack against the corporation's 140-employee / Series-B / pre-IPO stage.
3. **Data flow between stages** — what fields are populated by whom at each stage (current base, performance rating, proposed base, proposed grant, proposed bonus, promotion flag, retention flag), and how the data is locked between stages so late edits do not re-open closed decisions.
4. **Outlier-escalation path** — the explicit routing for recommendations that fall outside the guardrail set in Part E (e.g., >15% base increase, >2× typical refresh, out-of-cycle promotion, off-band hire-forward). Name the approver at each outlier tier.

### Part D — Pay-transparency-compliant communications

Produce the pay-transparency-compliant communications package. Cover:

1. **Written compensation statement** — the full field set every employee receives: current and new base, bonus target and 2024 actual, equity-refresh grant (shares, strike, vesting), total-rewards summary. State who signs the statement and the delivery mechanism.
2. **Interaction with state-specific job-posting ranges** — how the internal pay bands reconcile with the ranges the corporation posts externally in CA, CO, WA, and NY. Specifically address what happens when an employee's new base is below, inside, or above the posted range for their level. Cross-reference [`../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md`](../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md).
3. **Internal-equity question handling** — the manager script and the HRBP escalation path when an employee asks "am I paid fairly relative to my peers?" or "what is the band for my level?" Specify which questions the manager answers directly, which get escalated, and what the corporation will and will not disclose. Cross-reference [`../mod-103-employment-law-and-contract-design/08-state-law-variance.md`](../mod-103-employment-law-and-contract-design/08-state-law-variance.md).
4. **State-variance addendum** — a short per-state note (CA, CO, WA, NY) flagging the specific transparency obligation that applies to compensation-cycle communications (not just job postings) and whether 2024 or 2025 law changes affect the 2025 cycle. Flag unresolved items with `<!-- needs-research -->`.

### Part E — Calibration guardrails and rubric

Produce the explicit calibration rubric the HRBP uses in the Part A calibration windows. Cover:

1. **Tenure-anchored drift control** — the threshold at which a tenure-vs-pay or tenure-vs-equity outlier triggers calibration review (e.g., 90th-percentile tenure in band but <50th-percentile total comp).
2. **Performance-anchored drift control** — the threshold at which a performance-rating-vs-merit outlier triggers calibration review (e.g., top-rated employee receiving <median merit, or bottom-rated employee receiving above-median merit).
3. **Pay-equity-anchored drift control** — the gender / race / tenure-grouping threshold at which a pay-equity disparity triggers calibration review. State whether the corporation runs the pay-equity cut pre-cycle, mid-cycle, or both.
4. **The calibration rubric itself** — a tabular rubric listing (performance rating × band position × tenure band) and the expected merit / promotion / refresh outputs. Specify the override-with-justification path.
5. **Compensia's role** — where the retained consultant plugs into the calibration process (market-data refresh, exec-comp calibration, pay-equity audit, or all three).

### Part F — Documentation and audit trail

Produce the documentation and audit-trail standard the corporation will apply to the 2025 cycle. Cover:

1. **Comp-committee minutes retention** — the specific items captured in the written committee minutes (budget approval, merit-pool approval, equity-pool approval, exec-comp line items, dissents, abstentions). Cross-reference [`../05-compensation-committee.md`](../05-compensation-committee.md).
2. **HRBP calibration-notes retention** — what is captured per calibration session (attendees, outliers reviewed, overrides approved, pay-equity findings), and the retention location (HRIS, GRC tool, shared drive).
3. **Pre-IPO audit evidence base** — the artefact list that would satisfy an SOX-readiness or S-1-prep audit review in 2026 / 2027 (board resolutions, benchmark source files, calibration rosters, individual compensation statements, grant-notice packages).
4. **Access and privilege** — who inside the corporation can read comp-committee minutes, calibration notes, and the merit matrix, and the specific redactions applied for broader audiences.

## Starter guidance

- Chapter 06 is the primary reference. The chapter's four-stage cycle (plan → recommend → calibrate → approve) maps directly to Parts A and C.
- Compensia (or Radford, or Mercer — Compensia is the one named in the problem) typically delivers a market-data refresh on a Q4 cadence; the 2025 cycle calendar should respect that cadence rather than invent a schedule the consultant cannot support.
- The corporation has four pay-transparency states in-footprint (CA, CO, WA, NY). Treat MA as a 2025-watch state and Texas / Georgia as currently-unregulated for posting but still subject to federal EEOC / OFCCP obligations.
- Do not manufacture market numbers for merit %, refresh %, or promotion rate. Flag every one as `<!-- needs-research -->` and name the specific survey source the Head of Total Rewards will pull from.
- The 2024 ad-hoc cycle is the baseline the Head of People wants to replace, not a template to iterate on. Resist the urge to "preserve" ad-hoc practices for stakeholder comfort.
- The comp committee is new. Part A's cycle calendar should assume the committee needs 2–3 weeks of lead time before its first substantive meeting on the 2025 cycle — not a 48-hour turnaround.

## Deliverables

- `cycle-calendar-2025.md` — Part A (dated calendar + sequencing justification).
- `cycle-budgets-2025.md` — Part B (merit, refresh, promotion, bonus pools with `<!-- needs-research -->` markers).
- `cycle-workflow-and-tools.md` — Part C (pipeline, tool stack, data flow, escalation).
- `pay-transparency-communications-package.md` — Part D (statement, state addendum, manager script).
- `calibration-guardrails-and-rubric.md` — Part E (drift controls + rubric table).
- `documentation-and-audit-trail-standard.md` — Part F (minutes, notes, audit evidence, access).

## Acceptance criteria

The package is acceptable if:

1. Part A names specific calendar dates (month and day, not "week-of") for every one of the eight gates listed and justifies the sequencing against fiscal-year-end, Q1 performance-review conclusion, Compensia's market-data cadence, and the board's regular Q1 meeting.
2. Part B states a specific budget-allocation plan (merit %, refresh %, promotion %, bonus achievement factor) with `<!-- needs-research -->` flags on every current-market benchmark cited.
3. Part C names the tool stack (one primary comp tool, one market-data source, one equity-grant system) and specifies entry / exit criteria for each pipeline stage plus the outlier-escalation routing.
4. Part D includes a written compensation-statement field list, a specific reconciliation rule for each of CA / CO / WA / NY posted-range interactions, and a manager script for internal-equity questions.
5. Part E includes an explicit tabular calibration rubric (performance × band position × tenure) and three named drift controls (tenure, performance, pay-equity) with thresholds.
6. Part F names the specific artefacts retained at the committee, HRBP, and audit-evidence levels, and the access / redaction rule for each.
7. All five cross-references (chapter 06, chapter 05, chapter 03, mod-103 chapter 03, mod-103 chapter 08) are present and linked relatively.
8. Every current-market benchmark number is flagged with `<!-- needs-research -->`; no benchmark is asserted as current without the marker.
9. Nothing left as `[TBD]` or `[FILL IN]`.
