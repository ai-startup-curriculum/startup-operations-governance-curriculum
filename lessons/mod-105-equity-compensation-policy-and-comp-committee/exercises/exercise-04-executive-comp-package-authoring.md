# Exercise 04 — Executive comp package authoring

> Estimated time: **~5 hours** · Related chapter: [04 — Executive compensation packages](../04-executive-compensation-packages.md)

## Problem statement

Larksend Robotics is a Delaware C-corp building warehouse-automation hardware and the control-plane software that runs it. The corporation is ~300 employees today (170 engineering across hardware / firmware / software, 55 operations and manufacturing, 40 GTM, 25 G&A, 10 research) and is closing a $180M Series-C led by a growth fund with two existing investors following on. Post-money is sufficient to support a hired C-suite comp program at current-market bands. The board (two founder-directors, three investor-directors, one independent director — the comp-committee chair) is planning an S-1 filing roughly two years out, contingent on gross-margin and revenue durability.

The fractional CFO who carried the corporation through Series-B and the Series-C diligence is departing at Series-C close (announced). Two finalists are in play for the full-time CFO seat: Candidate A is a sitting public-company Chief Accounting Officer with S-1 and SOX-ramp experience; Candidate B is a sitting private-company CFO at a late-stage logistics corporation who has run a dual-track IPO / M&A process. Both candidates are willing to commit. Both have current comp packages that have been shared with Larksend's search firm. The comp committee has a working charter (reference chapter 05) and has retained Compensia for benchmarking against a 15-corporation peer set the committee approved last quarter.

Your role: you are the Head of People (or an outside operating advisor engaged by the comp-committee chair) tasked with authoring a defensible full-package proposal for the comp committee to review, approve, and recommend to the full board. The package must survive comp-committee scrutiny today, auditor and ISS / Glass Lewis scrutiny at S-1, and § 280G exposure analysis at a future change-of-control.

## Requirements

### Part A — Package architecture

Produce a written architecture of the CFO package. Cover:

1. **Base salary** — the target band and the specific number you are proposing, with benchmark citation (Compensia peer-set median / 60th / 75th percentile, cross-check against Radford Global Technology Survey and Pave private-market data). Flag specific numbers with `<!-- needs-research -->`.
2. **Target bonus** — percent-of-base, OTE (base + target bonus), and the plan mechanics (MBO vs. corporate-scorecard vs. hybrid). Justify the mix for a pre-IPO CFO vs. a public-company CFO.
3. **Equity grant** — the headline grant (treated in detail in Part B).
4. **PSU / MBO performance overlay** — whether to layer a performance-stock-unit or MBO-gated tranche on top of the time-based equity grant at Series-C. Chapter 04 flags this as optional pre-IPO; justify include-or-not for Larksend specifically given the ~2-year S-1 horizon. If you include a PSU overlay, specify the metrics (revenue, gross-margin, free-cash-flow, non-GAAP operating income — pick the ones that will survive S-1 disclosure) and the performance period.
5. **Severance** — the headline tier (treated in detail in Part C).
6. **CoC acceleration** — the headline terms (treated in detail in Part D).
7. **Benchmark-source table** — a short table showing, for each cash-and-equity line, which benchmark source (Compensia peer-set, Radford, Pave, prior-package data from the two finalists) the proposed number is drawn from, with `<!-- needs-research -->` on any specific percentile number.

### Part B — Equity grant sizing

Produce the equity-grant proposal. Cover:

1. **Percent-of-fully-diluted at hire** — the specific percent-of-fully-diluted the committee is being asked to approve, with the Compensia peer-set band flagged `<!-- needs-research -->`. State the number of shares that implies against Larksend's post-Series-C cap table.
2. **Vesting schedule** — 4-year monthly vesting with a 1-year cliff is the default. Discuss two variants (5-year vesting; back-weighted / "performance-oriented" vesting) and recommend one with justification. Note the interaction with the planned S-1 timeline.
3. **ISO / NSO / RSU allocation** — the specific allocation across instrument types. Reference chapter 02 for the US / country logic (ISO $100k-per-year limit, NSO default beyond that, RSU as a public-company instrument). Larksend is pre-IPO today so RSUs are generally not the right instrument yet; state the switch-over plan at S-1.
4. **Early-exercise / 83(b)** — whether the plan permits early exercise for the CFO and the mechanics the CFO would use (full-exercise-and-83(b)-election at grant vs. exercise-as-vested). Flag the AMT exposure for a large ISO exercise with `<!-- needs-research -->` on current-year AMT thresholds.
5. **Grant-dating policy** — the specific comp-committee practice (grant on the first trading day of the month after hire, or at the next-regular comp-committee meeting, or on offer-letter signature date) and the 409A-valuation that the strike price will be set against.

### Part C — Severance tier

Produce the severance proposal for the CFO. Cover:

1. **Base severance** — 12 months of base is the defensible C-suite starting point for a non-CEO officer. State the specific proposal.
2. **Target-bonus severance** — whether the severance includes 12 months of target bonus (pro-rated or full), and the trigger-event scope (termination without Cause; resignation for Good Reason).
3. **COBRA / health-continuation** — 12 months of employer-paid COBRA is the C-suite starting point. Note the ACA § 4980D and ADEA cross-checks.
4. **Equity treatment on severance (non-CoC termination)** — whether any unvested equity vests on severance in a non-CoC termination (the usual answer is no; the exception is for post-IPO CEOs or for very senior finance hires with large unvested cliffs — justify your choice).
5. **CEO exception** — note that chapter 04's CEO tier is typically 18 months rather than 12 and briefly state why you are not applying the CEO exception to the CFO.
6. **"Good Reason" definition** — the specific triggers (material diminution of duties, material reduction in base or OTE, relocation outside a defined radius, material breach of the agreement by the corporation) and the notice-and-cure mechanics the corporation will insist on.

### Part D — Change-of-control acceleration terms

Produce the CoC acceleration proposal. Cover:

1. **Double-trigger acceleration** — 100% acceleration of unvested equity on a qualifying termination within 12 months (or 24 months — pick one and justify) after a change-of-control. This is market-standard; state the specific proposal.
2. **Single-trigger exception** — whether any portion of the grant vests on CoC alone (not on termination). Chapter 04's default is no single-trigger; discuss where corporations have made exceptions (e.g., for a specific tranche tied to an acquired-corporation retention commitment) and recommend against or for.
3. **"Qualifying termination" definition** — the specific scope (without Cause; for Good Reason; death; disability) with cross-reference to Part C's Good Reason definition.
4. **ISS / Glass Lewis alignment** — note the specific ISS and Glass Lewis policies that double-trigger acceleration satisfies, and the specific ones that single-trigger acceleration would fail. Flag `<!-- needs-research -->` for current-year ISS / Glass Lewis policy language.
5. **CoC definition** — whether CoC is defined as a change in beneficial ownership (>50%), a change in board majority, a sale of substantially all assets, or a merger / consolidation. The specific definition matters for § 280G (Part E) and for whether a growth-equity recap would trigger acceleration.

### Part E — IRC § 280G exposure analysis

Produce the § 280G analysis for the proposed CFO package at a hypothetical change-of-control. Cover:

1. **Parachute-payment stack** — identify the specific payments that would be aggregated as "parachute payments" at CoC (cash severance, bonus severance, equity acceleration value, health-continuation value, any gross-ups).
2. **Base-amount calculation** — the mechanics of the five-year-average W-2 base amount and the "3× base amount" safe-harbor threshold. Note that for a CFO hired at Series-C, the five-year-W-2 history may not yet exist at the corporation — state how the base amount is computed in that case (annualized partial-year compensation).
3. **Excess-parachute determination** — whether the proposed package, at a plausible CoC valuation range, would stack a parachute payment exceeding 3× base amount and therefore trigger the 20% excise tax on the executive and the loss of the corporate deduction on the excess.
4. **Modified-economic-cutback vs. 280G cleanse** — propose one of the two defensible approaches: (a) a modified-economic-cutback (also called "best-after-tax") provision in the exec severance agreement that cuts the package back to just below the safe-harbor if that leaves the executive better off net-of-tax than paying the excise, or (b) a 280G shareholder-cleanse plan under § 280G(b)(5)(A)(ii) that uses the private-company 75%-shareholder-approval exception to disapply the parachute rules. Note the specific procedural requirements of each (cutback is a drafting item; cleanse requires 75% of voting shares entitled to vote, excluding shares held by the disqualified individuals, approving the specific parachute payments after full disclosure).
5. **Recommendation** — pick one approach (or a layered approach — cleanse as the primary path with cutback as a drafting fallback) and justify it for Larksend's cap-table concentration. Flag the specific percent-of-shares-controlled-by-the-top-N-holders as `<!-- needs-research -->`.
6. **§ 162(m) note** — note that § 162(m)'s $1M public-company deduction cap does not apply to Larksend today (private-company) but will apply at and after S-1; briefly state the implication for the base + bonus structure at IPO.
7. **§ 409A note** — note the specific drafting items that keep the severance and equity-acceleration provisions outside § 409A's deferred-compensation rules (short-term deferral exception; separation-pay exception; the six-month-delay rule for specified employees of public companies).

### Part F — Documents checklist

Produce a checklist of the full document set the comp committee will need to approve and the General Counsel will need to execute at CFO start. For each document, name the owner, the counterparty, and the specific cross-references. Cover:

1. **Offer letter** — the headline terms (base, target bonus, equity grant, start date, reporting line, at-will employment, confidentiality / IP-assignment cross-reference).
2. **Executive severance agreement** — the Part C and Part D terms in a standalone agreement (not inside the offer letter).
3. **Change-of-control addendum** — either the Part D terms in a standalone addendum or incorporated by reference into the severance agreement. State the specific choice.
4. **Indemnification agreement** — the officer-indemnification agreement (D&O policy cross-reference, advancement-of-expenses terms, cooperation-and-notice obligations). Cross-reference the officer-appointment side at `../mod-111-corporate-governance-board-operations-and-officer-duties/`.
5. **Stock-option / RSU agreement** — the equity-plan-level grant document, with Part B's early-exercise and acceleration terms wired in.
6. **PIIA / confidentiality / IP-assignment** — the standard IC agreement with the executive-specific additions (non-solicit scope, cooperation after departure).
7. **Board / comp-committee resolutions** — the specific resolutions the comp committee will adopt (approving the package; recommending to the full board); the specific resolutions the full board will adopt (approving the officer appointment under the bylaws; approving the equity grant under the equity-incentive plan; approving the indemnification agreement). Cross-reference `../mod-111-corporate-governance-board-operations-and-officer-duties/` for the officer-appointment resolution.
8. **S-1 forward-reference** — the SEC Reg S-K Item 402 disclosure items that this package will land in at S-1 (Summary Compensation Table, Grants of Plan-Based Awards, Outstanding Equity Awards, Potential Payments on Termination or CoC, CD&A narrative). Cross-reference `../09-sec-reg-sk-item-402-disclosure.md`.

## Starter guidance

- Chapter 04 is the primary reference. Chapters 02 (IC equity plan structure), 07 (CoC equity policy), 08 (executive severance and release), and 09 (SEC Reg S-K Item 402 disclosure) are the structural cross-references. Chapter 05 (comp-committee charter) is the governance cross-reference.
- Do not manufacture market numbers. Where you cite a Compensia / Radford / Pave percentile, a severance multiple benchmark, or a CoC acceleration prevalence number, flag it as `<!-- needs-research -->` for refresh with current data pulled under the Compensia engagement.
- The two finalists have different prior-package backdrops (public-CAO vs. private-CFO). Your package should be defensible against either finalist's walk-away leverage, not pre-fitted to one of them. The committee can then negotiate within the authorized band.
- The § 280G analysis in Part E is where most first-time authors understate the problem. Run the arithmetic even in rough form against a plausible CoC valuation; a growth-equity recap at a modest premium can still stack a parachute. The cleanse-vs-cutback choice has real cap-table consequences.
- The checklist in Part F is not boilerplate. The specific choice to put CoC terms in a standalone addendum vs. inside the severance agreement, or to put equity-acceleration terms in the grant agreement vs. the severance agreement, changes what the comp committee is approving and what the compensation disclosure at S-1 will look like.
- The chapter's default severance tier (12 months base + target bonus + 12 months COBRA + double-trigger CoC acceleration) is defensible for the CFO. The CEO-exception (18 months) is a separate conversation and is out of scope for this exercise.

## Deliverables

- `cfo-package-architecture.md` — Part A.
- `cfo-equity-grant-proposal.md` — Part B.
- `cfo-severance-tier.md` — Part C.
- `cfo-coc-acceleration-terms.md` — Part D.
- `cfo-280g-exposure-analysis.md` — Part E.
- `cfo-documents-checklist.md` — Part F.
- `comp-committee-memo-cfo-package.md` — a 2–3 page memo distilling Parts A–F for the comp committee's approval meeting, with the specific resolutions the committee is being asked to adopt.

## Acceptance criteria

The package is acceptable if:

1. Part A's architecture names a specific base, target bonus, OTE, equity grant percent-of-fully-diluted, and a defensible include-or-not decision on the PSU / MBO overlay with the metrics named if included.
2. Part B's equity proposal names a specific percent-of-fully-diluted at hire, a specific vesting schedule (default or justified variant), a specific ISO / NSO allocation with ISO $100k-per-year arithmetic shown, an early-exercise policy, and a grant-dating policy.
3. Part C's severance proposal names a specific tier (base months, bonus treatment, COBRA months, equity treatment on non-CoC severance) with a specific Good Reason definition and notice-and-cure mechanics.
4. Part D's CoC acceleration proposal names a specific double-trigger structure (acceleration percent, qualifying-termination window post-CoC), a specific stance on single-trigger exceptions, a specific CoC definition, and an ISS / Glass Lewis alignment note.
5. Part E's § 280G analysis identifies the parachute-payment stack, runs the base-amount calculation (with the annualized-partial-year adjustment for a newly-hired executive), determines whether the package stacks an excess parachute at a plausible CoC range, and picks a specific approach (modified-economic-cutback, 280G cleanse, or layered) with justification.
6. Part E also includes the § 162(m) forward-reference note and the § 409A compliance drafting notes.
7. Part F's checklist names at least seven distinct documents, each with owner, counterparty, and specific cross-reference, including the forward-reference to SEC Reg S-K Item 402 disclosure at S-1 and the cross-reference to officer appointment at `../mod-111-corporate-governance-board-operations-and-officer-duties/`.
8. Every market number cited (Compensia / Radford / Pave percentile, severance prevalence, CoC acceleration prevalence, AMT threshold, ISS / Glass Lewis policy language) is either taken directly from chapter 04's ranges or flagged with a `<!-- needs-research -->` marker.
9. The comp-committee memo names the specific resolutions the committee is being asked to adopt and the specific onward resolutions the full board will adopt.
10. Nothing left as `[TBD]` or `[FILL IN]`.
