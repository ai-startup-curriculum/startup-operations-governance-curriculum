# 3. Refresh, promotion, and retention grants

> An initial grant retains an employee for about three years. Everything after that is a design choice — and the corporation that treats refresh, promotion, and retention grants as one coherent policy keeps its people; the one that treats them as three ad hoc exceptions does not.

## Motivation

The initial new-hire grant covered in [chapter 02](./02-new-hire-grant-design.md) is a four-year instrument. It is sized against a market band, it vests on the standard 1-year cliff / monthly thereafter, and it is the single largest equity decision the corporation makes about that employee. It is also the single largest equity decision the corporation will *stop* making about that employee if nothing else is designed on top of it.

The problem is mechanical, not emotional. A four-year grant decays monotonically in forward-looking value. At month 12, the employee has 36 months of unvested equity ahead. At month 24, 24. At month 36, 12. At month 48, zero. The retention value of the grant — the amount of "if I leave now I walk away from X" that the employee can see when a recruiter emails them — collapses on a known schedule.

Without a refresh policy that is credible, differentiated, and visible, the corporation gets three predictable outcomes:
- A departure spike in the month-30-to-month-42 window as the forward-vest shrinks below the equivalent of a competing-offer sign-on grant.
- A talent-density problem at month-48, when the strongest performers — who have the most portable options — convert the fully-vested stake into a decision to leave.
- A promotion-grant improvisation problem in which every manager invents a different number for "what the newly-promoted staff engineer should get," because no cross-functional policy exists.

This chapter covers the three post-initial grant instruments — refresh grants, promotion grants, and retention grants — as a single policy surface. The sizing economics tie back to the equity-philosophy and ownership-targets conversation in [chapter 01](./01-equity-philosophy-and-ownership-targets.md); the initial grant mechanics come from [chapter 02](./02-new-hire-grant-design.md); the valuation and 409A inputs are covered in [chapter 04](./04-409a-and-pricing-mechanics.md); the comp-committee approval thresholds and workflow are covered in [chapter 05](./05-compensation-committee.md); the operating cadence that ties the policy into the annual cycle is covered in [chapter 06](./06-annual-comp-cycle.md); and the change-of-control-specific instruments (double-trigger acceleration, retention pool at deal) are covered in [chapter 07](./07-change-of-control-equity-policy.md). The dilution-budget math — how the refresh pool interacts with option-pool refreshes at the next priced round — is covered in the `startup-finance-fundraising-curriculum`.

## Why a grant decays — the "equity cliff at year 3" problem

The decay is arithmetic, but the behavioural effect is what matters.

### The forward-vest curve

A standard 4-year grant with a 1-year cliff produces the following "forward-looking unvested value" curve, measured in months of unvested vest remaining:

- Month 0 — 48 months unvested.
- Month 12 (cliff) — 36 months unvested; the first 25% has just hit.
- Month 24 — 24 months unvested.
- Month 30 — 18 months unvested.
- Month 36 — 12 months unvested.
- Month 42 — 6 months unvested.
- Month 48 — 0 months unvested.

The retention economics inflect somewhere between month 30 and month 42. Below roughly 12-18 months of forward-looking vest, a credible competing offer with a standard 4-year grant and a signing bonus can match or beat the forward-vest value of staying. The employee is now "equity-neutral" or "equity-positive" on leaving. If the corporation has not acted before this window, the departure decision is a rational one for the employee.

### Why this is not solved by salary

A base-salary increase does not refill the forward-vest. It raises the opportunity cost of a competing offer by a modest margin — a 10% raise against a market-matching offer is a tie-breaker, not a decision-mover — but it does not restore the "walk-away cost" that an unvested equity stake creates. The corporation needs to replenish the equity itself; cash is a different lever.

### Why this is not solved by the one-time year-4 cliff refresh

The naive policy is "we give everyone a refresh at their 4-year anniversary." This is simple to administer and fails for a specific reason: the window is highly visible, so departures cluster *before* the refresh — in the month-30-to-month-42 range — because employees who are already receiving outside interest cannot afford to wait a year for the policy to catch up. The policy becomes a tax on loyalty and a bonus to the departing.

## Refresh cadence options

The corporation picks a cadence for how refresh grants are made. Three canonical options:

### Annual top-up

A refresh grant is awarded every year — typically at the annual comp cycle (see [chapter 06](./06-annual-comp-cycle.md)) — sized to restore each tenured employee to a target *forward-looking vest* of some length (commonly 2-4 years). The refresh is new, standalone, with its own 4-year vest (see "Vesting start on refresh" below).

**Why this works.** The curve stays smooth. There is no visible "cliff year" at which an employee decides whether to stay or leave. Managers calibrate once a year as part of a normal cycle. The programme is legible to recruiters trying to counter-pitch — "every year we refresh" is a crisp sentence.

**When to use it.** This is the modal choice at Series-B and beyond and the recommended default for any corporation with more than ~50 employees.

### Milestone-based

Grants are tied to specific operating or product milestones — shipping a product, hitting a revenue threshold, closing a specific customer, completing a promotion. There is no fixed calendar.

**Why this is used.** At pre-Series-B, when the corporation is milestone-driven and the headcount is small enough that each grant is a bespoke conversation, milestone-based refreshes are legible and motivating. They also match the operating cadence of a small company that is not yet running an annual comp cycle.

**Why it does not scale.** At scale, milestone-based grants produce three failure modes: (a) employees on non-shipping functions (G&A, support, internal tooling) feel systematically underweighted; (b) the corporation ends up negotiating individually with the strongest performers every time a milestone hits; (c) comp-committee reporting becomes impossible to produce because the grants are not on a cadence.

### Cliff-based (year-3 or year-4 refresh)

A single refresh is granted at the end of the forward-vest window — month 36 or month 48 — and the corporation does not grant anything in between.

**Why this is used.** Simpler to administer. Lower refresh pool spend, because grants happen less frequently.

**Why it is the worst choice at scale.** The cliff is visible to the employee and to competing recruiters. The pre-cliff attrition window is a known quantity. The corporation ends up paying the retention cost in attrition rather than in refresh dilution, and attrition is a strictly worse use of the budget.

**Pick annual as the modal choice for Series-B and beyond.** The remainder of this chapter assumes an annual refresh cycle unless noted.

## Refresh grant sizing

Two sizing conventions exist, and they coexist at most Series-B and later corporations.

### Percent-of-initial-grant

The refresh is sized as a percentage of the employee's *original* initial grant. Commonly cited ranges are 25-50% of the initial grant for strong performers, scaled down for middle-quartile performers and down further or to zero for bottom-quartile. <!-- needs-research: confirm current-market refresh-as-percent-of-initial-grant benchmarks across quartiles; Carta refresh benchmarks and Pave compensation data are the usual primary sources. -->

**Advantages.** Easy to compute. Preserves the relative ordering of the initial grants, so an employee who was hired at a senior level continues to earn larger refresh grants than one hired at a junior level. Works even when the corporation does not yet have a mature levelling architecture.

**Disadvantages.** Decouples the refresh from the current-market comp band. An employee hired three years ago when the band was lower will receive a smaller refresh than a lateral hire at the same level today — a visible inequity that creates a "stay vs. interview externally" incentive.

### Dollar-value refresh at current 409A

The refresh is sized as a dollar amount — tied to the employee's level and performance quartile — and converted to a share count using the current 409A valuation (see [chapter 04](./04-409a-and-pricing-mechanics.md)). This is the standard structure once RSUs are in the mix, which typically happens at Series-B or later as the fair value of the common grows into a range where options stop being tax-efficient.

**Advantages.** The refresh is calibrated to the *current* market. Employees are brought up to a target forward-vest in dollar terms, not share-count terms. Benchmarking against external data (Carta Total Comp, Pave, Option Impact / Advanced-HR) is direct. <!-- needs-research: confirm the current primary benchmarking providers for refresh grant dollar values at Series-B through pre-IPO; Carta, Pave, Option Impact (Advanced-HR), Radford, and Compa are the commonly cited providers. -->

**Disadvantages.** Requires an up-to-date 409A, requires a levelling architecture that maps every employee to a target total-equity band, and requires the corporation to make a defensible choice about which market percentile to target.

### How to choose

A reasonable staged choice: percent-of-initial through Series-A; dollar-value refresh at current 409A starting at Series-B when the levelling architecture and benchmarking subscriptions are in place. The transition itself is a comp-committee decision (see [chapter 05](./05-compensation-committee.md)) because it changes the refresh-pool budget-sizing method.

## Promotion grants

A promotion grant is a one-time, event-driven top-up triggered when an employee is promoted to a new level.

### Sizing — the delta method

The standard sizing is the *delta* between the employee's current-level target total-equity band and the new-level target total-equity band, measured in current-409A dollars and converted to a share count. The employee is effectively being brought up from "mid-band at level N" to "mid-band at level N+1" in equity terms.

A corporation with a clean levelling architecture can state the policy as: "A promotion from L4 to L5 carries an equity delta of X dollars at the current 409A, vesting over 4 years from the promotion effective date." Everyone receives the same delta for the same transition; manager-by-manager improvisation disappears.

### Interaction with the annual refresh cycle

A standard failure mode: an employee is promoted in Q2 and also receives a Q4 annual refresh, double-counting the "levelled up" adjustment. Two policy choices resolve this:

- **Blended policy.** The promotion grant is sized to bring the employee to the new-level target *including* the forward-vest already in flight. The annual refresh in the same year is sized against the new level. No double-counting.
- **Reset policy.** The promotion grant is sized against the full new-level initial-grant band and the employee's prior equity is left in place. The annual refresh cycle resumes on the normal cadence the following year, with the promotion grant counted against the forward-vest.

The blended policy is the market norm at Series-B and beyond. Document which policy the corporation uses so the comp committee is not approving the same economics twice. See [chapter 06](./06-annual-comp-cycle.md) for the operating workflow.

## Retention grants

A retention grant is an exceptional grant made *outside* the refresh and promotion cadences. It is the discretionary instrument, and it is the one most frequently abused.

### The three legitimate triggers

- **A credible competing offer.** The employee has an at-hand offer from a comparable corporation with a verifiable grant. The retention grant is sized to make the stay-decision clearly economically preferred, usually with a 1-2 year focus on forward-vest.
- **Mission-critical status for an upcoming event.** A specific employee is critical to a change-of-control window (see [chapter 07](./07-change-of-control-equity-policy.md)), a product launch, or a pre-IPO stabilisation period. The grant is designed around the event's time horizon — often with cliff-vesting at the event date — to keep the employee in seat through the window.
- **One-time retention risk.** A role-specific or life-event-specific retention concern (a key engineer whose team has been reorganised; a critical salesperson whose territory was changed). Narrower in scope and smaller in size than the first two triggers.

### What is not a legitimate trigger

- "They are a strong performer and we want to show them we care." This is what the annual refresh is for.
- "The manager promised them something." This is a management-training issue, not an equity-policy issue.
- "The CEO decided to award it in a 1:1." Comp committees reject founder-discretionary retention grants above threshold for a reason; see [chapter 05](./05-compensation-committee.md).

### Approval mechanics

Market practice at Series-B and beyond requires comp-committee approval for IC retention grants above a dollar or share-count threshold, with CEO and CFO sign-off below that threshold. The specific thresholds and the pre-read package the committee expects are covered in [chapter 05](./05-compensation-committee.md).

## Refresh budget

The refresh budget is the dilution the corporation is willing to incur per year to fund refresh, promotion, and retention grants in aggregate.

### Two sizing conventions

- **Percent of outstanding fully-diluted shares.** Commonly cited ranges are 1-3% of fully-diluted outstanding per year at scale, with the lower end of the band appropriate at Series-B and the higher end common at pre-IPO when retention risk is highest. <!-- needs-research: confirm current-market refresh-pool-as-percent-of-fully-diluted benchmarks across Series-B, Series-C, growth, and pre-IPO stages. -->
- **Percent of initial grants.** The refresh pool is sized as a percent (commonly 25-50%) of the initial grants being made that year, scaled by headcount of tenured employees eligible for refresh. Simpler to compute; less tightly bound to total dilution.

The two conventions should produce roughly consistent numbers. If they diverge materially, the levelling architecture or the headcount plan is drifting from the equity philosophy — a signal to re-open the discussion from [chapter 01](./01-equity-philosophy-and-ownership-targets.md).

### Interaction with the option pool

Refresh dilution comes out of the available option pool. If the corporation is already running the pool low heading into the next priced round, refresh grants compete with new-hire grants for the same shares. The dilution-budget math and option-pool-top-up negotiation at the priced round are covered in the `startup-finance-fundraising-curriculum`.

## Grant distribution philosophy

Within the refresh budget, how is the pool distributed across employees?

### Differentiated distribution

The strong performers receive materially larger refreshes than the middle and lower performers. A commonly used shape — a "50-30-20" or similar skew — allocates roughly half of the refresh pool to the top quartile, roughly a third to the middle 50%, and the balance (sometimes zero) to the bottom quartile. <!-- needs-research: confirm current-market quartile-weighted refresh distributions; Pave and Carta publish ranges but the specific split varies by stage and sector. -->

**Why this works.** The highest-leverage retention spend is on the strongest performers. Differentiated distribution signals to the organisation that performance matters in equity, not just in cash bonus.

**Why it is hard.** It requires a trustworthy performance-rating process, a manager-calibration cadence, and an HRBP review workflow. The full annual-comp-cycle workflow is covered in [chapter 06](./06-annual-comp-cycle.md).

### Flat distribution

Every employee at a given level receives the same refresh. Simpler to administer. Appropriate when the corporation does not yet have a performance-management system that can defensibly produce quartile ratings.

**Why it degrades over time.** Flat distribution systematically underpays the top-quartile and systematically overpays the bottom-quartile. The top-quartile departure rate rises; the bottom-quartile departure rate falls. Over 2-3 refresh cycles, the talent density of the corporation decays.

Most corporations graduate from flat to differentiated at the same time they stand up a formal performance-rating cycle — typically Series-B.

## Vesting start on refresh

A refresh grant can either (a) carry its own new 4-year vest from the grant date, or (b) be "tacked on" to the end of the current vest schedule.

**Market standard — new 4-year vest from grant date.** The refresh is a standalone grant with its own 1-year cliff (or no cliff, depending on policy) and its own 4-year vest. The employee's "forward-looking vest" picture becomes a layered stack of overlapping grants, each with its own schedule.

**Tacked-on vest.** The refresh starts vesting only when the current grant is fully vested. Rare in standard refresh practice; appears in specific negotiations — most commonly in retention grants where the corporation is specifically trying to buy forward-vest coverage during a known-exit window and does not want to pay for vest that overlaps with the already-vesting initial grant.

Use the market-standard new-vest-from-grant-date as the default. Document the exception policy — when tacking is permitted and who approves it — rather than leaving it to case-by-case negotiation.

## A worked example

A Series-B enterprise-software corporation ("Fictional-Corp") has 180 employees, has just closed its Series-C term sheet (not yet signed), and is designing its first formalised refresh cycle. The CEO, CFO, and Head of People bring the policy to the comp committee for approval.

**Policy parameters.**

- **Cadence.** Annual, aligned with the fiscal-year end. First cycle Q1 of the next fiscal year.
- **Target forward-looking vest.** Two years at the annual anchor date for all tenured employees (hired more than 12 months before the anchor).
- **Refresh pool.** 2% of fully-diluted outstanding, approximately <!-- needs-research: Fictional-Corp's post-Series-C fully-diluted share count would determine the absolute number; the policy is expressed as a percent so the committee approves the percent and the absolute number is computed at close. --> shares.
- **Sizing method.** Dollar-value refresh at current 409A for L4 and above; percent-of-initial-grant for L1-L3 pending the levelling-architecture rollout later in the year.
- **Distribution.** Differentiated — 50% of the pool to the top quartile, 35% to the middle 50%, 15% to the bottom quartile, zero to anyone on a performance-improvement plan.
- **Vesting.** New 4-year vest from grant date, no cliff on refresh grants (initial grants retain the 1-year cliff).

**A promotion-grant bolt-on.** A senior engineer is promoted from L4 to L5 effective Q2. The L4-to-L5 equity delta per the levelling architecture is <!-- needs-research: Fictional-Corp's levelling architecture would specify the dollar delta; a defensible Series-B / C range for an L4-to-L5 engineering promotion equity delta is in the low-hundreds-of-thousands of dollars at current 409A but should be sourced to Pave / Carta / Option Impact benchmarks. --> dollars at current 409A, converted to shares at the then-current 409A price. The grant vests on a new 4-year schedule from the promotion effective date. Under the blended policy, the engineer's Q4 annual refresh is sized against the L5 target, with the Q2 promotion grant counted against the forward-vest.

**A retention-grant bolt-on.** A principal product manager is identified as mission-critical for the pre-IPO 18-month window (the corporation is targeting IPO readiness per the policy framework in [chapter 07](./07-change-of-control-equity-policy.md)). The CEO proposes a retention grant above the comp-committee threshold. The pre-read package to the committee (see [chapter 05](./05-compensation-committee.md)) includes: the employee's forward-vest curve showing the inflection in month 32; a benchmarking comparison from Pave / Carta Total Comp; the vesting schedule (24-month cliff at the targeted IPO window with 12-month tail); and the share-count impact against the refresh-pool budget. The committee approves.

**What the committee approves.** The committee approves the policy *parameters* for the annual cycle (cadence, target forward-vest, refresh-pool percent, sizing method, distribution shape, vesting defaults), the promotion-grant policy with the delta amounts per level transition, and the retention-grant threshold and workflow. Individual grants below the threshold are approved by CEO and CFO; grants above the threshold come back to the committee case-by-case.

## Summary

- A four-year initial grant decays monotonically in forward-looking value. Without a refresh, the retention cliff lands in the month-30-to-month-42 window and departures spike. Pick a refresh cadence that is credible, differentiated, and visible to the organisation.
- Annual refresh is the modal choice for Series-B and beyond; milestone-based works pre-Series-B; cliff-based (year-3 / year-4 only) is the worst choice at scale because the window is visible to recruiters and employees.
- Size refreshes as percent-of-initial-grant through Series-A and as dollar-value-at-current-409A starting at Series-B; distribute the refresh pool differentially by performance quartile once a trustworthy performance-rating process exists.
- Promotion grants are sized as the delta between current-level and new-level target total-equity bands at current 409A. Pick a blended-with-annual-refresh policy and document it so the comp committee does not approve the same economics twice.
- Retention grants are the exceptional instrument. Three legitimate triggers — credible competing offer, mission-critical status for an upcoming event, one-time retention risk. Everything else goes through the annual refresh. Comp-committee approval above threshold is required; see [chapter 05](./05-compensation-committee.md).
- The refresh budget — commonly 1-3% of fully-diluted per year at scale — competes with new-hire grants for the same option pool. The dilution-budget interaction and the option-pool-top-up negotiation at the next priced round are covered in the `startup-finance-fundraising-curriculum`.
