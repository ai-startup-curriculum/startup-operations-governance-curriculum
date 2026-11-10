# Exercise 02 — Cash and equity band authoring by geography

> Estimated time: **~5 hours** · Related chapter: [02 — Cash-and-equity bands per level per geography](../02-cash-and-equity-bands-per-level-per-geography.md)

## Problem statement

Austerlitz Robotics, Inc. is a Delaware C-corp building a software control plane for industrial-automation cells. The corporation closed a $62M Series-B eleven months ago at a $320M post-money and is actively distributed: **168 employees** across the US and a small UK bridgehead. Current headcount by geography:

- **San Francisco Bay Area (24)** — most of the founding engineering team, the CTO, and the applied-research group.
- **New York City (22)** — the Head of Sales, the Enterprise AE pod, and a satellite engineering cell.
- **Seattle, WA (14)** — a platform-engineering subteam and the Head of Design.
- **Boston, MA (9)** — two founding product managers and a small ML-engineering subteam.
- **Austin, TX (18)** — a growing sales-development group and an operations / finance subteam.
- **Denver, CO (11)** — a mix of product-engineering and customer-success roles.
- **Remote US, tier-2 metros (48)** — Nashville, Pittsburgh, Raleigh, Minneapolis, Salt Lake City, Columbus, Portland (ME), Portland (OR), and a long tail of smaller markets.
- **Remote US, tier-3 and rural (16)** — the balance.
- **London, UK (6)** — the corporation's first international hires, all Senior Engineer or Enterprise AE tier, employed through an EOR while a UK Ltd. subsidiary is spun up.

Current state of the cash-and-equity bands:

- **A ratified job architecture** (from [exercise 01](./exercise-01-job-architecture-and-leveling-framework-authoring.md) and chapter 01) is in place. Every IC and manager carries a ratified level.
- **No ratified cash-and-equity bands.** Offers are currently built by the Head of People and the hiring manager in Pave against a "national SF-Bay-Area benchmark" for every hire regardless of geography, with ad-hoc downward adjustments the founder-CEO applies by feel for tier-2 and tier-3 markets. The equity sizing is anchored to the grant-guideline table ratified at [mod-105 exercise 01](../../mod-105-equity-compensation-policy-and-comp-committee/exercises/exercise-01-equity-grant-guideline-table-by-level-and-function-authoring.md).
- **Three specific anomalies** the Head of People has flagged this quarter:
  1. **A Denver, CO Senior Engineer (E4)** was paid at a Bay-Area-median base; the hiring manager stretched the band on the rationale that "remote tier-2 is only 7% below SF." The subsequent CO pay-transparency posting carried the Bay-Area number. The Division of Labor has not raised a complaint, but a Reddit thread calling out the posting has 240 upvotes.
  2. **A Boston, MA ML Engineer (MLE4)** was hired at a base **12% above** the Bay-Area band midpoint for the equivalent engineering level. The hiring manager cited "Boston-ML scarcity premium." No documentation of the premium exists.
  3. **A London Enterprise AE** is being hired at a base pegged to the NYC Enterprise AE band. The founder-CEO has verbally committed to the hire. The Head of People believes the UK base is materially above the UK-market band and that the EOR provider will struggle to defend the spread at renewal.
- **A pending Series-C process** in nine to twelve months and a people-diligence Severity-2 finding from the Series-B's operating partner — "no geo-tiered pay strategy, no documented band widths, no compression / inversion diagnostic" — are both forcing functions.

Your role: you are the **Head of Total Rewards** (the role was split out from Head of People at Series-B close) tasked with authoring the first ratifiable cash-and-equity band file. Produce the geographic-tier strategy decision, the band widths and midpoint-target policy, the per-geography band table, the compression-and-inversion diagnostic against the current comp file, the UK bridgehead policy, and the comp-committee presentation memo.

## Requirements

### Part A — Geographic-tier strategy decision

Produce a written strategy decision for the comp committee. Cover:

1. **The four defensible strategies** chapter 02 names — **national-single-band**, **tier-1-and-national**, **cost-of-labor-tiered**, and **cost-of-living-tiered** — with a one-paragraph description of each.
2. **Austerlitz's pick.** State the chosen strategy with a defensible rationale against the current 168-employee footprint. Justify the choice against (a) the specific geographies in-footprint, (b) the Series-C diligence forward-look, (c) the pay-transparency statutes in CA / CO / WA / NY / IL (`<!-- needs-research: current statute-matrix cut for tier coverage requirements -->`), and (d) the operational burden on the Head of Total Rewards.
3. **The tier definitions.** Define the specific tiers under the chosen strategy — e.g., Tier 1 (SF Bay, NYC), Tier 2 (Seattle, Boston, Washington DC, LA), Tier 3 (Austin, Denver, Chicago, Atlanta, Portland OR), Tier 4 (national remote outside the above) — and the metropolitan-statistical-area (MSA) mapping convention the Head of Total Rewards will use. Flag the specific tier-differential percentages with `<!-- needs-research -->` against the Radford or Mercer or Compensia geo-differential cut the corporation will reference.
4. **The anchor-percentile choice.** State the band-midpoint anchor — 50th percentile of the chosen peer set, 60th percentile, or 75th percentile — and justify the choice against Austerlitz's competitive-hiring posture and the corporation's current burn / retention state. Chapter 02 will name a default (typically 50th at seed → 60th at Series-B for engineering, 50th for non-scarce functions); flag the specific percentile claim with `<!-- needs-research -->`.
5. **The explicit "no" list.** State what Austerlitz is explicitly *not* doing — no cost-of-living-only tiering (COL is a weak proxy for cost-of-labor), no individual-negotiation-based geo tiering (every hire in a tier gets the tier's band), no "we match wherever you move" policy (geo tier is reset at the next offer-letter-equivalent event — promotion, re-location, or new hire).

### Part B — Band widths and midpoint-target policy

Produce the band-width design. Cover:

1. **The band width.** State the band width (typically 20–40% from floor to ceiling, with a midpoint at the anchor percentile) and the width's variation by level (narrower at junior levels — 20–25%; wider at senior levels — 30–40%). Flag the specific percentages with `<!-- needs-research -->` against the chosen benchmark source.
2. **The midpoint-target policy.** State whether a new hire's starting base targets the floor (default for new-grad / junior levels, leaving headroom for in-band progression), the midpoint (default for senior / staff hires), or the ceiling (reserved for named-expert / scarce-skill premiums with documented justification). Specify the manager-discretion range inside which no approval is required and the above-ceiling approval path (Head of Total Rewards + founder-CEO; above a higher threshold, comp committee chair).
3. **The equity-band mirror.** For each level, state the equity band — floor / midpoint / ceiling expressed as (a) dollar-value at the current 409A FMV, (b) percent-of-fully-diluted, and (c) share count. Cross-reference [mod-105 chapter 01](../../mod-105-equity-compensation-policy-and-comp-committee/01-grant-guidelines-by-level-and-function.md) for the equity-grant-guideline table the band inherits.
4. **The band-widening trigger.** State the diagnostic that triggers a band-widening review — a cluster of above-ceiling exceptions in the last cycle (the "every hire is a ceiling hire" pattern), or a cluster of below-floor retentions (the "no one wants to join at the current band" pattern) — and the ratification path for a band revision.

### Part C — Per-geography band table

Produce the per-geography band table that the Head of Total Rewards will operate the comp system against for the next cycle. Cover, at minimum:

1. **Engineering IC** — E2, E3, E4, E5, E6. Base-salary floor / midpoint / ceiling for each tier (Tier 1 / Tier 2 / Tier 3 / Tier 4 / UK). Flag every midpoint with `<!-- needs-research -->` specifying the source (Carta Total Comp, Pave, Compensia, Advanced-HR, Radford Global Technology Survey), the stage cut (Series-B tech), the function, the level, the geography, and the vintage.
2. **Engineering management** — M4 first-line, M5 senior manager, D1 director. Same floor / midpoint / ceiling by tier.
3. **Product, Design, Data / ML, Marketing, CS** — the equivalent IC bands at each level. Note the function-vs-engineering ratio (product tends 5–15% below engineering at junior levels and converges at senior levels per chapter 01; design tends to match engineering; data / ML tends at parity or slightly above). Flag the ratios with `<!-- needs-research -->`.
4. **GTM** — AE, Senior AE, Enterprise AE, Strategic AE, Sales Manager, Director of Sales, VP Sales, SDR / Senior SDR / SDR Manager, SE1 / SE2 / Senior SE. Note that GTM base is typically a smaller portion of total cash than engineering (the OTE is the full picture; base is a line in a larger plan). Cross-reference [chapter 07](../07-sales-comp-plan-design.md) for the OTE / commission mechanics.
5. **G&A** — Finance (Analyst, Senior Analyst, Manager, Director, VP), Legal (Counsel, Senior Counsel, Managing Counsel, Deputy GC, GC), People (Manager, Director, VP), IT (Manager, Director). Note that first-of-its-kind strategic hires (first in-house GC, first Head of Finance, first Head of People at scale) are sized against the exec band and not the function band; cross-reference [mod-105 chapter 04](../../mod-105-equity-compensation-policy-and-comp-committee/04-executive-compensation-packages.md).
6. **UK bands.** State the UK equivalent of each US tier (typically London-proximity treated as UK Tier 1; Manchester / Edinburgh / regional as UK Tier 2) with the pound-sterling bands. Flag `<!-- needs-research -->` for the UK-cut source (Radford UK, Figures, or a UK-specific Compensia pull).

### Part D — Compression and inversion diagnostic

Produce the diagnostic against the current comp file. Cover:

1. **Compression definition.** Define compression (two ICs at different levels inside a band whose base-salary spread is smaller than the band width — e.g., an E3 and an E4 within 4% on base when the between-level midpoint spread should be 15–20%).
2. **Inversion definition.** Define inversion (a junior IC whose base is above a more-senior IC's base — the direct-pay symptom of promotion inflation plus merit-inertia).
3. **The scan.** Scan the current 168-employee comp file against the newly authored bands (Part C). Report, by function and by tier:
    - Every compression instance (name the two levels and the pattern, not the individual).
    - Every inversion instance (name the two levels and the pattern).
    - The specific remediation disposition for each — merit-adjustment at the next cycle, promotion if scope warrants, exception-documented-and-accepted, or termination-eligibility review.
4. **The three flagged anomalies.** Each of the three anomalies in the problem statement — the CO E4 paid at Bay-Area median, the MA MLE4 at 12% above Bay-Area midpoint, the pending London Enterprise AE — gets an explicit diagnosis (compression? inversion? above-ceiling exception? band-strategy violation?) and a specific remediation disposition.
5. **The named-pattern check.** Chapter 02 names a handful of recurring failure patterns — geographic-arbitrage drift (hires negotiated against SF bands then relocated to lower-tier markets without a band reset), tenure-inversion (long-tenured IC at or below the floor the newly hired peer landed at), cross-function inversion (a GTM OTE exceeding the engineering total cash at the equivalent level). Scan for each pattern at Austerlitz and report with evidence.

### Part E — UK bridgehead policy

Produce the UK-specific policy. Cover:

1. **The EOR-vs-subsidiary bridge.** The six UK hires are currently on an EOR. State the policy for the bridge window (how long the EOR runs before the UK Ltd. subsidiary takes over as the employer-of-record) and the hand-off conditions. Cross-reference [mod-113](../../mod-113-international-expansion-and-global-workforce/) for the international-expansion operating model.
2. **UK tier definition inside Austerlitz's strategy.** State whether UK Tier 1 (London) maps to US Tier 1 or US Tier 2 in the band strategy, with the differential driven by UK-market data not US-market data. Flag `<!-- needs-research -->` for the UK-vs-US differential at each level the corporation hires at.
3. **The pending London Enterprise AE.** Specifically disposition the hire — is the base the founder-CEO verbally committed to above the UK Tier 1 ceiling? If yes, is the premium justified by documented skill scarcity, or is it an above-ceiling exception that needs comp-committee ratification before the offer letter goes out? If no, the hire proceeds; if yes, state the three options (rescind-and-renegotiate, ratify-with-documented-premium, re-slot-to-a-US-geo).
4. **The EU Pay Transparency Directive forward-look.** Note the 2026-06-07 transposition deadline and the readiness requirement: documented objective gender-neutral criteria for role evaluation, published pay-band information on request to candidates and employees, gender-pay-gap reporting if the UK Ltd. subsidiary ever carries ≥100 workers. Cross-reference [chapter 05](../05-pay-transparency-compliance.md) for the full directive readiness plan.

### Part F — Comp-committee presentation memo

Produce the **1-page memo** attaching the band file and submitted to the comp committee for ratification. Cover:

- The chosen geographic-tier strategy (Part A), the band width and midpoint-target policy (Part B), and the headline anchor percentile.
- The three flagged current-comp anomalies (Part D), the dispositions proposed, and the `<!-- needs-research -->` queue grouped by function and geography.
- The UK bridgehead policy (Part E) and the specific disposition of the pending London Enterprise AE hire.
- The three asks the comp committee is being asked to ratify — the geo-tier strategy, the per-geography band table, and the exception-workflow + above-ceiling approval path.
- The forward-references to [chapter 03](../03-benchmarking-data-sources-by-stage.md) (benchmarking source selection), [chapter 04](../04-annual-comp-cycle.md) (the cycle the bands drive), [chapter 05](../05-pay-transparency-compliance.md) (the posting obligations the bands enable), and [chapter 08](../08-comp-architecture-failure-modes.md) (the failure-mode library the diagnostic in Part D anticipates).

## Starter guidance

- Chapter 02 is the primary reference. Re-read the "geographic-tier strategy," "band widths," "midpoint-target," "compression / inversion diagnostic," and "exception-workflow" sections before authoring.
- The geographic-tier decision is the first-order architectural choice. Do not let the discussion of specific tier percentages overwhelm the strategy question — pick the strategy (national / tier-1-and-national / cost-of-labor-tiered / cost-of-living-tiered), then populate the tiers.
- **Do not manufacture market numbers.** Every band midpoint, every tier differential, every function-vs-engineering ratio, every UK-vs-US differential must be flagged `<!-- needs-research -->` with the source (Radford, Compensia, Carta, Pave, Figures, Advanced-HR), the stage cut, the function, the level, the geography, and the vintage.
- The three flagged anomalies are the comp committee's anchor cases. The CO E4 posting is the regulatory-exposure case; the MA MLE4 is the premium-documentation case; the London Enterprise AE is the international-bridgehead case. Each disposition matters.
- The compression / inversion diagnostic in Part D is the artifact the Series-C diligence operating partner will ask for. Treat the scan as a first-class deliverable, not an appendix.
- The UK side defers substance to [mod-113](../../mod-113-international-expansion-and-global-workforce/). Do not re-author the EOR / subsidiary mechanics here; cite the module.

## Deliverables

- `geographic-tier-strategy.md` — Part A.
- `band-widths-and-midpoint-policy.md` — Part B.
- `per-geography-band-table.md` (or `.csv` / `.xlsx`) — Part C.
- `compression-inversion-diagnostic.md` — Part D.
- `uk-bridgehead-policy.md` — Part E.
- `comp-committee-memo.md` — Part F (1 page).

## Acceptance criteria

The package is acceptable if:

1. Part A picks one of the four defensible strategies, defines the specific tiers and MSA-mapping convention, states the anchor-percentile choice, and includes the "no" list.
2. Part B states the band widths (varied by level), the midpoint-target policy with manager-discretion range and above-ceiling approval path, the equity-band mirror cross-referenced to [mod-105 chapter 01](../../mod-105-equity-compensation-policy-and-comp-committee/01-grant-guidelines-by-level-and-function.md), and the band-widening trigger.
3. Part C's band table covers engineering IC (E2–E6), engineering management (M4–D1), product, design, data / ML, marketing, CS, the GTM ladder, and the G&A roles — in floor / midpoint / ceiling per tier (Tier 1 / Tier 2 / Tier 3 / Tier 4 / UK) with every midpoint flagged `<!-- needs-research -->`.
4. Part D's diagnostic reports every compression and inversion instance in the current 168-employee comp file, dispositions each of the three named anomalies, and scans for the named failure patterns (geographic-arbitrage drift, tenure-inversion, cross-function inversion).
5. Part E dispositions the pending London Enterprise AE with one of the three options (rescind-and-renegotiate, ratify-with-documented-premium, re-slot-to-a-US-geo), cross-references [mod-113](../../mod-113-international-expansion-and-global-workforce/) for the EOR / subsidiary mechanics, and names the EU Pay Transparency Directive transposition deadline (2026-06-07).
6. The comp-committee memo is **one page**, names the chosen strategy, the three flagged anomalies, and the three ratification asks, with the `<!-- needs-research -->` queue grouped by function and geography.
7. Every band number, every tier differential, every function-vs-engineering ratio, every UK-vs-US differential, and every anchor-percentile claim is flagged with a `<!-- needs-research -->` marker specifying source, stage cut, function, level, geography, and vintage. No invented percentages.
8. Cross-references to [chapter 03](../03-benchmarking-data-sources-by-stage.md), [chapter 04](../04-annual-comp-cycle.md), [chapter 05](../05-pay-transparency-compliance.md), [chapter 07](../07-sales-comp-plan-design.md), [chapter 08](../08-comp-architecture-failure-modes.md), [mod-105 chapter 01](../../mod-105-equity-compensation-policy-and-comp-committee/01-grant-guidelines-by-level-and-function.md), [mod-105 chapter 04](../../mod-105-equity-compensation-policy-and-comp-committee/04-executive-compensation-packages.md), and [mod-113](../../mod-113-international-expansion-and-global-workforce/) are present.
9. Nothing left as `[TBD]` or `[FILL IN]`.
