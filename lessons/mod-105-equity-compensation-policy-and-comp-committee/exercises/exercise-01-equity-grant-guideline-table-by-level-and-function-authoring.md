# Exercise 01 — Equity grant-guideline table by level and function authoring

> Estimated time: **~5 hours** · Related chapter: [01 — Grant guidelines by level and function](../01-grant-guidelines-by-level-and-function.md)

## Problem statement

Fallstreak Networks, Inc. is a Delaware C-corp building a programmable-WAN control plane for mid-market enterprises. The corporation closed a $48M Series-B six months ago at a $240M post-money and currently has **110 employees**: 48 engineering (12 platform, 14 product-engineering, 8 infra / SRE, 6 security, 5 data, 3 ML), 11 product / design, 32 GTM (16 AE / SE, 6 CS, 6 marketing, 4 sales operations), 14 G&A / operations (5 finance, 3 legal, 4 people, 2 IT), and 5 research.

Cap-table state at the last board meeting:

- **26,840,000 shares outstanding** on a fully-diluted basis.
- **15.0% option pool refreshed at the Series-B close**, of which **2.1% of fully-diluted remains uncommitted** (i.e., ~85% of the refreshed pool has already been granted or promised against pending offers).
- **409A FMV of $4.12 / share** at the last refresh (90 days ago); next 409A refresh scheduled in 90 days.
- Common strike on all new ISO grants is the current 409A FMV.

The board-approved 18-month plan calls for **45 net-new hires**: 20 engineering (across platform, product-engineering, infra, security, and a first ML-platform hire), 4 product / design, 15 GTM (including a Director of Enterprise Sales and the corporation's first Head of Revenue Operations), 4 G&A (first in-house GC, a Senior FP&A, and two People-ops hires), and 2 research.

Current state of the grant approach: **there is no formal grant-guideline table.** The founder-CEO, the Head of Engineering, and the VP Sales have each been sizing grants "by inspection," by anchoring to whatever the most recent comparable offer went out at, and occasionally by asking an investor-side advisor for a sanity check. The compensation committee was constituted at Series-B close but has not yet ratified a guideline table. Notable inconsistencies the Head of People has flagged in the last 30 days:

1. **Two L5 (staff) platform-engineering hires 92 days apart** — the second grant is **~2.1×** the first on a share-count basis at the same 409A, with no documented leveling or critical-skill rationale.
2. **A Senior Enterprise AE** was granted equity at a share count sitting inside the current engineering-band for the equivalent level (E4), roughly **1.6×** what a Carta-cited GTM band at the same level would predict; the OTE acceleration mechanics typical for the role were not factored in.
3. **The first in-house GC offer** currently being negotiated is sized against "what the founder-CEO remembers paying the fractional GC in 2024" — no benchmark data has been pulled.
4. **Three "founding-engineer" grants from 2023** are still being used as the anchor for current senior-IC offers, despite two priced rounds and a ~7× increase in 409A FMV since those grants were issued.

Your role: you are the **Head of People** (or the outside total-rewards advisor engaged by the comp committee) tasked with authoring the first ratifiable grant-guideline table. Produce the current-state diagnosis, the target-state table, function-specific adjustments, the dilution-budget interaction, and the comp-committee presentation memo.

## Requirements

### Part A — Current-state diagnosis

Produce a written diagnosis the comp committee can read in one sitting. Cover:

1. **Grant-by-grant audit** of the last 12 months of initial grants, grouped by hiring manager and by function. Identify which grants fall outside what a reasonable Series-B band would predict, and tag each anomaly with a candidate root cause (manager inconsistency, missing level anchor, cross-function miscalibration, stale founder-era anchor, undocumented critical-skill premium).
2. **At least two specific inconsistencies** the comp committee is going to surface at ratification — including (but not limited to) the two L5 platform-engineering hires with the 2.1× delta and the AE granted at an engineering-band share count. Name each inconsistency precisely and name the hiring manager and the date range.
3. **Pool-utilization snapshot**: the 2.1% remaining in a 15% pool at 110 employees with a 45-hire plan ahead. State the implied *average* fully-diluted grant per net-new hire that fits inside the remaining pool, and compare that to the Series-B IC bands referenced in chapter 01 (flag the specific band numbers as `<!-- needs-research -->` rather than inventing them).
4. **The four problems** chapter 01 names (inconsistency across managers, dilution burn, benchmarking drift, comp-committee ratification friction) — show which of the four are already present at Fallstreak and cite the evidence.

### Part B — Target-state grant-guideline table

Author the ratifiable grant-guideline table. Cover:

1. **Representation choice.** Chapter 01 recommends dollar-value at the current 409A FMV from Series-B onward, with share-count fallback. State the choice, state the fallback, and state the ISO § 422(d) footnote the table carries for grants that exceed the $100,000-per-year first-exercisable limit.
2. **The table itself**, as a markdown or spreadsheet artifact. Axes: **function × level × band** (floor / midpoint / ceiling) in dollar-value at the $4.12 409A FMV, with a parallel column translating the midpoint into percent-of-fully-diluted and into share count. Cover at minimum:
    - Engineering IC: E2, E3, E4, E5, E6.
    - Engineering management: M1, M2, D1.
    - Product management: P2, P3, P4, P5.
    - Design: D2, D3, D4.
    - GTM: AE, Senior AE, Enterprise AE, Sales Manager, Director of Sales, VP Sales; SE; CS Manager; Marketing Manager, Director of Marketing.
    - G&A: Finance (Analyst, Senior Analyst, Manager, Director), Legal (Senior Counsel, GC), People (Manager, Director), IT.
3. **Benchmark citation.** For each band, name the data source(s) that would be used to set the midpoint (Carta Total Comp, Pave, Compensia, Advanced-HR / Option Impact, Radford Global Technology Survey). **Do not manufacture numbers.** Flag every midpoint with a `<!-- needs-research -->` marker that specifies the source, the stage cut (Series-B tech), the function, the level, and the vintage ("Q3 2026 cut") you would resolve to before ratification.
4. **Exception workflow.** State the floor-to-ceiling range inside which the hiring manager grants without approval, the above-ceiling approval path (Head of People + founder-CEO; above a higher threshold, comp committee chair), and the equity-grant-log entry that documents every exception for the annual review.

### Part C — Function-specific adjustments

Produce the written rationale that sits alongside the table. Cover:

1. **Engineering vs. product management**: the chapter notes product tends to band 5–15% below engineering at junior levels and converge at senior levels. State Fallstreak's convention, flag the specific ratio as `<!-- needs-research -->`, and justify.
2. **Engineering vs. GTM**: the AE equity band is smaller than the equivalent-level engineering band because the AE upside is in commission acceleration. State the convention for AE, Senior AE, Enterprise AE, Sales Manager, Director of Sales, VP Sales. Call out explicitly that the AE grant last quarter (flagged in Part A) sat in the engineering band and name the corrective adjustment.
3. **Engineering vs. G&A**: G&A IC bands sit below engineering in most benchmark cuts. The first-of-its-kind strategic hires (first GC, first Head of Finance, first Head of People) are sized against the exec band, not the function band — explicitly note which of Fallstreak's 45 planned hires are "first-of-its-kind" and therefore priced as exec grants (see chapter 04).
4. **Founder-judgement cells.** Identify the cells where benchmark data is thin and the founder-CEO plus comp committee chair must set the number by judgement — chapter 01 names first-of-its-kind roles, critical-skill premiums, and founder-adjacent roles (Chief of Staff, first Head of People, first Business Operations hire). Mark those cells distinctly in the table.
5. **Critical-skill premium policy.** State the convention for above-band grants justified by scarce skill (foundation-model research, specific security clearance, named exec with public track record). State the documentation requirement so the comp committee can review exception density annually (see chapter 06).

### Part D — Interaction with the dilution budget

**Do not re-derive the pool math.** The pool-sizing, pool-refresh, and promised-but-ungranted mechanics are owned by `startup-finance-fundraising-curriculum` (equity-economics track). Here, describe the **policy constraint** the dilution budget imposes on the grant-guideline table:

1. State the pool-utilization forecast as a function of the proposed table × the 45-hire plan. Show the arithmetic (sum of midpoints weighted by the hiring plan ÷ remaining pool). If the sum exceeds the 2.1% remaining, state the three options chapter 01 names — under-grant against the table, grant to the table and run out mid-cycle, or negotiate a pool top-up at the next priced round — and recommend one with rationale.
2. Identify the specific **CFO / Head of Finance handoff**: who owns the forecast, who is notified when utilization crosses 60% / 80% / 90% of remaining pool, and the trigger that initiates a pool-refresh conversation with the board.
3. Reference the `startup-finance-fundraising-curriculum` module and chapter where pool sizing and refresh mechanics are owned, and explicitly note that the comp-committee memo defers the dilution math to that owner.

### Part E — Comp-committee presentation memo

Produce a **1-page memo** attaching the table and submitted to the comp committee for ratification. Cover:

- The two or more current-state inconsistencies (from Part A) that motivate the table.
- The representation choice and the top three design decisions (benchmark sources, exception workflow, critical-skill-premium policy).
- The pool-utilization headline from Part D and the recommended response.
- The three specific asks the comp committee is being asked to ratify (the table, the exception workflow, the critical-skill-premium documentation requirement) and the forward references to chapters 03 (refresh / promotion / retention), 04 (executive comp), and the forthcoming comp-committee charter work (`../05-compensation-committee.md` once authored, and the annual cycle in [chapter 06](../06-annual-comp-cycle.md)).
- The `<!-- needs-research -->` markers surfaced in Parts B and C, grouped so the comp committee can see at a glance what data refresh is required before the next ratification cycle.

## Starter guidance

- Chapter 01 is the primary reference. Re-read the "representation choice" section, the "initial-hire grant sizing by stage" section (specifically the Series-B subsection), the "function differentiation" section, and the "level differentiation" section before authoring the table.
- The exception workflow and the equity-grant log are introduced in chapter 01 and operationalised in [chapter 06](../06-annual-comp-cycle.md). Point back to both.
- The exec-band treatment for first-of-its-kind strategic hires (first GC, first Head of Finance) is owned by [chapter 04](../04-executive-compensation-packages.md). Reference it; do not re-derive the exec package here.
- The dilution budget and pool-refresh mechanics are owned by `startup-finance-fundraising-curriculum`. Do not re-derive the pool math; cite the owner module and chapter.
- **Do not manufacture market numbers.** Every midpoint, every band width, every function-vs-engineering ratio, every critical-skill-premium quantum must either be taken directly from a range the chapter already names *or* flagged with a `<!-- needs-research -->` marker that specifies the source (Carta, Pave, Compensia, Advanced-HR, Radford), the stage cut, the function, the level, and the data vintage you would resolve before the ratification meeting.
- The two L5 platform-engineering hires with the 2.1× delta and the Senior Enterprise AE granted inside the engineering band are the two inconsistencies the comp committee will anchor on. Treat them as the lead examples, not as the only two.

## Deliverables

- `current-state-diagnosis.md` — Part A.
- `grant-guideline-table.md` (or `grant-guideline-table.csv` / `.xlsx` if you prefer a spreadsheet) — Part B's table, with the dollar / percent / share-count columns and the `<!-- needs-research -->` markers.
- `function-adjustments-rationale.md` — Part C.
- `dilution-budget-policy-note.md` — Part D.
- `comp-committee-memo.md` — Part E (1 page).

## Acceptance criteria

The package is acceptable if:

1. The current-state diagnosis identifies **at least two specific inconsistencies** in the current grant history (including, at minimum, the two L5 platform-engineering hires with the 2.1× delta and the Senior Enterprise AE granted inside the engineering band), each with a hiring-manager and date-range attribution and a candidate root cause.
2. The representation choice is **dollar-value at the current 409A FMV with share-count fallback** (per chapter 01's Series-B recommendation), and the table carries the ISO § 422(d) $100,000 first-exercisable footnote.
3. The grant-guideline table covers, at minimum, engineering IC (E2–E6), engineering management (M1–D1), product (P2–P5), design (D2–D4), the GTM ladder through VP Sales, and the G&A roles enumerated in Part B — with floor / midpoint / ceiling bands and parallel dollar / percent / share-count columns.
4. **Every market-benchmark number** (band midpoint, floor, ceiling, function-vs-engineering ratio, critical-skill-premium quantum) is either cited to a range chapter 01 already names *or* flagged with a `<!-- needs-research -->` marker that specifies the source (Carta / Pave / Compensia / Advanced-HR / Radford), the stage cut, the function, the level, and the vintage. No invented percentages, no invented dollar numbers.
5. The exception workflow states the manager-discretion range, the above-ceiling approval path, and the equity-grant-log documentation requirement.
6. The function-adjustments rationale explicitly treats engineering vs. product, engineering vs. GTM, and engineering vs. G&A, and identifies at least three cells where founder judgement (not benchmark data) is the dominant input.
7. The first-of-its-kind strategic hires in the 45-hire plan (first in-house GC, Senior FP&A if sized against finance-leadership, Director of Enterprise Sales, first ML-platform hire, Head of Revenue Operations as applicable) are explicitly flagged for exec-band treatment with a cross-reference to [chapter 04](../04-executive-compensation-packages.md).
8. The dilution-budget note shows the pool-utilization arithmetic at the proposed table × the 45-hire plan, states whether the sum fits inside the 2.1% remaining, and recommends one of chapter 01's three responses — with an explicit cross-reference to `startup-finance-fundraising-curriculum` as the owner of the pool math.
9. The comp-committee memo is **one page**, names the two or more current-state inconsistencies, names three specific ratification asks, and surfaces the `<!-- needs-research -->` markers grouped for the comp committee's data-refresh queue.
10. The memo forward-references [chapter 03](../03-refresh-promotion-and-retention-grants.md), [chapter 04](../04-executive-compensation-packages.md), the forthcoming compensation-committee charter (`../05-compensation-committee.md`), and [chapter 06](../06-annual-comp-cycle.md) so the comp committee understands where this exercise sits in the broader equity-governance arc.
11. Nothing left as `[TBD]` or `[FILL IN]`; every market number is either cited to a chapter 01 range or flagged `<!-- needs-research -->`.
