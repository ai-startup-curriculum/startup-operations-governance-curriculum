# Exercise 01 — Job architecture and leveling framework authoring

> Estimated time: **~5 hours** · Related chapter: [01 — Job architecture and the leveling framework](../01-job-architecture-and-leveling-framework.md)

## Problem statement

Perihelion Data Systems, Inc. is a Delaware C-corp building a streaming-ingest and governance platform for regulated-industry data warehouses. The corporation closed a $32M Series-A fourteen months ago and is expected to open the Series-B process in the next two quarters. Headcount is **96 employees**: 42 engineering (18 product-engineering, 9 platform / infra, 6 data-engineering, 5 security, 4 applied-research for a new foundation-model-assisted schema-mapping capability), 8 product / design, 24 GTM (12 AE / SE, 5 CS, 4 marketing, 3 sales operations), 15 G&A (6 finance, 2 legal, 5 people, 2 IT), and 7 operations / support.

Current state of the people system:

- **No ratified job architecture.** Titles have accreted over three years of hiring. There are two "Senior Engineers," one "Lead Engineer," one "Staff Engineer," one "Principal Engineer, Platform," and one "Lead Software Architect" on the engineering org chart. The Head of Engineering cannot defensibly say which of those six are peers and which are not.
- **The founder-CEO still signs every offer** and still makes the base-cash and equity-sizing call in a Slack thread with the hiring manager roughly forty minutes before the offer letter is sent.
- **No promotion machinery.** Two engineers were promoted in the last cycle (the Head of Engineering described them in a one-line summary to the CEO); one was given the title "Staff Engineer" and a 14% base bump, the other was given the title "Senior Engineer II" and an 11% base bump with a 3,000-share refresh. No written criteria were consulted; no committee met.
- **Cross-function friction is surfacing.** At a joint quarterly planning meeting last week, a "Senior Product Manager" claimed scope parity with a "Staff Engineer" on a shared initiative. The Head of Engineering disagreed on the floor of the meeting. The Head of Product and the Head of Engineering have since spent two Slack threads arguing about what the equivalence should be.
- **A pay-transparency incident is pending.** A Colorado job posting the recruiting coordinator published eight days ago for a "Senior Engineer, Data Infrastructure" carries a pay range the Head of People now believes is below the band the Head of Engineering would have authored if asked. The Head of People has paused new Colorado postings pending resolution.
- **The Series-B diligence dry-run** the prospective lead investor's operating partner ran three weeks ago surfaced "no leveling framework, no band-to-level map, no calibration record" as a Severity-2 finding.

Your role: you are the **Head of People** (title not yet upgraded to Head of Total Rewards — that split is scheduled for the Series-B close) tasked with authoring the first ratifiable job architecture for Perihelion. Produce the track inventory and ratification decisions, the IC-and-manager parallel ladder, the level rubric, the calibration-norm playbook, and the comp-committee presentation memo that moves the architecture from draft to ratified state before the Series-B diligence re-engages.

## Requirements

### Part A — Function-track inventory and ratification decisions

Produce a written track inventory the comp committee can ratify in one sitting. Cover:

1. **The track list.** Enumerate the function tracks Perihelion will stand up at ratification. At minimum: Engineering, Product, Design, Data / ML, GTM (AE / SDR / SE / Sales Management sub-ladders), Marketing, Customer Success, Operations, Finance, People, Legal. For each, state whether the track exists today (named ICs in-seat), is forward-authored (no ICs yet but hiring is imminent), or is deferred (no hiring plan this cycle).
2. **The own-track vs. parent-track decision for the four-person applied-research team.** The current four research ICs sit inside Engineering with the title "Engineer, Applied Research." Chapter 01 names the two-part test (does the hiring market and competency expectation differ meaningfully from the parent track?). Apply the test and state the decision with rationale. Flag any market claim with `<!-- needs-research -->`.
3. **The ratification path.** Name the body that ratifies each new track (leveling council described in Part D), the required inputs (function-leader-supplied competency draft, Head-of-People-supplied draft rubric, market-data note where relevant), and the quorum / approval rule. Cross-reference [chapter 01](../01-job-architecture-and-leveling-framework.md) and the compensation-committee charter work at [mod-105 chapter 05](../../mod-105-equity-compensation-policy-and-comp-committee/05-compensation-committee.md).
4. **The off-ladder role inventory.** Identify roles that do not sit on a function track (Chief of Staff, Executive Assistant, Founder-office roles, Board Advisor / EIR slots). State the convention — these roles are *explicitly* off-ladder, priced individually, and documented as such in the leveling librarian's master document — so that future hires in these roles do not get retroactively placed on a track whose shape does not fit them.

### Part B — IC and manager parallel ladders

Author the dual-ladder convention Perihelion will adopt. Cover:

1. **IC-ladder height.** State the full IC-ladder height — E1 new-grad through E7 Fellow — for Engineering, and the parallel ladders (P, D, DS / MLE, F, HR, L, BO, GTM) with their heights. For any ladder that currently has an unfilled top tier (e.g., Perihelion has no E7 and no P6 today), state why the tier is authored anyway and the compression-trap rationale from chapter 01.
2. **Manager-premium vs. manager-parity decision.** Pick one convention and justify it. The decision must be stated at the band-midpoint level (e.g., "a first-line engineering manager M4 sits at the E4–E5 midpoint with the midpoint closer to E5") and must be documented as reviewable only at the annual revision cadence.
3. **The specific IC-to-manager equivalence claim.** State, in a short table, the peer-tier claim across the ladders: E6 = M5 = D1 in cash and equity; E7 = VP peer; P5 = E5; D5 = E5; MLE5 = E5; etc. For each equivalence claim that is not already supported by in-seat ICs at both tiers, flag with `<!-- needs-research -->` for the market-data check that must happen at band authoring in [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md).
4. **The two already-promoted Engineers.** Reconcile the two mid-cycle promotions (one to "Staff Engineer," one to "Senior Engineer II") against the newly authored ladder. For each, state the level the IC *should* be at under the ratified rubric in Part C, and state the retroactive-reconciliation disposition (no change, title-only change, title-and-band change) and the communication script the Head of Engineering will use with the IC.

### Part C — Level rubric

Produce the level rubric that lets the calibration committee place any current or future IC at exactly one level. Cover:

1. **The four-dimension rubric.** For each level in the Engineering IC ladder (E1 through E7) and for each level in the Product, Design, Data / ML, and People ladders Perihelion stands up today, write a short definition against the four dimensions (scope, complexity, autonomy, impact) borrowed from chapter 01. Keep each definition to 2–4 lines; the goal is a committee-readable rubric, not an HR-compendium entry.
2. **The GTM ladder exception.** State that GTM levels are role-named (AE / Senior AE / Enterprise AE / Strategic AE; SDR / Senior SDR / SDR Manager; SE1 / SE2 / Senior SE; Sales Manager / Director / VP / CRO) and that the dimensions carry different weights (deal complexity, quota segment, named-account mechanics). Cross-reference [`startup-product-gtm-curriculum`] for the GTM-track nuances.
3. **The six existing Engineering-title placements.** Place each of the six anomalous engineering titles ("Senior Engineer," "Senior Engineer," "Lead Engineer," "Staff Engineer," "Principal Engineer, Platform," "Lead Software Architect") at exactly one level under the new rubric. For each, state the scope / complexity / autonomy / impact evidence the Head of Engineering has that justifies the placement, and any retroactive-reconciliation disposition (keep title, re-title, re-level) with the communication script.
4. **The Finance, Legal, and People ladders.** Author these in less depth (the Head of Finance, the fractional GC, and the Head of People each own the respective function-leveling nuances), but state the equivalence claim to the Engineering ladder and the cross-references to `startup-finance-fundraising-curriculum` mod-111 for Finance and to this module's own [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md) for band treatment.

### Part D — Leveling calibration norms

Produce the standing calibration-norm playbook. Cover:

1. **Calibration-committee cadence and membership.** Name the standing membership (Head of People, Head of Total Rewards once that role splits out at Series-B close, a rotating function leader per session) and the cadence — monthly during the annual comp-cycle window, quarterly outside it, ad-hoc for any proposed above-band exception or mid-cycle promotion. Cross-reference [chapter 04](../04-annual-comp-cycle.md) for the annual-cycle calibration gate and [mod-107](../../mod-107-performance-promotion-and-offboarding/) for the promotion machinery that feeds the committee.
2. **The calibration-against-hire-letter audit.** State the sampling cadence (annually, sampled from the previous cycle's offer letters), the sampling rate `<!-- needs-research: a defensible sampling rate for a Series-A → Series-B population moving from ~96 to an expected ~150 in 12 months -->`, and the audit-finding thresholds that trigger a band revision or a definition-rubric revision.
3. **Cross-function leveling council.** State the membership (one representative per track plus the leveling librarian), the cadence (twice per year), and the specific decisions reserved to the council — new-track standup, ladder-height change, inter-ladder equivalence-claim change.
4. **Leveling librarian ownership.** Name the role (Head of People at Series-A, Head of Total Rewards post-split) and the artifacts owned: master level-definition document, title-to-level map, calibration-committee minutes, cross-function leveling-council minutes, version-control log.
5. **Annual revision cadence.** State the fixed revision window (the annual comp-cycle window; see [chapter 04](../04-annual-comp-cycle.md)) and the mid-cycle-revision exception rule — new-function standup, documented material error — with the comp-committee-ratification requirement for any mid-cycle revision.

### Part E — Drift-mode diagnostic and the three present failure modes

Produce a written diagnostic that identifies which of chapter 01's drift modes are already present at Perihelion. Cover, at minimum:

1. **Function-by-function inflation** — is there evidence that any Perihelion function has drifted on its own? The two engineering promotions last cycle are candidate evidence. The Product-vs-Engineering equivalence dispute is candidate evidence.
2. **Scope creep inside a level** — identify any in-seat IC whose current scope exceeds the level they were hired at (chapter 01's E5-who-is-doing-E6-work pattern). Name the IC pattern (not the individual), the scope evidence, and the proposed disposition.
3. **New-function ladder-standup drift** — the four-person applied-research team is the test case. Diagnose whether the "Engineer, Applied Research" title has created an implied ladder that the council has not ratified.
4. **The Colorado posting incident.** Trace the incident — paused Colorado postings, a pay range that does not match the Engineering band — back to the drift-mode taxonomy. Is it a leveling failure, a band-authoring failure (the band does not yet exist), a reconciliation failure, or all three? State the root cause and the specific remediation gate (which Part — A, B, C, D, or F — closes the incident).

### Part F — Comp-committee presentation memo

Produce the **1-page memo** attaching the ratified architecture package and submitted to the comp committee. Cover:

- The three specific drift-mode diagnoses from Part E and the retroactive-reconciliation dispositions proposed in Parts B and C.
- The ratification asks the committee is being asked to approve: the track inventory (Part A), the dual-ladder convention (Part B), the level rubric (Part C), the calibration-norm playbook (Part D).
- The specific forward-dependencies this architecture unlocks: the cash-and-equity bands in [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md), the benchmark-source selection in [chapter 03](../03-benchmarking-data-sources-by-stage.md), the annual comp cycle in [chapter 04](../04-annual-comp-cycle.md), and the pay-transparency-compliance posture in [chapter 05](../05-pay-transparency-compliance.md).
- The Series-B diligence Severity-2 remediation tie-back and the expected timing (ratification before the diligence re-engages).
- The `<!-- needs-research -->` queue grouped by Part so the committee sees at a glance what data refresh is pending before the next ratification cycle.

## Starter guidance

- [Chapter 01](../01-job-architecture-and-leveling-framework.md) is the primary reference. Re-read the "why a job architecture exists," "function tracks," "IC and manager parallel ladders," "level definitions," "leveling calibration norms," and "drift modes" sections before authoring.
- The track inventory is a two-part question — not just which tracks exist but which stand up as their own vs. inside a parent. The applied-research team is the live decision; do not defer it.
- The two already-promoted engineers are the retroactive-reconciliation test case. The comp committee will anchor on them; name both dispositions precisely and own the communication script.
- The Colorado posting incident is the connective tissue between the architecture and the pay-transparency statute regime. The remediation gate is not "the Head of People unpauses the postings" — it is the ratified band that sits on top of the ratified level.
- Deep engineering-ladder competencies defer to `cto-curriculum`. Deep GTM-ladder nuances defer to `startup-product-gtm-curriculum`. Deep Finance-ladder nuances defer to `startup-finance-fundraising-curriculum` mod-111. Reference them explicitly rather than re-authoring them.
- **Do not manufacture market numbers.** Every band-equivalence claim, every market-calibration assertion, every sampling-rate proposal must be flagged `<!-- needs-research -->` with the source (Radford, Carta, Pave, Compensia), the stage cut (Series-A / Series-B tech), the function, the level, and the vintage.

## Deliverables

- `track-inventory-and-ratification.md` — Part A.
- `parallel-ladders-and-equivalences.md` — Part B.
- `level-rubric.md` — Part C.
- `calibration-norms-playbook.md` — Part D.
- `drift-diagnostic.md` — Part E.
- `comp-committee-memo.md` — Part F (1 page).

## Acceptance criteria

The package is acceptable if:

1. Part A enumerates every function track at Perihelion with a documented own-track-vs-parent-track decision for the applied-research team, a ratification path with the named body and quorum rule, and an off-ladder-role inventory.
2. Part B states the full IC-ladder height for every track (including unfilled tiers), picks a manager-premium or manager-parity convention with justification, states the specific IC-to-manager equivalence claims, and dispositions the two already-promoted engineers with a retroactive-reconciliation plan.
3. Part C places each of the six anomalous engineering titles at exactly one level under the new rubric with scope / complexity / autonomy / impact evidence and a retroactive-reconciliation disposition.
4. Part D names the calibration-committee membership and cadence, the calibration-against-hire-letter audit with sampling cadence and `<!-- needs-research -->` on the sampling rate, the cross-function leveling-council membership and cadence, the leveling-librarian role and artifacts owned, and the annual-revision cadence.
5. Part E diagnoses all three chapter-01 drift modes against Perihelion's current state and traces the Colorado posting incident to its root cause.
6. The comp-committee memo is **one page**, names the three drift-mode diagnoses, names the four ratification asks (track inventory, dual-ladder convention, level rubric, calibration norms), and surfaces the `<!-- needs-research -->` queue grouped by Part.
7. Every market-benchmark claim, every ladder-height-vs-market assertion, and every sampling-rate proposal is flagged with a `<!-- needs-research -->` marker specifying source, stage cut, function, level, and vintage. No invented percentages, no invented market claims.
8. The cross-references to [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md), [chapter 04](../04-annual-comp-cycle.md), [chapter 05](../05-pay-transparency-compliance.md), [mod-105 chapter 05](../../mod-105-equity-compensation-policy-and-comp-committee/05-compensation-committee.md), [mod-107](../../mod-107-performance-promotion-and-offboarding/), `cto-curriculum`, `startup-product-gtm-curriculum`, and `startup-finance-fundraising-curriculum` mod-111 are present.
9. Nothing left as `[TBD]` or `[FILL IN]`; every market or sampling claim is either cited to a chapter-01 range or flagged `<!-- needs-research -->`.
