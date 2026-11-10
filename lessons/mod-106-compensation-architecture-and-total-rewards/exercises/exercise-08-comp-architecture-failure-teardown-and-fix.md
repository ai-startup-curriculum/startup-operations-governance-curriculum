# Exercise 08 — Comp architecture failure teardown and fix

> Estimated time: **~5 hours** · Related chapter: [08 — Comp-architecture failure modes and their fixes](../08-comp-architecture-failure-modes.md)

## Problem statement

Oxbow Labs, Inc. is a Delaware C-corp selling an infrastructure-automation platform to mid-market cloud-native engineering orgs. The corporation is five-and-a-half years old, closed a $92M Series-C fourteen months ago at a $410M post-money, and has grown to **325 employees** across a US-centric footprint with a small UK bridgehead (12 employees). A Series-D round is being contemplated 12–18 months out.

Current state of the comp architecture — the inherited mess:

- **A job architecture was authored at Series-A** (four years ago) by the founding Head of People. It was lightly ratified by the founder-CEO, never ratified by a comp committee (the committee was not constituted until Series-B), and has been revised in place three times — twice by subsequent Heads of People and once by a tenured engineering manager who promoted themselves into the Head-of-Engineering role. The current version on the wiki is not clearly versioned; three team leaders are each operating against a different snapshot.
- **The engineering ladder has drifted.** A cross-function headcount pull three weeks ago showed that **47% of the engineering IC population is at Staff or above** (E5–E7), against a market cut that is typically 15–25% for a Series-C tech corporation (`<!-- needs-research -->` on the specific market cut). The CPO and the new Head of Total Rewards both believe the ladder has suffered promotion inflation.
- **The IC-ladder is compressed at the top.** The highest engineering IC level the corporation uses is E6 ("Principal Engineer"). No E7 exists. Three Principal Engineers in the last 18 months have left with exit interviews that cited "no path forward on the IC track" as a contributing reason.
- **Cross-function inversion is live.** A current Enterprise AE's actual total cash (base + commissions at ~180% quota attainment) sits 23% above the total cash of an E5 Staff Engineer on the same team. The Enterprise AE's written OTE sits 8% above the Staff Engineer's total cash; the actual attainment-driven overage is 15% on top of that. The E5 Staff Engineer, who sees the comparison clearly because the two sit on the same cross-functional team, has raised the issue to their manager twice.
- **Geographic-arbitrage drift is visible.** Three engineers hired against the Bay-Area band have since relocated to tier-3 markets (Nashville, Boise, Omaha) without a band reset. Two of the three have raised the band-reset-on-relocation question internally; the Head of People at the time (now departed) told them verbally that the "band follows the hire, not the location."
- **Tenure-vs-performance drift is diagnosed.** The annual comp-cycle run by the previous Head of People awarded a merit pool roughly proportional to tenure, with little differentiation by performance rating. The top-performer merit vs. median-performer merit differential at the last cycle was ~1.6× (top 15% of performers getting 6.5% merit; median getting 4%; bottom 10% getting 3%). A chapter-04 and chapter-08 cut would recommend a 2.5–3× differential at Series-C to retain top performers; `<!-- needs-research -->` for specific peer-cut cuts.
- **Promotion inflation is live.** The promotion rate at the last two annual cycles was 18% and 22% of the eligible population. A chapter-04 / chapter-08 cut recommends 8–12% at Series-C for a mature architecture; `<!-- needs-research -->` for specific peer-cut distributions.
- **Pay-equity audit output from eight months ago** is sitting unaddressed. The audit (run under attorney-client privilege by the GC's chosen outside counsel using Syndio or a similar tool) identified a **statistically significant 4.3% pay gap between female and male engineering ICs** at the E3 and E4 levels after controlling for tenure, geography, level, and performance rating. The audit's remediation recommendation (a one-time true-up at the next cycle, with the cost absorbed in the market-adjustment sub-pool) has not been implemented.
- **The Series-D process is a forcing function.** The expected lead investor's operating partner will diligence the comp architecture; the known-unaddressed items (ladder drift, inversion, promotion inflation, pay-equity audit) are likely to surface as Severity-1 or Severity-2 findings if not remediated in advance.

Your role: you are the **newly-hired Head of Total Rewards** (first 90 days in seat), reporting into the CPO (newly-hired Head of People, also in first 90 days) and dotted-line to the comp-committee chair. Produce the failure-mode teardown, the prioritized remediation plan, the specific per-mode fixes, the cycle-integration plan, the comp-committee presentation memo, and the all-hands communication plan.

## Requirements

### Part A — Failure-mode teardown

Produce the failure-mode teardown against chapter 08's five-mode library. Cover, for each of **level compression, tenure-vs-performance drift, cross-function inversion, promotion inflation, and geographic-arbitrage drift**:

1. **The mode's definition.** State the chapter-08 definition in one or two sentences.
2. **The specific evidence at Oxbow.** Name the specific data point(s) from the problem statement that diagnose the mode. For modes diagnosed against market cuts (promotion rate, Staff-and-above proportion, tenure-vs-performance differential), name the current Oxbow number, the target chapter-cut, and the source for the chapter-cut (flagged `<!-- needs-research -->`).
3. **The root cause.** State the root cause — which operating decision (hiring-manager-driven promotion, merit-pool-proportional-to-tenure, band-follows-the-hire geo policy, no E7 authored, no comp-committee ratified band file) created the mode. Chapter 08 names the leading indicator for each mode.
4. **The compound effect.** State the compound effect on the other failure modes — e.g., promotion inflation drives level compression; level compression drives inversion with the senior IC ladder; inversion drives attrition at the top of the IC ladder; attrition at the top of the IC ladder makes promotion-inflation worse at the bottom as the architecture tries to retain through promotion. Diagnose the compound effect at Oxbow.
5. **The Series-D-diligence severity.** State the expected Severity rating (1, 2, or 3) the operating partner will apply to each mode if it remains unremediated at diligence, with rationale.

### Part B — Prioritised remediation plan

Produce the prioritised remediation plan. Cover:

1. **The ranking.** Rank the five failure modes by remediation priority. Chapter 08 notes the typical priority (pay-equity audit first because the legal exposure is immediate; cross-function inversion second because the attrition risk is immediate; level compression third because the ladder change is structural; geographic-arbitrage drift fourth because the per-hire adjustment is bounded; promotion inflation fifth because the remediation is cyclical and multi-year). State Oxbow's ranking with rationale.
2. **The sequencing against the annual cycle.** The next annual comp cycle is Q1 2026. State which remediations are sequenced *inside* the Q1 2026 cycle (the fast-remediation list), which are sequenced *outside* the cycle (the slow-remediation list — architecture changes that land at the cycle after but are briefed to the organisation now), and which are *structural* (the architecture work that is in progress at Series-D diligence but not expected to be complete).
3. **The budget impact.** State the budget impact of each remediation on the Q1 2026 cycle — the pay-equity true-up cost, the inversion-correction cost (base-adjustment to the E5 Staff Engineer or equivalent remediations across the architecture), the Staff-level re-leveling cost (if some ICs are moved from E5 to E4 at the next cycle, the implication for their comp is a flat-not-reduced merit at the next cycle, which is manageable — but telling 10 ICs they are being re-leveled is a non-financial cost). Flag `<!-- needs-research -->` for current-cut market data on the true-up cost magnitudes.
4. **The communication-sequencing risk.** The remediation plan will be visible to the organisation. State the communication-sequencing risk — a leak about the re-leveling exercise before the comp-committee ratification would create a retention crisis. State the all-hands communication plan (Part F) and the specific gates (comp committee ratifies before anything is communicated; the CPO and the Head of Total Rewards communicate before any manager; every re-leveling conversation is 1:1 with the manager and the HRBP present).

### Part C — Per-mode fixes

Produce the specific fix for each of the five failure modes. Cover:

1. **Level compression and promotion-inflation fix.**
    - **The ladder audit.** A full audit of the current E4, E5, E6 population against the ratified rubric (the updated rubric is a Part D deliverable). For each IC flagged as "over-leveled" at hire or at promotion, the disposition — re-level down, re-level only at the next promotion opportunity (the "downward natural progression" approach), or accept the over-level with documentation and no further promotion at the next cycle.
    - **The E7 standup.** Author the E7 "Distinguished / Fellow" level definition against the chapter-01 rubric. State the first E7 internal candidate(s) (if any) and the ratification path through the leveling council and the comp committee. Cross-reference [chapter 01](../01-job-architecture-and-leveling-framework.md) for the ladder-height rationale and [exercise 01](./exercise-01-job-architecture-and-leveling-framework-authoring.md) for the authoring template.
    - **The promotion-rate target.** State the target promotion rate for the Q1 2026 cycle and the cycles beyond, with the merit-pool reservation for promotion increases and the strict review gate the leveling council will apply.
2. **Tenure-vs-performance drift fix.**
    - **The merit-differential policy.** State the new policy — the top-performer merit vs. median-performer merit differential at the Q1 2026 cycle targets 2.5–3× (top 15% at 7.5%, median at 3%, bottom 10% at 1%), with specific numbers flagged `<!-- needs-research -->` against market cuts.
    - **The communication to managers.** State the manager-training session at cycle kickoff that explains the differential and the expectation.
    - **The HRBP calibration gate.** State the calibration-rubric update ([exercise 04](./exercise-04-annual-comp-cycle-workflow-and-communications.md) Part E) that catches top-performers-receiving-median-merit as a mandatory calibration review item.
3. **Cross-function inversion fix.**
    - **The scan.** Run the scan against the current comp file — every E5 vs. Enterprise AE, every E5 vs. Sales Manager, every E6 vs. Director of Sales, every exec-tier comparison. For each inversion instance (named by level-pair pattern, not individual), state the disposition.
    - **The named Enterprise AE vs. E5 Staff Engineer disposition.** Specifically — is the Enterprise AE's 180% attainment the comp-plan working as designed (the accelerator is paying as intended, the E5's comp is at-band, the inversion is driven by attainment not architecture), or is the architecture itself inverting (the OTE midpoint for Enterprise AE is above the E5 Staff Engineer midpoint, which is a chapter-07 and chapter-02 architectural error)? Cross-reference [chapter 07](../07-sales-comp-plan-design.md) and [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md).
    - **The structural fix.** If the OTE midpoint inverts, the fix is to the chapter-02 band file; if the attainment-driven overage inverts, the fix is to the Staff Engineer's merit or a retention grant from the equity-refresh pool.
4. **Geographic-arbitrage drift fix.**
    - **The three relocated engineers.** For each of the three (Nashville, Boise, Omaha), state the disposition — band-reset at the next cycle with the specific tier applied (loss from Tier 1 to Tier 3/4), band-reset with a one-time transition payment to soften the reset (chapter-08 notes this is market-practice at Series-B+ but is not required), or no reset with a documented exception (which creates a new precedent that has to be honored for future relocations).
    - **The policy rewrite.** State the updated geo-policy: the band follows the *location*, not the *hire*. Relocation to a lower tier triggers a band reset at the next cycle gate; relocation to a higher tier triggers a band reset only if the relocation is corporation-initiated or the IC requests a reset. Cross-reference [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md).
    - **The communication to the three engineers.** The specific communication script — the policy change, the specific band reset at the next cycle, the transition-payment-or-not decision.
5. **Pay-equity audit remediation.**
    - **The true-up.** State the one-time true-up — every female engineering IC at E3 and E4 (or whatever levels were flagged in the audit) receives a base-salary adjustment at the Q1 2026 cycle sized to close the 4.3% gap. The cost is absorbed in the market-adjustment sub-pool of the merit budget.
    - **The attorney-client-privilege wrapper.** State the wrapper — the pay-equity audit output is protected work-product, prepared at the direction of the GC for the purpose of legal advice; the true-up is an operational implementation of the privileged recommendation, implemented through the normal cycle (merit adjustment in the market-adjustment sub-pool) rather than a standalone "pay-equity true-up" line that would be discoverable. Cross-reference [mod-103](../../mod-103-employment-law-and-contract-design/) for the NLRA § 7 backdrop and the privilege treatment.
    - **The forward-looking audit cadence.** State the audit cadence going forward — pre-cycle pay-equity audit at the Q1 cycle and the mid-year cycle (if a mid-year cycle exists), with the Compensia-or-Syndio-or-equivalent tool and the outside-counsel privilege wrapper.

### Part D — Cycle-integration plan

Produce the cycle-integration plan — how the remediations land inside the Q1 2026 annual comp cycle. Cover:

1. **The cycle calendar amendments.** Cross-reference the [exercise 04](./exercise-04-annual-comp-cycle-workflow-and-communications.md) cycle calendar and amend it to include:
    - The ladder-audit gate (pre-cycle; the leveling council reviews the current E4–E6 population and approves the re-level list before the cycle kicks off).
    - The pay-equity audit gate (pre-cycle; the GC's audit output is reviewed by the CPO and the Head of Total Rewards; the true-up is sized against the market-adjustment sub-pool).
    - The cross-function inversion-scan gate (pre-cycle; the Head of Total Rewards scans the current comp file and dispositions each inversion instance).
    - The geographic-arbitrage-drift gate (pre-cycle; the three relocated engineers are dispositioned).
    - The re-leveling-communication gate (mid-cycle; after comp-committee ratification and before cycle-close).
2. **The cycle budget amendments.** Cross-reference the [exercise 04](./exercise-04-annual-comp-cycle-workflow-and-communications.md) cycle budget and amend it to include:
    - The pay-equity true-up cost in the market-adjustment sub-pool.
    - The inversion-correction cost in the retention sub-pool.
    - The staff-level re-leveling savings (if any) applied to the merit pool (the re-leveling is typically cost-neutral because the ICs' comp stays the same but their level changes; the merit-pool impact is on their next-cycle merit, not this cycle).
3. **The comp-committee ratification sequence.** State the specific sequence — the comp committee ratifies the ladder audit before the cycle kicks off, the merit-pool sizing (including the market-adjustment sub-pool with the pay-equity true-up) at cycle kickoff, and the individual exec-comp line items at cycle-close.

### Part E — Comp-committee presentation memo

Produce the **1-page memo** attaching the failure-mode teardown and the remediation plan. Cover:

- The five failure modes, the specific Oxbow evidence, and the ranked remediation priority (Part B).
- The specific remediation dispositions for each mode (Part C) — the ladder audit and E7 standup, the merit-differential policy, the inversion-scan and the Enterprise-AE-vs-Staff-Engineer disposition, the three relocated engineers, and the pay-equity true-up.
- The Q1 2026 cycle integration (Part D) and the budget impact.
- The Series-D diligence tie-back — the specific Severity-1 and Severity-2 findings expected to be remediated before diligence re-engages.
- The all-hands communication plan (Part F) and the specific gates.
- The `<!-- needs-research -->` queue grouped by remediation decision (market cuts on promotion rate, Staff-and-above proportion, tenure-vs-performance differential, pay-equity audit true-up magnitudes).

### Part F — All-hands communication plan

Produce the **short** all-hands communication plan (max 1 page) that the CPO and the founder-CEO will use to communicate the architecture changes to the organisation. Cover:

1. **The high-level message.** Two sentences on the why — the Series-D process, the architecture maturation, the commitment to a sustainable comp system.
2. **The specific audiences.** The exec team (first; already in the loop), the managers (second; one-cycle-ahead briefing), the full organisation (third; cycle-launch all-hands).
3. **The specific topics and the specific audiences.** For each of the five failure-mode remediations, state which audience hears about it and when — e.g., the ladder audit and re-level list are briefed to the affected ICs 1:1 before the cycle, not announced at the all-hands; the merit-differential policy change is briefed to managers at cycle-kickoff; the pay-equity true-up is implemented silently in the market-adjustment sub-pool and *not* communicated as a standalone initiative (to preserve the privilege wrapper).
4. **The never-communicate list.** State what the organisation will *never* hear communicated in those terms — "we found a gender pay gap," "we over-leveled the engineering org," "the Enterprise AE is overpaid relative to the Staff Engineer." State the reason — operational communications in those terms create legal exposure, retention risk, and manager-trust erosion.

## Starter guidance

- Chapter 08 is the primary reference. Re-read the "level compression," "tenure-vs-performance drift," "cross-function inversion," "promotion inflation," "geographic-arbitrage drift," and "pay-equity audit" sections before authoring.
- The teardown is a diagnostic exercise, not a blame exercise. The previous Head of People is departed; the previous CPO is departed. The teardown is backward-looking for root-cause purposes but the remediation is forward-looking.
- **Do not manufacture market numbers.** Every market-cut (promotion rate, Staff-and-above proportion, tenure-vs-performance differential, pay-equity magnitude, merit-differential) must be flagged `<!-- needs-research -->`.
- The pay-equity remediation is the highest-stakes line in the plan. The attorney-client-privilege wrapper is operational — the true-up is implemented through the normal market-adjustment sub-pool, not through a standalone line item. The communication plan (Part F) codifies the "never-communicate" list.
- The Series-D diligence severity ratings in Part A are the operating-partner-facing framing. Treat them as the lens the comp committee will adopt at ratification.
- Cross-reference [exercise 01](./exercise-01-job-architecture-and-leveling-framework-authoring.md) for the ladder-authoring template, [exercise 02](./exercise-02-cash-and-equity-band-authoring-by-geography.md) for the band file and the compression / inversion diagnostic, [exercise 04](./exercise-04-annual-comp-cycle-workflow-and-communications.md) for the cycle integration, and [exercise 07](./exercise-07-sales-comp-plan-design-in-coordination-with-gtm.md) for the cross-function inversion with Enterprise AE.

## Deliverables

- `failure-mode-teardown.md` — Part A.
- `prioritised-remediation-plan.md` — Part B.
- `per-mode-fixes.md` — Part C.
- `cycle-integration-plan.md` — Part D.
- `comp-committee-memo.md` — Part E (1 page).
- `all-hands-communication-plan.md` — Part F (1 page).

## Acceptance criteria

The package is acceptable if:

1. Part A's teardown covers all five failure modes with the chapter-08 definition, the specific Oxbow evidence (with `<!-- needs-research -->` flags on market cuts), the root cause, the compound effect on other modes, and the expected Series-D-diligence severity rating.
2. Part B ranks the five modes by remediation priority with rationale, sequences each against the Q1 2026 cycle (fast / slow / structural), states the budget impact, and identifies the communication-sequencing risk.
3. Part C authors the specific fix for each of the five modes:
    - Level compression + promotion inflation: ladder audit, E7 standup with ratification path, promotion-rate target.
    - Tenure-vs-performance drift: merit-differential policy with specific numbers flagged, manager-training, HRBP calibration gate update.
    - Cross-function inversion: comp-file scan, named Enterprise AE vs. E5 Staff Engineer disposition, structural fix path.
    - Geographic-arbitrage drift: three-engineer disposition, policy rewrite, communication script.
    - Pay-equity audit: true-up implemented through market-adjustment sub-pool, privilege wrapper, forward-looking audit cadence.
4. Part D amends the [exercise 04](./exercise-04-annual-comp-cycle-workflow-and-communications.md) cycle calendar and budget with the specific gates (ladder audit, pay-equity audit, inversion scan, geo-drift disposition, re-leveling communication) and the specific comp-committee ratification sequence.
5. Part E's comp-committee memo is **one page**, names the five failure modes, the specific remediation dispositions, the cycle integration, the Series-D diligence tie-back, the all-hands communication plan gates, and the `<!-- needs-research -->` queue.
6. Part F's all-hands communication plan is **one page**, states the high-level message, the three specific audiences, the topic-by-audience sequencing, and the never-communicate list with rationale.
7. Every market cut (promotion rate, Staff-and-above proportion, tenure-vs-performance differential, merit differential, pay-equity magnitude, true-up cost) is flagged `<!-- needs-research -->`. The attorney-client-privilege wrapper on the pay-equity remediation is explicit.
8. Cross-references to [chapter 01](../01-job-architecture-and-leveling-framework.md), [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md), [chapter 04](../04-annual-comp-cycle.md), [chapter 07](../07-sales-comp-plan-design.md), [exercise 01](./exercise-01-job-architecture-and-leveling-framework-authoring.md), [exercise 02](./exercise-02-cash-and-equity-band-authoring-by-geography.md), [exercise 04](./exercise-04-annual-comp-cycle-workflow-and-communications.md), [exercise 07](./exercise-07-sales-comp-plan-design-in-coordination-with-gtm.md), and [mod-103](../../mod-103-employment-law-and-contract-design/) are present.
9. Nothing left as `[TBD]` or `[FILL IN]`.
