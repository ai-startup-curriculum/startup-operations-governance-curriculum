# Exercise 03 — Benchmarking source selection by stage

> Estimated time: **~4 hours** · Related chapter: [03 — Benchmarking data sources by stage](../03-benchmarking-data-sources-by-stage.md)

## Problem statement

Resolute Signals, Inc. is a Delaware C-corp building an IoT data-pipeline platform for fleet operators. The corporation is nearing the end of a long Series-A runway (closed 26 months ago at a $34M post-money) and is three to four months out from opening a Series-B process. Headcount is **54 employees**: 24 engineering, 6 product / design, 14 GTM (including a Head of Sales hired six months ago from a sector-adjacent Series-C competitor), 7 G&A, and 3 operations.

Benchmarking state today:

- **The founder-CEO and Head of People have been relying on Carta Total Comp** since the corporation was 12 employees. Carta data is free as part of the cap-table subscription. The sample sizes at the corporation's stage cut (US Series-A, 50–100 FTE, technology) are usable for engineering IC levels E2–E4 but thin above E5 and thin for most non-engineering functions.
- **A one-off Pave subscription** was turned on nine months ago at the Head of People's request, specifically because the new Head of Sales walked in from a corporation with Compensia-benchmarked packages and the Carta GTM data was inadequate to defend the counter-offer. The Pave subscription has not been systematically renewed; it has been used ad hoc for three subsequent GTM hires and one engineering management hire.
- **The founder-CEO's board has, at the last two meetings, floated retaining Compensia** for the comp-committee work the Series-B will require. The founder-CEO has resisted on cost (Compensia's retainer is materially above the Pave subscription) and on the implicit signal to the board that "we are now a Compensia-stage company."
- **Three specific mis-sized offers** the Head of People has flagged in the last six months:
  1. **An E6 (Principal Engineer, Platform)** hired four months ago was sized against the Carta E5 → E6 cut at Series-A tech; the hire's current peer-review-visible compensation inside the corporation is now ~18% below the Pave Series-A tech E6 median. The hire has been vocal internally about the gap. The Head of People believes the Carta sample size for E6 at Series-A was fewer than 30 corporations.
  2. **A Director of Product** offer currently being negotiated is sized against the Pave Series-A tech cut; a competing offer the candidate has shared from a Series-C sector-adjacent corporation is ~12% higher. The candidate's recruiter has anchored on Radford Global Technology Survey percentiles the corporation does not have access to.
  3. **A fractional GC-to-full-time-GC conversion** — the fractional GC has offered to convert to a 60% full-time role at a conversion package neither the founder-CEO nor the Head of People can defend against any benchmark source they currently access (Carta's GC sample is empty at Series-A; Pave's is thin).
- **A pending Series-B diligence** will ask, among other things, for the benchmarking source the corporation uses, the sample sizes at the stage cut, the supplementation rule, and the comp-committee's documented reliance on the source.

Your role: you are the **Head of People** tasked with authoring the benchmarking-source decision the corporation will take forward into Series-B. Produce the current-state source audit, the by-stage source-selection decision, the supplementation rule, the tool-stack-and-vendor-management plan, and the comp-committee presentation memo.

## Requirements

### Part A — Current-state source audit

Produce a written audit of the current benchmarking state the comp committee can read in one sitting. Cover:

1. **Source-by-source inventory.** For each benchmarking source the corporation currently uses or accesses (Carta Total Comp, Pave, the Head of Sales's residual Compensia-exposure knowledge, any recruiter-shared Radford data), state:
    - The access path (free tier, paid subscription, consulting engagement, informal).
    - The stage cut the source supports (seed, Series-A, Series-B, growth, public).
    - The functions the source covers adequately at the corporation's stage (engineering IC, engineering management, product, design, GTM, G&A, exec).
    - The sample-size constraint — specifically, the levels and functions where the sample is thin at the current stage cut. Flag `<!-- needs-research -->` for specific sample-size numbers.
2. **The three mis-sized offers.** For each (the E6 platform hire, the Director of Product negotiation, the fractional-GC conversion), diagnose the source-selection failure:
    - Which source was used, and which should have been?
    - Where did the sample-size constraint bite?
    - What supplementation would have caught the gap before the offer letter went out (or, for the GC conversion, before the fractional engagement started)?
3. **The vendor-drift pattern.** Chapter 03 names the pattern where corporations accrete subscriptions over time without rationalising them (free Carta + paid Pave + ad hoc Radford pulls + founder-remembered Compensia numbers + a recruiter-provided data point). Diagnose whether Resolute Signals is already in the pattern.

### Part B — By-stage source-selection decision

Produce the source-selection decision the comp committee will ratify for the Series-B transition and the next 18 months. Cover:

1. **The stage-cut map.** Chapter 03 recommends a default stage-cut ladder — Carta and Pave at seed → Series-B; Radford and Compensia at Series-B → growth; and Advanced-HR / Option Impact as a cross-check at Series-B+. State Resolute Signals's chosen ladder with the specific transitions:
    - Which source is the **primary** at the current Series-A → Series-B window?
    - Which source becomes primary at Series-B close?
    - Which source becomes primary at Series-C / pre-IPO?
    - Where does each cross-check sit?
2. **The specific vendor-selection decisions.** For the Series-B-close transition:
    - **Compensia retainer — yes or no?** State the decision with justification. If yes, state the scope (comp-committee advisory, peer-set construction, annual market-data refresh, exec-comp calibration). If no, state the alternative (continue Pave + add Radford Global Technology Survey subscription + retain an outside advisor for exec-comp only).
    - **Pave continuation — yes or no?** State the decision. If yes, state the primary use (band-management, cycle execution, pay-transparency-compliance posting data). If no, state the migration path.
    - **Carta continuation — yes or no?** State the decision. Chapter 03 notes Carta becomes thin above Series-B; the usual answer is "continue for cap-table and 409A but retire as the primary comp benchmark."
    - **Radford Global Technology Survey subscription — yes or no?** State the decision. Note the per-year retainer cost (`<!-- needs-research -->`) and the sample-size advantage at senior IC levels and exec.
3. **The exec-comp cut.** State the specific source the corporation will use to size exec packages (CFO, CRO, CPO, GC) going forward. Chapter 03 points to Compensia and Radford as the two defensible options at Series-B pre-IPO; Pave and Carta are typically inadequate at the exec cut. Flag `<!-- needs-research -->` on the specific sample-size argument.
4. **The decision's tie-in to the comp-committee charter.** Cross-reference [mod-105 chapter 05](../../mod-105-equity-compensation-policy-and-comp-committee/05-compensation-committee.md) for the independent-compensation-consultant retention that becomes a comp-committee requirement at Series-B / pre-IPO.

### Part C — Supplementation rule

Produce the supplementation rule — the explicit trigger for pulling a second source. Cover:

1. **The sample-size trigger.** State the sample-size threshold below which the primary source is deemed inadequate and a second source is pulled. Chapter 03 recommends a default (typically 30–50 corporations in the peer cut at the stage / function / level). Flag the specific number with `<!-- needs-research -->`.
2. **The function-coverage trigger.** State the functions for which the primary source is deemed inadequate at Resolute Signals's stage *regardless of sample size* — typically exec, specialty engineering (ML / security / applied research at scarcity premium), and new-function first hires (GC, Head of Finance, Head of People at scale).
3. **The variance-tolerance trigger.** State the between-source variance threshold at which the comp committee must review the supplementation choice — e.g., if the Pave midpoint and the Compensia midpoint for the same function and level differ by more than 15%, the comp committee reviews which source anchors the band. Flag the specific percentage with `<!-- needs-research -->`.
4. **The documented-supplementation record.** State what gets captured in the equity-grant log and the band-authoring record every time a supplementation decision is made — the levels / functions supplemented, the sources used, the variance observed, the Head of Total Rewards' selection rationale. Cross-reference [chapter 04](../04-annual-comp-cycle.md) for the annual-cycle integration.

### Part D — Tool-stack and vendor-management plan

Produce the tool-stack and vendor-management plan. Cover:

1. **The band-management tool.** Chapter 03 names Figures, Pequity, and Assemble as the Series-B-era band-management tools. State the selection (or a defensible "no dedicated tool yet; Pave suffices at 54 FTE") with justification. If a tool is adopted, state the integration path with the HRIS (see [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md)) and the market-data source.
2. **The vendor-management rhythm.** State the per-vendor review cadence (annual contract renewal, mid-year sample-size check, quarterly data-refresh review), the owner (Head of Total Rewards post-Series-B split), and the budget line.
3. **The data-access rhythm.** State who inside the corporation can pull data from each source directly, who is the single point of truth (the Head of Total Rewards; recruiters pull *reports*, not raw queries), and the data-handling policy (benchmark data is confidential; comp-cycle pulls are retained in the HRIS or GRC tool, not in Google Drive).
4. **The vendor exit cost.** For each vendor, state the exit cost — contract termination notice, data retention post-cancellation, portability of the band artifacts. Chapter 03 notes that Pave's band-management artifacts are generally portable; Compensia's engagement-specific artifacts are less so.

### Part E — Comp-committee presentation memo

Produce the **1-page memo** attaching the benchmarking-source decision and submitted to the comp committee for ratification. Cover:

- The current-state audit headline (Part A) — the three mis-sized offers and the vendor-drift pattern.
- The by-stage source-selection decision (Part B) — the primary source at Series-A → Series-B, the Series-B-close transition, and the Series-C forward-look.
- The specific comp-committee asks: ratify the source ladder, ratify the Compensia-retention-or-not decision, ratify the supplementation rule.
- The budget implication — the delta between the current spend (free Carta + Pave) and the proposed spend (Pave + Radford + Compensia, or whatever the Part B decision is).
- The three forward-dependencies: the band file this source stack feeds ([chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md)), the annual cycle it powers ([chapter 04](../04-annual-comp-cycle.md)), and the pay-transparency postings it supports ([chapter 05](../05-pay-transparency-compliance.md)).
- The `<!-- needs-research -->` queue grouped by decision (sample-size thresholds, variance-tolerance percentages, Compensia retainer cost, Radford subscription cost).

## Starter guidance

- Chapter 03 is the primary reference. Re-read the "sources by stage," "sample-size constraint," "supplementation rule," and "band-management tool" sections before authoring.
- The vendor-selection decision is not just a cost comparison. Compensia's reputation with institutional investors and the ISS / Glass Lewis proxy-advisor ecosystem materially changes the Series-C / pre-IPO diligence experience. Factor that into the Part B decision; do not bury it in the budget line.
- The three mis-sized offers in the problem statement are the test cases. The E6 platform hire is the "thin-sample at the level cut" case; the Director of Product is the "competing-offer anchor to a source we do not access" case; the fractional-GC conversion is the "no source at this function at this stage" case. Each fits a different part of Part B's source ladder.
- **Do not manufacture market numbers or vendor pricing.** Every sample-size threshold, every variance-tolerance percentage, every vendor retainer cost must be flagged `<!-- needs-research -->`.
- The decision's tie-in to the comp-committee charter and the independent-comp-consultant retention requirement is the Series-B hinge. Cross-reference [mod-105 chapter 05](../../mod-105-equity-compensation-policy-and-comp-committee/05-compensation-committee.md) explicitly rather than re-authoring the charter mechanics.

## Deliverables

- `current-state-source-audit.md` — Part A.
- `by-stage-source-selection.md` — Part B.
- `supplementation-rule.md` — Part C.
- `tool-stack-and-vendor-management.md` — Part D.
- `comp-committee-memo.md` — Part E (1 page).

## Acceptance criteria

The package is acceptable if:

1. Part A inventories every current benchmarking source with access path, stage cut, functions covered, and sample-size constraint; diagnoses each of the three mis-sized offers to a specific source-selection failure; and diagnoses whether Resolute Signals is in the vendor-drift pattern.
2. Part B states the specific primary / secondary source choice at Series-A → Series-B, at Series-B close, and at Series-C / pre-IPO, with a documented Compensia-retention-or-not decision, a Pave-continuation decision, a Carta-retention decision, and a Radford Global Technology Survey decision.
3. Part C states the sample-size trigger, the function-coverage trigger, the variance-tolerance trigger, and the documented-supplementation record requirements, with `<!-- needs-research -->` on every specific threshold.
4. Part D states the band-management-tool selection (or defensible "not yet"), the vendor-management rhythm, the data-access rhythm, and the vendor exit cost for each vendor.
5. The comp-committee memo is **one page**, names the three mis-sized offers, the three ratification asks, the budget delta, and the `<!-- needs-research -->` queue.
6. Every sample-size threshold, every variance-tolerance percentage, every vendor retainer cost, and every function-coverage claim is flagged with `<!-- needs-research -->`. No invented numbers.
7. Cross-references to [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md), [chapter 04](../04-annual-comp-cycle.md), [chapter 05](../05-pay-transparency-compliance.md), [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md), and [mod-105 chapter 05](../../mod-105-equity-compensation-policy-and-comp-committee/05-compensation-committee.md) are present.
8. Nothing left as `[TBD]` or `[FILL IN]`.
