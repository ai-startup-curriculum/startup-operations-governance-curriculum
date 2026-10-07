# 1. Grant guidelines by level and function

> A grant-guideline table is the single artifact that turns equity from a founder-by-founder judgement call into a reproducible compensation decision — and the single artifact a comp committee will ask to see first.

## Motivation

Every offer letter the corporation sends out carries an equity number. That number is either (a) the output of a grant-guideline table that the Head of People, the founder-CEO, and (at Series-B+) the compensation committee have ratified, or (b) a one-off decision the hiring manager made in a Slack thread with the founder-CEO forty minutes before the offer went out. The second mode is where most of the recurring equity-governance pain in a startup originates.

Getting grant guidelines wrong — or operating without them at all — costs the corporation in specific, repeating ways:

- **Inconsistency across managers.** Two IC engineers of equivalent level, hired the same month into the same team, get materially different grants because two different hiring managers negotiated two different packages with two different candidate expectations. The second-hire discovers this at the first all-hands bar conversation, and the corporation now has a trust problem that no HR-ops fix can clean up.
- **Dilution burn.** Without a per-stage grant budget tied to the fully-diluted cap table, the corporation over-grants early and under-grants late — the pool runs dry, a pool refresh gets negotiated into the next round at founder-dilutive terms, and the Series-B lead captures economics the founders did not intend to give up. The economics of pool sizing and refresh are owned by `startup-finance-fundraising-curriculum`; this chapter owns the per-grant *policy* that spends against the pool.
- **Benchmarking drift.** The corporation offers a Series-A engineer the "0.25%" the founder-CEO vaguely remembers from a 2019 Carta blog post. The current-market Series-A IC band is somewhere else entirely, the offer either over- or under-shoots, and the corporation either over-dilutes or loses the candidate.
- **Comp-committee ratification friction.** At Series-B+ the compensation committee is going to ask "what are the grant guidelines, who authored them, when were they last benchmarked, and what are the exception-escalation rules." A corporation that cannot answer those four questions in one meeting slot will spend the next three meeting cycles answering them.
- **17 C.F.R. § 229.402 downstream disclosure.** For an eventual public company, named-executive-officer grant history under Item 402 is a public document. A messy grant history — unexplained outliers, mid-cycle refresh grants with no documented rationale, exec grants that look judgement-call-y — becomes a proxy-season narrative the corporation did not want. See [chapter 09](./09-sec-reg-sk-item-402-disclosure.md).

This chapter builds the grant-guideline table from the ground up: what it is, how it is represented at each stage, who authors it, and how it varies across function and level.

## Why a grant-guideline table exists

Four distinct problems collapse into a single artifact when the corporation writes a grant-guideline table.

### Consistency across managers

The grant-guideline table is the compensation analogue of a leveling rubric. Two candidates of the same level in the same function should receive grants from the same band, modulo documented adjustments (critical-skill premium, counter-offer, geographic differential). The band is the manager's constraint; the exception-approval workflow is the manager's escape hatch; the comp committee (at Series-B+) is the backstop. Without the table, every offer is a bespoke negotiation and the corporation has no way to defend the equity line against a future pay-equity audit.

### Dilution control

Every grant is a draw against the option pool. The pool is a finite resource negotiated at each priced round. A grant-guideline table that is denominated in percent-of-fully-diluted at hire gives the Head of People and the CFO a direct read on "if we execute the hiring plan at the current guidelines, how much of the pool is consumed, and when does the next refresh need to happen." The pool-math machinery itself — pool size negotiation at a priced round, refresh math, promised-but-ungranted shares, waterfall interaction — lives in `startup-finance-fundraising-curriculum`. This chapter uses the pool as a budget constraint.

### Equity-vs-cash philosophy at stage

A seed-stage corporation is cash-poor and equity-rich; a growth-stage corporation is comparatively cash-rich and equity-scarce. The grant-guideline table encodes the corporation's current position on that trade-off. A common pattern: at seed, equity is a disproportionate share of total compensation and base salary is deliberately under-market; at Series-B+, base salary approaches market and equity settles into a market-band at the current 409A valuation. The *shape* of the equity-vs-cash curve is a founder / CEO / board decision; the table operationalises it.

### Benchmarking discipline

Grant-guideline tables are not authored in a vacuum. They are drafted against external benchmarking data from a small set of market vendors:

- **Carta Total Comp** — percentile data on equity grants and cash comp by stage, level, and function, drawn from the Carta customer base.
- **Pave** — comp-benchmarking SaaS with aggregated grant and base-salary data by level and function.
- **Option Impact (now part of Advanced-HR / J.Thelander)** — one of the longest-running venture-backed-company compensation surveys; the Advanced-HR VC Executive Compensation Survey is used widely by VC-firm comp advisors.
- **Compensia** — compensation consultancy that advises comp committees and provides peer-group analyses, particularly at Series-B+ through pre-IPO.
- **Radford (Aon)** — the standard public-company and late-stage-private benchmark data source; the Radford Global Technology Survey is a comp-committee staple.

The grant-guideline table should name its data sources and the vintage of the data (e.g., "Carta Series-B tech bands, Q3 2026 cut"). <!-- needs-research: current pricing / packaging of Carta Total Comp, Pave, Advanced-HR, Compensia advisory, and Radford Global Technology Survey for a Series-B startup; what is the typical annual spend on comp-benchmarking data at that stage? -->

## The structure of the grant-guideline table

The table has four axes: **function** (engineering / product / design / GTM / G&A), **level** (IC ladder, manager ladder, exec ladder), **stage** (the corporation's current funding stage), and **grant size** (the unit varies — see below). Each cell is a band, not a point: a target midpoint and a floor-to-ceiling range the hiring manager may land anywhere inside without exception approval.

### Representation choice: four candidate units

A grant can be denominated four different ways. Each has an operating consequence.

1. **Percent of fully-diluted** at the time of grant. Candidate-legible ("you are getting 0.4% of the company"), founder-legible (direct dilution read), but drifts as the corporation issues more shares — a 0.4% grant today becomes a smaller percentage after the next round. Used by convention at seed and Series-A, where the pool is small and the dilution read is the point.
2. **Share count** — a fixed number of options or RSUs. Candidate-illegible unless paired with a current 409A FMV ("1,000 options at a $12 FMV is $12,000 of intrinsic value today"). Operationally natural because the equity-admin system (Carta, Pulley, Shareworks) issues share counts, not percentages.
3. **ISO/dollar value** at the current 409A FMV. "Here is $320,000 of options at the current fair market value, vesting over four years." Candidate-legible once the candidate trusts the 409A number, directly comparable to public-company RSU grants, and the standard representation from Series-B onward because that is how market comp data (Carta, Pave, Radford) is reported.
4. **OTE multiple** for sales — "equity grant equal to 1.5× on-target earnings" — occasionally seen for commissioned GTM roles so that the equity line scales with the comp band.

The two defaults this chapter recommends:

- **Pre-Series-B**: denominate the guideline in **percent-of-fully-diluted at hire**. The pool is small enough that the dilution read is the most important lens, and candidates at this stage are selected for their willingness to engage with the percent-of-company narrative.
- **Series-B and later**: denominate the guideline in **dollar-value at the current 409A FMV**, with share-count fallback for the actual grant instrument. This is how market benchmarks are reported and how the comp committee will want to see the table.

The ISO $100,000-per-year first-exercisable limit under **IRC § 422(d)** is a separate constraint on how much of a given grant qualifies as an incentive stock option in a given calendar year. Guideline tables denominated in dollar-value should carry a footnote that grants exceeding the § 422(d) limit convert the excess to NSO treatment. The ISO vs. NSO mechanics in depth are in [chapter 02](./02-ic-equity-plan-structure.md).

### Dilution-budget interaction

The sum of all cells in the table, weighted by the hiring plan for the next 12–18 months, must fit inside the current option pool. If it does not, one of three things happens: (a) the corporation under-grants against the table and the table becomes decorative; (b) the corporation grants to the table and the pool runs out mid-cycle, forcing an off-cycle refresh at terms the lead investor sets; (c) the corporation negotiates a pool top-up at the next priced round, which is dilutive to the common. The CFO or Head of Finance is the owner of the pool-utilization forecast; this is the primary cross-functional handoff into `startup-finance-fundraising-curriculum`.

## Initial-hire grant sizing by stage

The pattern across stages: **initial grants are the largest grant an IC ever receives in their tenure.** Everything after the initial grant — refresh, promotion, retention — is additive and smaller. Refresh cadence and sizing is the subject of [chapter 03](./03-refresh-promotion-and-retention-grants.md). This chapter sizes initial grants only.

### Seed (pre-priced or priced seed; headcount < 15)

Grants are denominated in percent-of-fully-diluted. The founder-CEO (plus a comp advisor if one is engaged) authors the table. Variance across hires at this stage is dominated by employee number, not by level — hire #3 is categorically different from hire #12 — and the "level" dimension is sometimes compressed into a single "early-engineer" or "founding-engineer" band. <!-- needs-research: current-market seed-stage founding-engineer equity bands (percent-of-fully-diluted at hire) and how they vary by employee number across employees 1–15; cite to a specific Carta, Pave, or Index Ventures benchmark. -->

### Series-A (headcount 15–50)

Grants are still denominated in percent-of-fully-diluted but the band widens as the level ladder emerges. A rudimentary IC ladder (E2 / E3 / E4 / E5 — see "level differentiation" below) and a first manager level typically appear. Base salaries move toward market as the Series-A capital funds a two-year runway. The founder-CEO and the Head of People (plus an outside comp advisor if engaged) author the table. <!-- needs-research: current-market Series-A IC equity bands by level (E2–E6 or equivalent) in percent-of-fully-diluted; typical Series-A pool size as a percent of fully diluted post-raise. -->

### Series-B (headcount 50–200)

The denomination shifts to dollar-value at the current 409A FMV. The comp committee is in place and ratifies the table. The Head of People (or Head of Total Rewards, if that role has been added) drafts; a Compensia / Radford / Pave advisor supplies the benchmark data; the comp committee ratifies annually (see [chapter 06](./06-annual-comp-cycle.md)). <!-- needs-research: current-market Series-B IC equity bands by level in dollar-value at FMV; typical refresh cadence and refresh-grant-as-percent-of-initial-grant. -->

### Growth (headcount 200+, Series-C through pre-IPO)

The table is a mature, benchmarked artifact. Peer-group selection becomes a comp-committee decision — the committee ratifies a 10–20-company peer group against which the corporation benchmarks executive and senior IC compensation. Radford Global Technology Survey, Compensia peer-group analyses, and the ISS / Glass Lewis executive-comp lens all enter the frame. The exec-comp overlay (performance-based grants, change-of-control vesting, severance) is substantial — see [chapter 04](./04-executive-compensation-packages.md), [chapter 07](./07-change-of-control-equity-policy.md), and [chapter 08](./08-executive-severance-and-release.md). <!-- needs-research: current-market pre-IPO IC equity bands in dollar-value and how they shift as the corporation approaches an IPO window. -->

### Pre-IPO / dual-track

Grants may begin to use RSUs (or double-trigger RSUs with a liquidity-event vesting condition) rather than options, particularly for executives and senior ICs where the strike-price-to-409A spread has grown large enough that options are no longer efficient. The equity-plan structure that permits RSUs is covered in [chapter 02](./02-ic-equity-plan-structure.md); the ownership-boundary map that governs who signs what at this stage is covered in [chapter 10](./10-ownership-boundary-map.md).

## Function differentiation

At the same level, grant size varies by function. Three recurring patterns:

- **Engineering** is the baseline. Market benchmarks for engineering ICs at each level are the richest dataset (Carta, Pave, and Radford all report thick engineering bands).
- **Product management** typically bands close to engineering at equivalent level — some benchmarks run 5–15% lower at junior levels and converge at senior levels. <!-- needs-research: confirm current-market product-vs-engineering equity band ratios at IC levels in Carta Total Comp or Pave data. -->
- **GTM** (sales, SE, CS, marketing) is the function where OTE multiples and commission plans complicate the equity picture most. Equity grants for AEs are typically smaller as a percent of total comp than engineering at equivalent "level," because the AE's upside is intended to come from commission acceleration against quota. Sales leadership (Sales Manager, Director, VP) carries larger grants because the quota-acceleration mechanic falls away at the leadership tier. <!-- needs-research: current-market GTM equity grant bands at AE, Sales Manager, Director, and VP Sales levels. -->
- **G&A** (finance, legal, HR, IT) typically bands lower than engineering at equivalent IC level in most benchmark cuts. Where the role is a strategic hire (first Head of Finance, first GC), the grant is sized against the exec band, not the function band — see [chapter 04](./04-executive-compensation-packages.md).

The parts of the table where founder judgement, not benchmark data, is the dominant input:

- **First-of-its-kind roles.** The corporation's first designer, first DevRel, first platform engineer, first data engineer. Benchmark data at the "first X at this stage" granularity is sparse; the founder-CEO and the hiring manager are the primary inputs.
- **Critical-skill premiums.** A specific hard-to-find skill (foundation-model research, specific regulatory expertise, a named exec with a track record) justifies above-band equity. These should be documented as exceptions in the equity-grant log — not as changes to the table — so the comp committee can review exception density at the annual cycle.
- **Founder-adjacent roles.** Chief of Staff, first Head of People, first Business Operations hire. These roles are often sized by founder judgement because the "level" dimension does not map cleanly onto an IC ladder.

## Level differentiation

Three ladders typically coexist in a Series-B+ corporation.

### IC ladder (E1–E7 or equivalent)

A common engineering IC ladder: E1 (new-grad / associate), E2 (SWE), E3 (SWE II / mid), E4 (senior), E5 (staff), E6 (senior staff / principal), E7 (distinguished / fellow). Product and design have parallel ladders (P1–P5, D1–D5). The grant band at each level roughly doubles between adjacent levels at the mid-career tiers (E3 → E4 → E5), compresses at the top (E6 → E7), and anchors to the external market by level, not by title. The leveling rubric that assigns people to levels is a separate artifact from the grant-guideline table — see [chapter 06](./06-annual-comp-cycle.md) for the calibration cycle.

### Manager / director ladder (M1–M3, D1–D2)

Managers typically sit between two IC levels on the grant band — an M1 (first-line engineering manager) is often banded between E4 and E5. The convention varies; some corporations run manager grants at a slight premium to the "equivalent IC level" and some run at a slight discount with the rationale that the manager career path is lower-variance than the IC path. The corporation should pick a convention and stick with it; mid-cycle changes to the convention are visible to the whole org inside two weeks.

### Exec ladder (VP / SVP / C-suite)

Executive grants are a different animal and are not covered by the same grant-guideline table. Executive compensation layers (a) a materially higher cash band, (b) a materially larger equity grant, (c) a performance-based grant component (performance RSUs, milestone options, or a performance multiplier on standard options) at Series-B+, (d) a change-of-control acceleration policy (single- or double-trigger — see [chapter 07](./07-change-of-control-equity-policy.md)), and (e) a severance / release package ([chapter 08](./08-executive-severance-and-release.md)). The comp committee owns the executive-comp band directly — see [chapter 05](./05-compensation-committee.md) — and [chapter 04](./04-executive-compensation-packages.md) builds out the executive-comp package in depth. The IC grant-guideline table should stop at the VP line and defer upward.

## Who authors the table at each stage

The authorship pattern follows the governance maturity of the corporation.

- **Pre-seed / seed.** The founder-CEO drafts, often with input from a seed-stage comp advisor or a lead investor's platform team. There is no comp committee; the board as a whole approves grants above a threshold (the equity-plan administrator role is still the full board, acting under the equity plan).
- **Series-A.** The founder-CEO plus the CPO or Head of People (if that hire has been made) co-author. An outside comp advisor — a fractional engagement with Compensia, Pave's advisory arm, or an independent consultant — is engaged for the first market-benchmarked band build. The board compensation committee may be formed at the Series-A if the investor documents require it; if not, the board as a whole continues to ratify.
- **Series-B+.** The comp committee is a formal subcommittee of the board. The Head of People or Head of Total Rewards drafts; a Compensia or Radford advisor supplies peer-group analysis and recommends adjustments; the comp committee ratifies the table at the annual compensation cycle (see [chapter 06](./06-annual-comp-cycle.md)) and ratifies exceptions outside the cycle. The committee's charter, membership, and operating rhythm are the subject of [chapter 05](./05-compensation-committee.md).

The ownership-boundary map in [chapter 10](./10-ownership-boundary-map.md) is the one-page artifact that names who-does-what across the full equity-compensation stack; the grant-guideline table is one row on that map.

## A worked example — Fallstreak Networks, Series-B

Fallstreak Networks is a fictional Series-B infrastructure-software corporation. It raised a $45M Series-B eleven months ago at a $280M post-money valuation. Headcount is 112, split roughly 55 engineering / 12 product / 8 design / 28 GTM / 9 G&A. The corporation uses Carta for cap-table and equity administration, Pave for comp benchmarking, and has a quarterly 409A valuation (current FMV: $4.80 per share on a ~58M fully-diluted share count). The option pool was topped up at the Series-B to 12% of post-money fully diluted; approximately 42% of the post-top-up pool is unallocated. A compensation committee was formed at the Series-A and has three members (two independent directors, one investor director); it meets quarterly plus ad hoc for exception approvals.

The Head of People (hired six months post-Series-B) and a Compensia advisor drafted the Series-B grant-guideline table below. The comp committee ratified the table at its most recent quarterly meeting, with a next review at the annual compensation cycle in Q1 of the next fiscal year.

### Engineering IC — initial-hire grants

| Level | Target base ($) | Equity grant (dollar-value at current FMV) | Approx. share count |
|---|---|---|---|
| E3 | <!-- needs-research: Pave/Carta Series-B E3 engineer base --> | <!-- needs-research: Pave/Carta Series-B E3 equity grant dollar-value band --> | computed from grant $ / $4.80 |
| E4 | <!-- needs-research: Pave/Carta Series-B E4 engineer base --> | <!-- needs-research: Pave/Carta Series-B E4 equity grant dollar-value band --> | computed |
| E5 | <!-- needs-research: Pave/Carta Series-B E5 engineer base --> | <!-- needs-research: Pave/Carta Series-B E5 equity grant dollar-value band --> | computed |
| E6 | <!-- needs-research: Pave/Carta Series-B E6 engineer base --> | <!-- needs-research: Pave/Carta Series-B E6 equity grant dollar-value band --> | computed |

### Product and design IC — initial-hire grants

| Level | Equity grant (dollar-value at current FMV) | Notes |
|---|---|---|
| P3 | <!-- needs-research: current-market P3 equity grant at Series-B --> | Banded against E3; convention is -5% at mid-career, parity at senior. |
| P4 | <!-- needs-research: current-market P4 equity grant at Series-B --> | Banded against E4. |
| P5 | <!-- needs-research: current-market P5 equity grant at Series-B --> | Banded against E5. |

### GTM — initial-hire grants

| Role | Base ($) | OTE ($) | Equity grant (dollar-value at current FMV) |
|---|---|---|---|
| AE (enterprise) | <!-- needs-research: Series-B AE base --> | <!-- needs-research: AE OTE --> | <!-- needs-research: AE equity grant at Series-B --> |
| SE | <!-- needs-research --> | <!-- needs-research --> | <!-- needs-research --> |
| Sales Manager | <!-- needs-research --> | <!-- needs-research --> | <!-- needs-research --> |
| Director, Sales | <!-- needs-research --> | <!-- needs-research --> | <!-- needs-research --> |

### G&A — initial-hire grants

| Role | Level | Equity grant (dollar-value at current FMV) |
|---|---|---|
| Senior Finance IC | M3-equivalent | <!-- needs-research --> |
| Senior Legal IC | M3-equivalent | <!-- needs-research --> |
| HR Business Partner | M3-equivalent | <!-- needs-research --> |
| Director, Finance | D1 | <!-- needs-research --> |
| Director, Legal | D2 | <!-- needs-research --> |

### Exception thresholds

- Hiring manager may land anywhere inside the band without approval.
- Grant above the band ceiling by up to 25% requires Head of People approval.
- Grant above the band ceiling by 25–50%, or any grant at a level not in the table (new function, first-of-its-kind role), requires founder-CEO + Head of People approval.
- Any grant above the band ceiling by 50% or any grant to a VP-level or above requires compensation-committee approval. Exec grants are off this table — see [chapter 04](./04-executive-compensation-packages.md).

### Benchmark cadence

Compensia refreshes the Series-B peer-group analysis annually; Pave data is pulled quarterly for mid-cycle calibration. The comp committee reviews the full table once per year at the Q1 annual compensation cycle (see [chapter 06](./06-annual-comp-cycle.md)) and ratifies exception density as a standing agenda item at each quarterly meeting.

## Summary

- The grant-guideline table is the single artifact that turns equity into a reproducible decision and the first artifact a comp committee asks for. Four problems — manager consistency, dilution control, equity-vs-cash philosophy, and benchmarking discipline — collapse into it.
- The table has four axes (function, level, stage, grant size). The representation unit should be **percent-of-fully-diluted at pre-Series-B** and **dollar-value at the current 409A FMV at Series-B+**. Share-count is the instrument the equity-admin system issues; dollar-value is how the market reports; percent-of-fully-diluted is how the pool is budgeted. The IRC § 422(d) ISO $100k limit sits on top of all three representations.
- Initial grants are the largest grant an IC ever receives; refresh, promotion, and retention grants are additive and smaller — see [chapter 03](./03-refresh-promotion-and-retention-grants.md).
- Function differentiation at the same level is real (engineering as the baseline, product near parity, GTM lower-equity / higher-commission, G&A typically lower except for strategic hires). First-of-its-kind roles and critical-skill premiums are where founder judgement — documented as exceptions — displaces benchmark data.
- Authorship escalates with governance maturity. Founder-CEO at seed; founder-CEO + CPO / Head of People + outside advisor at Series-A; Head of People / Head of Total Rewards drafts and comp committee ratifies at Series-B+ (see [chapter 05](./05-compensation-committee.md)).
- The equity-economics side — pool sizing, pool refresh math, waterfall interaction, 409A mechanics, Rule 701 secondary programs — is owned by `startup-finance-fundraising-curriculum`. This chapter owns the grant-policy side. The handoff is the pool-utilization forecast that the Head of Finance and the Head of People co-own.
