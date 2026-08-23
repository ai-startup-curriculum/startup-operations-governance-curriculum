# 1. The performance-management operating system

> A defensible cadence, a defensible format, calibration that survives the room, and a manager corps trained to write and deliver the review — anchored to the annual comp cycle that reads its output.

## Motivation

Performance management is the single people-ops instrument that touches every employee, every manager, every executive, every quarter — and the one most first-time COOs, heads-of-people, and GCs get wrong first. The failure mode is not "we forgot to run reviews." The failure modes are subtler and more expensive:

- Reviews run on no fixed cadence and land after comp decisions have already been made, so the review is decorative rather than load-bearing.
- Every manager writes reviews in a different format and every function calibrates on a different scale, so a "meets expectations" in Engineering means something different from a "meets expectations" in Sales and neither maps cleanly to the merit budget the comp cycle in mod-106 needs.
- Managers are asked to give hard feedback with zero training, they duck the hard message, and six months later they cannot open a PIP because there is no documented performance gap.
- The company buys Lattice / 15Five / Culture Amp / Betterworks at Series-Seed because a peer company did, spends a year fighting a workflow that does not match its operating cadence, and ends up back in a spreadsheet.

The purpose of a performance-management operating system is to make performance management **a boring, predictable, calendared operation** — anchored to the [annual comp cycle](../mod-106-compensation-architecture-and-total-rewards/04-annual-comp-cycle.md) so that ratings actually drive merit, promotion, and refresh decisions; standardised in format so that calibration is meaningful; supported by manager training so that hard conversations happen; and tooled at the level of maturity the company has actually reached.

## The five operating decisions

Every performance-management operating system answers five questions:

1. **Cadence.** How often do formal reviews run, when are they anchored, and what continuous-feedback loop runs between them?
2. **Format.** What inputs feed each review (self, manager, peer, upward, skip-level, 360), and how does the mix change by level?
3. **Calibration.** How does the corporation prevent rating inflation, cross-function drift, and manager-favouritism from polluting the merit / promotion signal?
4. **Manager training.** How does a first-time manager learn to write a review, deliver it, and follow through?
5. **Tooling.** In-house spreadsheet at seed, or a dedicated tool (Lattice, Culture Amp, 15Five, Betterworks) at what stage, at what cost, with what integration into HRIS and comp?

Each is a separate decision. Answering "we use Lattice" does not answer the cadence question, and answering "twice a year" does not answer the calibration question.

## Decision 1 — Cadence

The cadence has three layers.

**The formal review cadence.** The mainstream startup pattern is **semi-annual** formal reviews — a full review in Q4 (feeding the Q1 comp cycle) and a lighter mid-year checkpoint in Q2. A minority of companies run **annual** reviews only, but annual-only cadence tends to collide with fast-changing goals at Series-A / Series-B and delays the identification of performance gaps by six months. Quarterly formal reviews are common only in high-turnover functions (early-stage Sales) or at companies that have deliberately chosen a very-fast feedback culture — the operating cost of quarterly reviews for every employee is high and typically not worth it.

**The continuous informal cadence.** Formal reviews are lagging. Every people-ops function needs an *informal* cadence between formal reviews — a weekly 1:1, a monthly written check-in, or both — so that no surprise appears in a formal review that has not already been raised in a 1:1. The single most common source of PIP-and-termination litigation is a formal review or PIP that documents performance issues the employee is hearing about *for the first time*.

**The comp-cycle anchor.** The formal review has to close before the comp cycle in [mod-106 chapter 04](../mod-106-compensation-architecture-and-total-rewards/04-annual-comp-cycle.md) begins. The typical calendar:

- **October–November:** self-reviews and peer-reviews open; managers begin writing manager reviews.
- **Late November:** calibration meetings (see decision 3).
- **December:** final ratings locked; managers deliver reviews to reports.
- **January–February:** comp cycle runs — merit, equity refresh, promotion — using the ratings as the primary input.
- **March–April:** compensation statements delivered; promotion effective dates communicated.

A review process that lands *after* the comp cycle is decorative — the merit budget was allocated on stale data. Anchor the review process to the comp cycle before choosing anything else.

## Decision 2 — Format

The review format is not one thing; it is a mix of inputs, and the mix changes by level.

**The four canonical inputs:**

- **Self-review.** The employee writes a summary of accomplishments against their goals, an assessment against the corporation's competency framework (see [mod-106 chapter 01](../mod-106-compensation-architecture-and-total-rewards/01-job-architecture-and-leveling-framework.md)), a list of growth areas, and a career-conversation prompt. Standard for every level.
- **Manager review.** The manager writes a full assessment against goals and competencies, calibrates the employee against level expectations, produces a rating, and drafts development recommendations. Standard for every level.
- **Peer review.** The employee and manager together identify 3–5 peers who worked closely with the employee; peers submit structured feedback. Standard for IC roles from mid-level upward; often skipped for the most junior IC level where peer sample is too small.
- **Upward review / skip-level review.** Reports assess their manager (upward), and skip-level reports assess the second-line manager (skip-level). Standard for anyone with direct reports.

**360 reviews** — a fully-formalised process that gathers self + manager + peer + upward + skip-level input and often external stakeholders — are typically reserved for the most senior levels (VP / SVP / C-level) because they are expensive to run well. Running a full 360 for every level every review is the most common way to spend three months of the people-ops function's calendar and get diminishing return on the signal.

**The format-by-level pattern:**

| Level | Self | Manager | Peer | Upward | Skip-level | 360 |
|---|---|---|---|---|---|---|
| L1–L2 (IC junior) | ✓ | ✓ | (light) | — | — | — |
| L3–L5 (IC mid to senior) | ✓ | ✓ | ✓ | — | — | — |
| L4+ manager | ✓ | ✓ | ✓ | ✓ | — | — |
| L6+ second-line manager | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| VP+ / exec | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

Levels are labelled here per [mod-106 chapter 01](../mod-106-compensation-architecture-and-total-rewards/01-job-architecture-and-leveling-framework.md). Pick a format pattern deliberately, document it, and hold it stable — moving formats every cycle destroys year-over-year comparability.

**The rating scale.** The two dominant patterns:

- A **five-point scale** — often "Does Not Meet / Approaching / Meets / Exceeds / Greatly Exceeds Expectations." Common at Series-B and later.
- A **three-point scale** — "Below / At / Above expectations." Common at seed and Series-A because it forces managers to take a position and resists the "everyone is a 4 out of 5" inflation.

The three-point scale is easier to calibrate and easier to communicate; the five-point scale carries more resolution and pairs better with a formal merit-matrix in the comp cycle. Choose based on manager maturity and comp-cycle mechanics, not on what the tool defaults to.

## Decision 3 — Calibration

Uncalibrated ratings are worse than no ratings. Three failure modes to design against:

1. **Rating inflation.** Every manager wants to protect their people, and unless the corporation applies pressure, most rating distributions drift toward "Exceeds Expectations" for everyone.
2. **Cross-function drift.** Engineering's "Meets Expectations" becomes stricter than Sales's "Meets Expectations" (or vice versa), and the merit budget rewards the more lenient function.
3. **Manager favouritism / bias.** A single manager systematically over- or under-rates against demographic lines, and no one sees it because ratings are never compared side-by-side.

**The calibration meeting.** The standard mechanism is a **function-level calibration meeting** followed by a **cross-function calibration meeting**:

- **Function-level calibration.** All managers in a function (Engineering, Product, Sales, etc.) sit with their function head and the HRBP. Each manager walks through their proposed ratings for each report. The room challenges the distribution and specific ratings. The output is a function-level rating distribution that the function head signs off on.
- **Cross-function calibration.** Function heads plus the CEO and the head of people sit in a single room. Each function head presents their calibrated distribution and any borderline cases. The room re-anchors "Exceeds Expectations" across functions so that the meaning of a rating is comparable.

**Distribution guardrails.** The mainstream pattern is not a forced curve (the discredited Jack-Welch-era "rank-and-yank" model that the Wharton and MIT critiques of GE-era stack-ranking documented) but a **soft distribution guardrail**: a signal from the head of people that a function whose ratings distribute as 60% "Exceeds" and 40% "Greatly Exceeds" needs to explain itself. Guardrails without a mechanical curve preserve the ability to genuinely rate a strong team highly while catching runaway inflation.

**Anti-bias norms.** The calibration meeting should include a step that reviews ratings by demographic slice (gender, race / ethnicity, tenure, work-location) with the HRBP flagging patterns that warrant a second look. This is a pattern-detection step, not a quota mechanism; it exists to protect the corporation and the employee alike from unconscious bias baked into the ratings.

## Decision 4 — Manager training

Every people-ops function underinvests in this. The mainstream startup pattern is:

- **Review-writing training.** A one-hour workshop before each review cycle covering: how to write a specific, behaviour-anchored review (SBI — situation, behaviour, impact — as the default frame); how to distinguish outcome from effort; how to rate against the level rubric, not against the employee's tenure or likability; how to write a review that supports its rating (a "Meets Expectations" needs supporting evidence just as much as a "Does Not Meet" does).
- **Delivery training.** A one-hour workshop covering: how to deliver a review in a 30–45 minute 1:1; how to open ("I'd like to walk through your review — here's the summary rating, and I want to spend the time on why and what's next"); how to handle disagreement ("I hear you — this is my read of the evidence, and here is what would move the rating up over the next cycle"); how to close on the development plan and not on the rating.
- **Hard-conversation training.** A separate workshop, typically annual, covering: the difference between coaching and PIP-precursor conversations; how to give a "not-progressing" signal without triggering a resignation; how to document a coaching conversation so that if it escalates to a PIP the documentation is already in place; how to escalate to HRBP support early rather than late.

The manager-training curriculum is the single highest-ROI programme the people-ops function runs. A one-hour investment per manager per cycle prevents most of the downstream PIP-and-termination pain covered in [chapter 04](./04-pip-mechanics.md) and [chapter 05](./05-termination-playbook.md).

## Decision 5 — Tool selection

The tool decision is a function of stage, manager count, and integration burden — not a function of feature list.

**Pre-Series-A (≤~30 employees):** An in-house Google Sheet or Notion database is usually the right answer. The workflow is: a self-review template, a manager-review template, a peer-review Google Form, and a shared calibration sheet. Total cost: zero. Total effort: one afternoon of setup. This is not primitive — it is the right level of investment for the operating maturity, and it forces the head of people to design the cadence and format decisions above before offloading them to a tool.

**Series-A to Series-B (~30–150 employees):** Dedicated performance-tool selection becomes worthwhile. The three most common categories:

- **Continuous-feedback-first tools.** [Lattice](https://lattice.com/), [15Five](https://www.15five.com/), [Betterworks](https://www.betterworks.com/) — anchored around 1:1 agendas, goals / OKRs, and continuous feedback, with a formal-review module bolted on.
- **Engagement-first tools.** [Culture Amp](https://www.cultureamp.com/) — anchored around engagement surveys and pulse checks, with a formal-review module bolted on.
- **Compensation-integrated tools.** Some of the above (Lattice, Betterworks) offer comp-cycle modules that read the performance rating and drive merit / equity / promotion recommendations. Others (Figures, Pequity, Assemble — see [mod-106 chapter 03](../mod-106-compensation-architecture-and-total-rewards/03-benchmarking-data-sources-by-stage.md)) are comp-first and integrate with the performance tool via API.

**Series-B and beyond (~150+):** A full HCM (Workday, Dayforce, SuccessFactors) will typically include a performance module. Whether to use it depends on manager-experience quality — HCM performance modules are frequently less usable than dedicated performance tools, and many companies at this stage keep a dedicated performance tool alongside the HCM.

**The selection criteria to actually weight:**

1. **HRIS integration** (write ratings back into the employee record; pull org chart, level, and reporting-line data).
2. **Comp-cycle integration** (the tool feeds the comp cycle in [mod-106 chapter 04](../mod-106-compensation-architecture-and-total-rewards/04-annual-comp-cycle.md)).
3. **Manager UX** (a bad manager UX kills adoption; a great one raises review-completion rate meaningfully).
4. **Calibration-meeting workflow** (drag-and-drop rating comparison across a team is worth more than any single other feature).
5. **Data-export capability** (never buy a tool that will not export your data cleanly; you will change tools).

Buying a performance tool before the cadence / format / calibration / manager-training decisions are settled is the fastest way to spend $30k–$150k of annual license fees on shelfware.

## Concrete example: a Series-A operating system

A 60-person, Series-A B2B SaaS company. Twelve managers reporting into a five-person executive team. HRIS is Rippling; comp-cycle tool is Figures; performance tool is Lattice.

- **Cadence.** Formal review in November (feeding Q1 comp cycle); mid-year lightweight check-in in June. Weekly 1:1s using Lattice agendas; monthly written check-in in Lattice.
- **Format.** Self + manager for L1–L3; add peer for L4+; add upward for anyone with direct reports; skip-level and 360 not yet in scope (deferred to Series-B).
- **Rating scale.** Three-point (Below / At / Above expectations) with a fourth "Not Yet Rateable" for anyone in role fewer than 90 days.
- **Calibration.** Function-level meetings in the second week of November; cross-function meeting the third week of November, chaired by the head of people with the CEO in attendance. Ratings by demographic slice reviewed with the HRBP.
- **Manager training.** One-hour review-writing workshop the week before self-reviews open; one-hour delivery workshop the week before manager reviews are due; annual hard-conversation workshop in Q3, before formal-review season.
- **Tool.** Lattice for cadence, format, and calibration workflow; ratings sync to Rippling employee records via API; Figures pulls ratings into the merit / promotion budget model for the Q1 cycle.

This operating system runs in ~120 hours of head-of-people time per year, ~4 hours of manager time per report per cycle, and ~2 hours of employee time per cycle. It is boring and predictable, which is the point.

## Summary

- Performance management is five separate operating decisions — cadence, format, calibration, manager training, tooling — and they must be answered in that order.
- Anchor the cadence to the [annual comp cycle](../mod-106-compensation-architecture-and-total-rewards/04-annual-comp-cycle.md); a review that lands after comp is decorative.
- Match format to level; a full 360 for every employee is a common and expensive mistake.
- Calibrate at the function level and then across functions; add a demographic-slice review as an anti-bias norm.
- Invest in manager training every cycle; it is the highest-ROI programme the people-ops function runs.
- Buy a tool when the cadence / format / calibration / training decisions are already settled, not before. In-house spreadsheet is the right answer at seed; dedicated performance tool (Lattice / Culture Amp / 15Five / Betterworks) becomes worthwhile at Series-A → Series-B; HCM performance module at growth if manager UX holds up.
- See [exercise-01](./exercises/exercise-01-performance-management-operating-system-authoring.md) for the authoring drill.
