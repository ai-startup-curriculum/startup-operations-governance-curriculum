# Exercise 03 — ISO / NSO / RSU country selection drill

> Estimated time: **~5 hours** · Related chapter: [02 — The IC equity-plan structure](../02-ic-equity-plan-structure.md)

## Problem statement

Breakwater Compute is a Delaware C-corp building AI-training infrastructure. It closed a $64M Series-B eight months ago and now employs 118 people across seven jurisdictions:

- **California** — 41 employees (engineering, research, GTM-west)
- **New York** — 19 employees (GTM-east, finance, legal)
- **Texas** — 11 employees (data-center ops, hardware)
- **Ontario, Canada** — 14 employees (engineering satellite office in Toronto)
- **London, United Kingdom** — 12 employees (EMEA GTM + a small research team)
- **Berlin, Germany** — 9 employees (platform engineering)
- **Singapore** — 12 employees (APAC GTM + a solutions-architecture team)

The equity plan — a standard US-style 2016-vintage Carta template adopted at Series-A — issues **ISOs to every US employee** and **NSOs to every international employee** regardless of country. Vesting is 4-year with a 1-year cliff. There are no RSUs in the plan today. Early exercise is permitted up to the first anniversary for employees hired before Series-B close; it was quietly closed for post-Series-B hires without a formal board resolution.

Breakwater's aggregate gross assets (AGA) are approximately **$41.7M** at the last close. The CFO's working forecast — assuming no further financing in the next 9 months — projects AGA to cross **$50M around month 11 from today**. The $50M AGA line matters because stock issued after the corporation's AGA crosses $50M loses the Qualified Small Business Stock (QSBS) exemption under IRC §1202.

The General Counsel and CFO have asked you — the Head of People Ops, acting with outside-equity-counsel support — to produce a refreshed **per-country, per-level grant-instrument matrix**; a **QSBS-planning overlay** for US employees in light of the oncoming $50M AGA line; a **plan for a private-company RSU shift** at executive levels; and a **comp-committee memo** that packages the recommendation plus the outside-counsel work list.

## Requirements

### Part A — Current-state audit

Produce a written diagnosis of the current equity-plan posture. Cover:

1. Where "ISO for every US employee" is factually fine and where it is likely tripping over the $100k ISO vesting-value limit at senior IC and manager grants.
2. Where "NSO for every international employee" is likely leaving tax-qualified instrument capacity on the table (specifically: UK EMI; Canadian stock-option deduction; Singapore qualified employee stock option schemes). For each country, name what the plan is currently missing and why that matters to the employee (post-tax outcome) and to the corporation (deductibility, filings).
3. The securities-law exposure of granting US-template options into Germany and Singapore without local-law wrappers or filings. Flag with `<!-- needs-research -->` the specific filing / prospectus-exemption questions each jurisdiction raises.
4. The governance-hygiene problem of early-exercise having been quietly closed for post-Series-B hires without a formal board resolution — and what has to happen to clean that up.

### Part B — Per-country, per-level grant-instrument matrix

Produce a matrix with one row per country and columns for IC-level, senior-IC-level, manager-level, and executive-level grants. For each cell, specify the plan instrument, the typical level cutoff that triggers a shift, and the specific country-tax / securities-law constraint that drives the choice. Where the local law moves quickly or involves a number you cannot verify from the chapter, use `<!-- needs-research -->` markers rather than inventing values.

Cover at minimum:

1. **United States** — ISO up to the $100k vesting-value limit per calendar year; NSO for the overflow above $100k and for all non-US-resident hires on US payroll; an RSU appearance at executive grants above a specified aggregate grant value (define the threshold); an early-exercise policy decision (open or closed, uniform across levels or not); and the QSBS implications of the oncoming $50M AGA line — specifically, which employees should be issued pre-crossing vs. post-crossing.
2. **United Kingdom** — EMI (HMRC-qualified Enterprise Management Incentive) option up to the per-employee cap; non-qualified NSO (or UK unapproved option) for grants above the EMI cap and for employees who do not satisfy the EMI working-time or non-material-interest tests. Flag `<!-- needs-research -->` the current EMI individual limit, the EMI aggregate company limit, the HMRC gross-assets and employee-count company-size qualification thresholds, and the current qualifying-trade exclusions.
3. **Canada (Ontario)** — stock options with the CRA stock-option deduction. Flag `<!-- needs-research -->` the 2021 federal legislation that limited the stock-option deduction above a per-employee annual vesting threshold for employees of larger / non-CCPC employers (Breakwater is not a CCPC); the current threshold; and whether the deduction limitation applies to Breakwater's grant pattern.
4. **Germany** — virtual-share-plan (VSU / phantom equity) is the common instrument because actual share issuance into Germany carries local-law complexity (notarisation, dry-income taxation at vesting). Flag `<!-- needs-research -->` the 2024 Future Financing Act (Zukunftsfinanzierungsgesetz) changes to §19a EStG that extended tax-deferral treatment for employee share grants and the current qualifying employer size / revenue thresholds; also flag whether VSUs still clear the dry-income problem better than real-share grants for Breakwater's stage.
5. **Singapore** — stock options with CPF (Central Provident Fund) treatment and the "deemed exercise" rule that triggers taxation when a non-citizen / non-permanent-resident employee leaves Singapore while holding unexercised options. Flag `<!-- needs-research -->` the current qualified employee stock option scheme (QEOS) and employee equity-based remuneration (EEBR) scheme availability for a company of Breakwater's size.

Each per-country section must name the plan instrument, the typical level cutoff, and the specific country-tax or securities-law constraint. For any number or current-year threshold you cannot verify from the chapter, use `<!-- needs-research -->` markers rather than invent values.

### Part C — QSBS planning overlay (US only)

Produce a written overlay that addresses the oncoming $50M AGA line. Cover:

1. The specific population of US employees who should be issued **before** the AGA crosses $50M (so that the five-year QSBS clock starts on QSBS-eligible stock) vs. **after** the AGA crosses $50M (where the shares will not qualify as QSBS and the issuance pattern should be reconsidered on different grounds).
2. The role of **NSO + early-exercise + 83(b) election** in locking in the QSBS clock for a current pre-$50M-AGA hire whose vesting-value would otherwise push the grant over the $100k ISO limit — i.e., why issuing an NSO with early-exercise and a timely 83(b) can start the five-year clock on day one of grant rather than on each vesting event.
3. The decision tree for pre-$50M-AGA grants: ISO (within $100k limit) vs. NSO-with-early-exercise-and-83(b), and when each wins on a post-tax basis for the employee.
4. The decision tree for post-$50M-AGA grants (where QSBS is off the table): what the plan optimises for instead (long-term capital gains on exercise-and-hold, RSU double-trigger simplicity, cash deferral).
5. The specific **operational asks** on the finance team: AGA monitoring cadence, who signs off before each new grant that the AGA has not yet crossed $50M, and what the data-trail looks like for a §1202 defence five years from now.

### Part D — Private-company RSU shift

Produce a written recommendation on introducing double-trigger private-company RSUs (PCRSUs) at executive levels. Cover:

1. The exec-level threshold above which PCRSUs with double-trigger (service + liquidity-event) vesting replace options as the default instrument. Specify the threshold both as a title band (e.g., "VP and above") and as a grant-value threshold (e.g., aggregate grant value above $X).
2. The rationale for the shift — the dilutive-share-count argument, the executive-tax-at-exercise problem for high-value option grants at a late-private valuation, the recruiting-signal argument vs. big-tech public-RSU packages.
3. The mechanics — double-trigger (service-based time vesting + liquidity-event trigger, typically IPO or change-of-control within a specified post-grant window), 83(i) election considerations, and the §409A implications of settlement timing.
4. A reference to the **Carta PCRSU documentation pattern** (plan amendment, award agreement template, double-trigger definition) as the operational baseline. Flag `<!-- needs-research -->` the current Carta template version and any 2025 updates to the pattern.
5. The international wrinkle — PCRSUs are a US-conceived instrument; name which of the six non-US jurisdictions (if any) in Breakwater's footprint can accept a PCRSU-equivalent and which will need a local-law substitute (phantom RSU, cash-settled RSU, etc.).

### Part E — Comp-committee memo + outside-counsel ask list

Produce two outputs:

1. A **2–3 page comp-committee memo** that packages Parts A–D into a decision-ready recommendation. The memo must name:
   - the three or four specific plan amendments the comp committee is being asked to approve;
   - the per-country matrix (Part B) as an appendix;
   - the QSBS overlay (Part C) and the AGA-monitoring commitment the finance team is making;
   - the PCRSU shift (Part D) and the exec-level threshold;
   - the budget envelope for outside-counsel engagements across the six non-US jurisdictions.
2. An **outside-counsel ask list** — one entry per country (UK, Canada, Germany, Singapore, plus a US-equity-counsel entry and a general-securities-counsel entry) — specifying what each counsel needs to opine on before the matrix is operationalised. Each entry names the specific statutory / regulatory question, the deliverable Breakwater is asking for (memo, filing, template agreement), and a target turnaround.

Cross-reference `../02-ic-equity-plan-structure.md` for the IC-plan structure and `../mod-113-international-expansion-and-global-workforce/` for the broader international-workforce overlay that drives the per-country footprint.

## Starter guidance

- Chapter 02 is the primary reference for the IC equity-plan structure. Use the ISO / NSO / early-exercise / 83(b) / QSBS framing from that chapter as your spine; the per-country overlay is the net-new work.
- Do **not** invent country-specific tax thresholds, deduction caps, or current-year EMI limits. The point of the `<!-- needs-research -->` markers is to force a disciplined handoff to outside counsel rather than a confident-sounding wrong number.
- The $50M AGA line is a hard cliff for QSBS, not a soft target. Treat the pre-cross / post-cross distinction as a binary that drives the Part C overlay.
- The "ISOs for US, NSOs for international" default is a common Series-A artefact and is almost always suboptimal by Series-B. The point of the drill is to replace that default with a per-country, per-level matrix rather than to defend it.
- PCRSUs are a US instrument; do not assume they port cleanly to the UK, Germany, or Singapore. Part D's international wrinkle is non-trivial.
- The comp-committee memo is a decision document, not a tutorial. The committee's job is to approve the amendments and the outside-counsel budget — write the memo accordingly.

## Deliverables

- `current-state-audit.md` — Part A.
- `per-country-per-level-matrix.md` (or `.xlsx` / `.csv` if you prefer a table) — Part B.
- `qsbs-planning-overlay.md` — Part C.
- `pcrsu-shift-recommendation.md` — Part D.
- `comp-committee-memo-equity-plan-refresh.md` — Part E, memo.
- `outside-counsel-ask-list.md` — Part E, counsel engagement list.

## Acceptance criteria

The package is acceptable if:

1. The current-state audit identifies the $100k ISO vesting-value overflow at senior IC and manager grants and the missed EMI / Canadian-deduction / Singapore-qualified-scheme opportunities, with the specific country consequence for each.
2. The per-country matrix has one row per country and columns for IC, senior IC, manager, and executive grants, with the plan instrument and the driving constraint named in each cell.
3. Every country-specific tax number, EMI threshold, Canadian deduction limit, German §19a or 2024 Future Financing Act threshold, and Singapore QEOS / EEBR availability flag is marked `<!-- needs-research -->` rather than invented.
4. The QSBS overlay is **explicit**: it names which US employees should be issued pre-$50M-AGA vs. post-$50M-AGA, and it walks through the NSO + early-exercise + 83(b) mechanic for locking in the five-year clock.
5. Part D names a specific exec-level threshold (title band and grant-value threshold) above which PCRSUs with double-trigger vesting replace options, and references the Carta PCRSU documentation pattern as the operational baseline.
6. The comp-committee memo names three or four specific plan amendments the committee is being asked to approve and a budget envelope for the outside-counsel engagements.
7. The outside-counsel ask list has one entry per non-US jurisdiction (UK, Canada, Germany, Singapore) plus a US-equity-counsel entry and a general-securities-counsel entry, each with a specific statutory question, a named deliverable, and a target turnaround.
8. The early-exercise governance-hygiene problem (post-Series-B closure without a board resolution) is addressed with a specific remediation step.
9. Cross-references to `../02-ic-equity-plan-structure.md` and `../mod-113-international-expansion-and-global-workforce/` are present where the chapter dependency is load-bearing.
10. Nothing left as `[TBD]` or `[FILL IN]`.
