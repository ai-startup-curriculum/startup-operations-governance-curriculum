# 7. Change-of-control equity policy

> The change-of-control policy is where the corporation decides, in advance of any transaction, how much of the exec team's unvested equity will accelerate — and the right answer is almost always "double-trigger, with a handful of named exceptions and a 280G strategy that keeps the deal from eating itself."

## Motivation

Every exec equity grant the corporation issues contains a latent clause: *what happens to this grant if the corporation is acquired?* The question is small when the corporation is small and the equity is worth little, and it becomes a board-level governance question the moment a term sheet is on the table. Deferring the answer until a transaction appears is one of the recurring and expensive governance failures in venture-backed companies — because by the time the term sheet arrives, the acquirer, the board, the exec team, and the IRC § 280G calculator are all operating against each other with different information and different leverage.

The change-of-control ("CoC") equity policy is the pre-committed answer. It lives in three documents — the equity plan, the individual grant notice, and the exec severance agreement — and it is the policy the comp committee writes *before* a transaction is in motion so that it is not negotiated under duress. The modern US venture-backed default is a double-trigger standard with narrow single-trigger exceptions, assumption-or-substitution treatment at close, and a 280G-conscious design that avoids stacking accelerations into a parachute problem.

This chapter builds that policy end-to-end: the definitions, the trigger standards, the treatment of unvested equity in each transaction structure, the ESPP and ISO interactions, the § 280G overlay, and the drafting mechanics (which document controls which clause). The transaction-execution-side of a real exit sits in [`startup-exit-curriculum`](../../../startup-exit-curriculum/); the deal-structuring economics sit in [`startup-finance-fundraising-curriculum`](../../../startup-finance-fundraising-curriculum/); this chapter is the *policy design* that both of those downstream workflows inherit.

## Definitions — what counts as a change in control

The first governance mistake is to assume "change in control" is self-defining. It is not. Every equity plan and every individual exec agreement defines CoC explicitly, and the definitions are not identical across documents even inside the same corporation.

### The plan-level CoC definition

The CoC definition in the equity plan document is the plan-level default — it applies to every grant issued under the plan unless the grant notice or an individual agreement overrides it. The canonical US-venture-backed definition enumerates four triggers:

- **Asset sale.** A sale, lease, exclusive license, or other disposition of all or substantially all of the corporation's assets. "Substantially all" is a facts-and-circumstances test and is not a bright-line percentage; the comp committee should assume ~<!-- needs-research: confirm the Delaware "substantially all" asset-sale threshold as developed in case law (Gimbel v. Signal Companies, Hollinger Int'l v. Black); commonly cited rough-order threshold is ~75% of asset value but the test is qualitative not quantitative. --> as a working rule of thumb.
- **Merger or consolidation.** A merger, consolidation, or similar transaction in which more than 50% of the corporation's voting power transfers to a non-pre-existing holder group. The policy carve-out is important here: a pure recapitalisation in which the same holder group retains >50% voting power is *not* a CoC.
- **Stock acquisition.** The acquisition by any single person or entity, or by a coordinated group acting together, of more than 50% of the corporation's outstanding voting power. The "coordinated group" language is what defeats the structural end-run of splitting the acquisition across two nominally independent entities.
- **Hostile-board-replacement trigger.** The replacement of a majority of the incumbent board within a defined window — commonly 12 or 24 months — by directors not nominated or endorsed by the incumbent board. This is the hostile-takeover trigger. It is present in most well-drafted plan definitions and it is the one most often omitted in rushed plan documents.

### "Change in control" vs. "change in capital structure"

A financing round — a priced preferred-stock issuance, even one in which the new investors acquire a controlling preferred stake — is **not** a CoC event. It is a change in capital structure. The distinction matters because the acceleration clauses the exec team cares about should not trigger when the Series-C closes. Well-drafted equity plans say so explicitly, and well-drafted exec agreements say so explicitly in parallel.

The failure mode is a sloppy exec agreement that defines CoC as "any transaction in which >50% of the equity transfers" without the capital-structure carve-out — such an agreement would, read literally, be triggered by a sufficiently large preferred round. Comp committees should audit for this language on every new exec agreement.

### Exec-agreement-level overrides

The individual exec severance / employment agreement often *overrides* the plan-level CoC definition for that exec. Common exec-level overrides:

- A narrower definition that removes the hostile-board-replacement trigger (acquirers sometimes negotiate this out of post-close exec agreements).
- A broader "good reason" definition (see below) that effectively lowers the bar for the second trigger.
- A definition that explicitly includes a secondary-sale transaction (e.g., a tender offer for common and vested-option shares at a premium) as a CoC, which some execs negotiate for post-ratchet protection.

The hierarchy — plan default, grant override, exec-agreement override — is covered under *Policy drafting mechanics* below.

## The double-trigger standard

### What double-trigger means

The modern US-venture-backed default is a **double-trigger** acceleration standard: unvested equity accelerates only if (1) a CoC event occurs *and* (2) the exec is involuntarily terminated without cause, or resigns for good reason, within a defined post-CoC window — most commonly 12 months, sometimes 18 months, occasionally 24 months for the CEO.

The structural logic of double-trigger is a two-sided risk allocation:

- **Protects the acquirer** from immediate exec flight. If every exec's unvested equity accelerated at close, the acquirer would be purchasing a corporation whose entire exec team is suddenly fully vested and economically free to leave the day after close. Acquirers price this risk aggressively — in a single-trigger-heavy cap table, the acquirer discounts the headline price.
- **Protects the exec** from being terminated after close without acceleration. If the exec's acceleration required only a termination (no CoC), the corporation could terminate the exec before any transaction and avoid the acceleration cost. If acceleration required only a CoC (no termination), the exec would get a windfall even if they chose to stay. The double trigger allocates the acceleration *to the specific economic harm it is intended to remedy* — being terminated by the acquirer after a transaction the exec helped create.

### "Good reason" — the critical definition

The second trigger is the one most often litigated, and the "good reason" definition is where most of the drafting work lives. Market-standard "good reason" clauses enumerate specific triggering events:

- A material reduction in base salary (commonly ≥10% reduction, measured against pre-CoC base).
- A material reduction in duties, authority, or responsibilities (the hardest to adjudicate — the comp committee should require the clause to specify the pre-CoC role as the baseline).
- A material reduction in title (CFO becoming "VP, Finance" post-close is the canonical example).
- A required relocation of the exec's primary work location by more than a defined distance — commonly 35 or 50 miles.
- A material breach of the exec's employment agreement by the corporation (or the successor).

Every market-standard clause requires a **notice-and-cure process**: the exec must notify the corporation in writing within a defined window (commonly 30 or 60 days) of the good-reason event, the corporation has a defined cure window (commonly 30 days) to cure the event, and the exec must resign within a defined window after the cure period expires if they intend to claim the acceleration. Without this notice-and-cure protocol, a stale "good reason" claim can be asserted months after the triggering event — which is both bad drafting and bad governance.

### The post-CoC window

The post-CoC window — the period during which the second trigger must occur for acceleration to apply — is a negotiated term:

- **12 months** is the mode for most exec roles.
- **18 months** is common for the CEO and sometimes the CFO.
- **24 months** is rare and typically only for a founder-CEO as part of founder protection.

The longer the window, the more exec protection and the more the acquirer discounts the deal. Comp committees should set the policy default (commonly 12 months) and allow exceptions by role, documented in the exec agreement.

## Single-trigger and modified-single-trigger — the exceptions

### Pure single-trigger

**Pure single-trigger** acceleration — acceleration on the CoC alone, regardless of termination — is rare in modern US-venture-backed exec packages and is treated by ISS and Glass Lewis as a *problematic pay practice* at pre-IPO companies. The institutional-investor advisory firms (see [chapter 09](./09-sec-reg-sk-item-402-disclosure.md) on disclosure of CoC terms) flag single-trigger CoC in their voting policies and will typically recommend AGAINST say-on-pay or against comp-committee-member re-election if single-trigger is present at a public company.

The narrow situations where single-trigger occasionally appears:

- **Hired CEO.** A CEO recruited from outside, usually at a late-stage private or near-IPO company, sometimes negotiates single-trigger as part of the recruiting package. Rare and board-visible.
- **Founder-CEO (founder protection).** A founder-CEO's grant may have single-trigger as part of the original founder equity structure, particularly if the founder is also the largest common holder and the acceleration is viewed as a founder-protection mechanism rather than an exec-comp mechanism.
- **CFO (orderly-transition rationale).** Occasionally the CFO is given single-trigger on the argument that the CFO's role in deal execution and post-close transition makes immediate full-vesting part of the compensation for shepherding the transaction. This is a defensible but minority practice.

Single-trigger is *not* market-standard for CFO (except as noted), COO, CPO, CMO, GC, or any other named exec. Comp committees should treat a request for single-trigger as an exception requiring explicit board approval and a documented rationale.

### Modified single-trigger ("walk-away" right)

A **modified single-trigger** — sometimes called a "walk-away right" or a "single-trigger-with-resignation" — allows the exec to resign on their own initiative within a defined post-CoC window (commonly 12 months) and still receive full acceleration plus severance. The structure is nominally two-step (CoC + resignation) but functionally single-trigger because the second trigger is at the exec's sole discretion.

ISS and Glass Lewis treat modified-single-trigger similarly to pure single-trigger — as a problematic pay practice. Comp committees should assume modified-single-trigger will draw the same advisory-firm negative recommendation and should document the rationale accordingly.

## Treatment of unvested equity at close

Separate from the acceleration-trigger question is the question of what the acquirer *does with* the outstanding equity grants — vested and unvested — at close. The equity plan should enumerate the available treatments and specify which the plan administrator (post-close, the acquirer or the successor comp committee) may elect.

### Assumption or substitution

The acquirer **assumes** the outstanding grants on their existing terms, or **substitutes** acquirer-stock-denominated grants with economically equivalent terms (adjusted for the exchange ratio in a stock-for-stock deal). The vesting schedule continues; the acceleration terms attach to the acquirer-stock grant going forward. This is the most common treatment in stock-for-stock and in many cash-and-stock deals, and it is the treatment that integrates cleanly with the double-trigger standard (because the second trigger — post-close termination — happens inside the acquirer).

### Cash-out

The acquirer **pays cash** at close for the outstanding grants. Vested options are cashed out at (deal price − strike) × vested shares. Unvested grants are either (a) accelerated per the single- or double-trigger terms and cashed out at the same spread, (b) continued as a cash-vesting arrangement (the exec receives the cash on the original vesting schedule, subject to continued employment), or (c) cancelled if the unvested grant does not qualify for acceleration and the plan does not require continuation.

The cash-vesting-continuation structure is the acquirer's typical hedge against post-close exec flight: it gives the double-trigger exec the economics they bargained for while retaining the retention lever of forfeiture-on-resignation. The policy design in the equity plan should permit all three sub-structures and defer the election to the acquirer.

### Cancellation for lesser or no consideration

The acquirer **cancels** the outstanding grants for lesser or no consideration. This is rare and in practice applies only where (a) the deal value is at or below the strike price such that the option is underwater — the holder is not economically harmed by cancellation at zero — or (b) the unvested-and-non-accelerated portion is cancelled under the terms of the double-trigger clause and no alternative continuation is offered. The plan should explicitly permit cancellation of underwater options for zero consideration.

### Acceleration

The acquirer applies the plan-level or grant-level acceleration — fully vesting the unvested shares at close (single-trigger) or at the second-trigger event (double-trigger). The acceleration can be combined with any of the three treatments above: an accelerated grant can be assumed, cashed out, or (less commonly) continued as a cash-vesting arrangement on its original schedule now treated as vested.

## ESPP in a transaction

The employee stock purchase plan interacts with CoC through a terminate-and-purchase clause in the plan document. Market-standard ESPP language gives the plan administrator two options at CoC:

- **Close and purchase (market standard).** The current offering period is shortened to end immediately prior to the CoC closing. Participants' contributions-to-date are used to purchase shares at the lower of (a) the fair market value at the start of the offering period and (b) the shortened-period purchase-date fair market value (which, in a cash deal, is the deal price). The purchased shares then participate in the transaction consideration like any other outstanding common share.
- **Cancel and refund.** The current offering period is cancelled and contributions-to-date are refunded in cash to participants without a share purchase.

The close-and-purchase treatment is strongly preferred by employees — in a successful exit it typically produces a meaningful spread (deal price − start-of-period FMV × shares purchasable with contributions) which is the economic value of the ESPP's § 423 "look-back" feature. Comp committees should ensure the ESPP plan document specifies close-and-purchase as the default and the administrator has discretion only in narrow circumstances (e.g., where the ESPP's § 423 qualification is at risk because the deal structure fails one of the § 423 requirements).

## ISO-to-cash-tender treatment

Incentive stock options cashed out in a transaction lose their ISO tax treatment because the holding-period requirements under IRC § 422(a) — two years from grant and one year from exercise — are not met (the "exercise" is deemed to occur at the cash-tender close). The result is that the spread (deal price − strike) × shares is taxed as **ordinary income** to the holder at close, as if the options were NSOs. The corporation gets a corresponding ordinary-income tax deduction.

The interaction with transaction structure:

- **Stock-for-stock.** If the ISO grant is **assumed or substituted** rather than cashed out, the ISO treatment can survive — the holding-period clock continues on the substituted acquirer-stock option. This is the preferred outcome from the holder's perspective.
- **All-cash.** ISOs cashed out at close become ordinary-income events. Nothing the plan drafting can do changes this — the structure of the transaction, not the plan, is dispositive.
- **Cash-and-stock.** The plan document and the acquirer's election control the allocation; typically a mix of cash and acquirer-stock produces a split outcome.

The transaction-side tax mechanics are covered in [`startup-exit-curriculum`](../../../startup-exit-curriculum/); the policy-level implication for mod-105 is that the equity plan should permit ISO assumption / substitution in stock-for-stock and cash-and-stock deals so that the holder-favourable outcome is available where the structure allows.

## Transfer-of-award mechanics by transaction type

- **Stock-for-stock.** Unvested options convert to acquirer-stock options at the deal's exchange ratio with proportionate strike adjustment. Vesting continues on the acquirer-stock option; the double-trigger acceleration clause attaches to the new grant. ISO treatment is preserved where § 424(a) substitution requirements are met.
- **Cash-and-stock.** Split treatment per the acquirer's election and the plan's permitted treatments. The equity plan document controls what the acquirer may elect; a well-drafted plan permits assumption, substitution, cash-out, continuation, and acceleration in combination.
- **All-cash.** Vested options cash out at (deal price − strike) × vested shares. Unvested options either (a) accelerate at close and cash out at the same spread (if single-trigger applies), (b) accelerate on second trigger and cash out via a holdback or escrow arrangement (if double-trigger applies), or (c) cancel at close (if neither trigger applies and the plan does not require continuation).

## IRC § 280G and § 4999 overlay

### What § 280G and § 4999 do

The parachute-payment rules under IRC § 280G and § 4999 ([26 C.F.R. § 1.280G-1](https://www.law.cornell.edu/cfr/text/26/1.280G-1)) impose two penalties when CoC-contingent compensation to a "disqualified individual" exceeds a defined threshold:

- The recipient owes a **20% excise tax under § 4999** on the "excess parachute payment" — the portion of the CoC-contingent compensation that exceeds the recipient's "base amount."
- The corporation **loses the deduction under § 280G** for the excess parachute payment.

The triggering threshold is that the aggregate CoC-contingent payment to the disqualified individual equals or exceeds **3× the base amount**, where the base amount is the recipient's 5-year average W-2 compensation (or the compensation for the period of employment if less than 5 years). When the 3× threshold is crossed, the excess over 1× base amount — not just the excess over 3× — becomes the excess parachute payment subject to both penalties.

### The private-company shareholder-approval cleanse

Private companies have an escape hatch under **IRC § 280G(b)(5)(A)(ii)**: if 75% of the disinterested shareholders approve the parachute payments after full disclosure of the amounts, the payments are **not** parachute payments and the § 280G / § 4999 penalties do not apply. The cleanse is a routine CoC workflow at private companies — typically run in the three-to-four weeks before close as part of the signing-to-closing checklist.

The cleanse is unavailable to public companies, which means the § 280G problem at a public company is a *real* problem that must be solved by payment design: either by reducing the parachute payment below 3× base amount (the "cutback" approach), by grossing up the exec for the excise tax (rare post-Dodd-Frank), or by applying a "best-net" calculation that computes which of the two outcomes leaves the exec with more after-tax cash.

### Policy design to avoid stacking

The mod-105 CoC policy's job is to **avoid stacking** accelerations that force a 280G problem in the first place. The common stacking failure modes:

- A double-trigger acceleration of unvested options, combined with a cash severance payment under the exec severance program (see [chapter 08](./08-executive-severance-and-release.md)), combined with a transaction bonus specifically contingent on CoC closing — three CoC-contingent payments to the same disqualified individual, which collectively exceed 3× base amount.
- An unusually dense recent-vesting pattern that produces a large single-year W-2 immediately preceding the CoC — paradoxically, a *higher* recent-year W-2 *raises* the base amount and may reduce the § 280G exposure.
- A newly hired exec with a short employment history and therefore a short base-amount averaging period — the exec is more likely to cross the 3× threshold because their base amount is lower.

The policy design response is to (a) model the § 280G exposure for each named exec at the time the CoC policy is adopted (and update it annually), (b) coordinate the acceleration schedule with the severance program to avoid stacking, and (c) include a best-net cutback clause in the exec severance agreement so that the exec is not economically disadvantaged by crossing the threshold.

The § 280G *analysis at transaction execution* — the per-exec parachute-payment computation, the shareholder-approval mechanics, the Q&A memo to disinterested shareholders — belongs to [`startup-exit-curriculum`](../../../startup-exit-curriculum/). The *policy design that keeps the analysis manageable* belongs here.

## Rule 10b5-1 and the CoC window — a post-IPO flag

Post-IPO, the Rule 10b5-1 trading plans (see [17 C.F.R. § 240.10b5-1](https://www.law.cornell.edu/cfr/text/17/240.10b5-1)) of named execs interact with CoC in a specific way: the pending-but-undisclosed negotiation of a potential CoC transaction is material non-public information, and continuing to trade under a pre-existing 10b5-1 plan during that period raises affirmative-defence questions.

Market practice is for the general counsel (via a blackout notice or a plan-suspension protocol in the issuer's insider-trading policy) to suspend 10b5-1 plan trades during active M&A negotiations and to resume trading only after the transaction is either closed or publicly abandoned. The policy design detail is to ensure the issuer's insider-trading policy and the CoC policy point at each other — a flag in the CoC policy noting the 10b5-1 interaction, and a flag in the insider-trading policy noting the CoC-negotiation blackout protocol.

Full treatment of 10b5-1 plan design and administration sits in the post-IPO insider-trading-policy chapter and in the SEC disclosure chapter ([chapter 09](./09-sec-reg-sk-item-402-disclosure.md)).

## Policy drafting mechanics — where CoC terms live

The CoC terms applicable to a given exec's unvested equity are determined by a hierarchy of documents:

1. **Plan-level default (equity plan document).** The CoC definition, the available treatments at close, and the default acceleration standard (double-trigger, 12-month window, standard good-reason definition) are specified in the equity plan. See [chapter 02](./02-ic-equity-plan-structure.md) on IC equity plan structure for the plan-level drafting choices.
2. **Grant-level override (grant notice).** The individual grant notice can override the plan default for a specific grant — e.g., a specific grant with a longer post-CoC window or an acceleration schedule that differs from the plan default. In practice, grant-level overrides are uncommon for ICs and are reserved for named-exec grants.
3. **Exec-level override (employment / severance agreement).** The individual exec employment or severance agreement overrides both the plan default and the grant notice for that exec. This is where the single-trigger exception, the 18-month post-CoC window for the CEO, and the exec-specific good-reason definition typically live. See [chapter 04](./04-executive-compensation-packages.md) on exec compensation packages and [chapter 08](./08-executive-severance-and-release.md) on exec severance.

The hierarchy matters when drafting because an inconsistency between the three documents is resolved in favour of the most-specific document — typically the exec agreement. Comp committees should (a) audit the three documents for internal consistency at each exec grant and at each exec agreement renewal, and (b) maintain a one-page cross-reference table for the named execs so that the applicable acceleration terms for each exec can be read off a single sheet.

### The CoC policy brief

The CoC policy brief is a **1–2 page document** that the comp committee adopts and the board ratifies. It summarises:

- The plan-level double-trigger standard, the 12-month post-CoC window, and the market-standard good-reason definition.
- The named-exec exceptions (which execs, if any, have single-trigger or modified-single-trigger; the rationale; the board vote adopting the exception).
- The treatment-at-close options the plan permits (assumption, substitution, cash-out, continuation, acceleration, cancellation of underwater options).
- The § 280G strategy — most commonly a best-net cutback in the exec severance agreement, modelled annually against each named exec's base amount.
- The ESPP CoC treatment (close-and-purchase as default).
- Pointers to the exec severance program ([chapter 08](./08-executive-severance-and-release.md)) and the disclosure obligations ([chapter 09](./09-sec-reg-sk-item-402-disclosure.md) and the Item 402 CD&A at [reg-sk-item-402-disclosure](./09-sec-reg-sk-item-402-disclosure.md)).

The brief is the document the comp committee re-reads when a term sheet arrives — the one-sheet that says "this is the policy we adopted when we were not under deal pressure, these are the exceptions we approved and why, and this is the § 280G calculation we have been maintaining."

## A worked example

**Fictional corporation.** *Northstream Signals, Inc.*, a Series-C industrial-telemetry SaaS corporation, 220 employees, Delaware C-corp, pre-IPO. The CEO is a founder, holds <!-- needs-research: this is a worked example — founder-CEO common-stock position is left unspecified; the point of the example is the policy flow not the cap table. --> of outstanding common. The CFO (external hire, year 2), CRO (external hire, year 3), CPO (external hire, year 1), and GC (external hire, year 2) each hold ISO / NSO grants under the 2022 Equity Incentive Plan.

**The CoC policy as adopted.**

- Plan-level double-trigger standard, 12-month post-CoC window, market-standard good-reason definition (notice-and-cure protocol: 60-day notice, 30-day cure, resign within 30 days of cure-period expiry).
- Named-exec exceptions: the founder-CEO has an 18-month post-CoC window and a single-trigger carve-out on 50% of the unvested grant with double-trigger on the remaining 50% (founder-protection rationale, approved by board resolution dated <!-- needs-research: date-of-resolution is unspecified — this is a worked example, not an actual corporation -->). The CFO, CRO, CPO, and GC are all double-trigger with 12-month windows and no single-trigger.
- Treatment-at-close: the plan permits assumption, substitution, cash-out, continuation, and acceleration, at the acquirer's election.
- § 280G strategy: best-net cutback in the exec severance agreements; annual modelling of each named exec's base amount; private-company shareholder-approval cleanse under § 280G(b)(5)(A)(ii) to be executed in the signing-to-closing window.
- ESPP: close-and-purchase on the next-scheduled purchase date, which the plan administrator will accelerate to immediately prior to CoC closing.

**The transaction.** A strategic acquirer — *Meridian Industrial Networks* — offers a **cash-and-stock** acquisition at a headline enterprise value of <!-- needs-research: deal value unspecified — the point of the example is the policy flow -->. The consideration mix is 60% acquirer stock, 40% cash.

**How the policy flows through to closing.**

1. **CoC trigger.** The transaction closes as a merger in which >50% of Northstream's voting power transfers — a plan-level CoC under definition (b). The capital-structure carve-out is not implicated.
2. **Treatment of unvested equity.** Meridian elects **assumption** for the stock portion and **cash-out** for the cash portion — split 60/40 across every grant.
3. **Acceleration at close.** The founder-CEO's single-trigger-50% portion accelerates at close under the single-trigger carve-out. The remaining 50% of the founder-CEO grant plus 100% of every other named exec grant *does not* accelerate at close under the double-trigger rule — those grants are assumed (stock portion) and continued on the original vesting schedule as a cash-vesting arrangement (cash portion), with acceleration contingent on the second trigger within the 12-month window (18 months for the founder-CEO).
4. **§ 280G analysis.** The comp committee's modelling flags that the CFO and CRO are at risk of crossing the 3× threshold when the single-trigger-equivalent-value of the assumption + any transaction bonus is included. The best-net cutback clause in their severance agreements is engaged. The private-company shareholder-approval cleanse under § 280G(b)(5)(A)(ii) is run in the three weeks before closing — the parachute amounts are disclosed to the disinterested shareholders, 75% approval is obtained, and the § 4999 excise tax and § 280G deduction loss are both avoided.
5. **ESPP.** The current offering period is shortened to end on the business day before closing. Contributions-to-date are used to purchase shares at the lower of (a) the start-of-period FMV and (b) the shortened-period purchase-date FMV, which in a cash-and-stock deal is the implied per-share deal price. The purchased shares participate in the transaction consideration like any other common share.
6. **ISO treatment.** The ISO grants that are assumed by Meridian retain their § 422 holding-period clock (assuming the § 424(a) substitution requirements are met). The portion cashed out loses ISO treatment and is taxed as ordinary income on the spread at close.
7. **Post-close.** Within the 12-month post-CoC window (18 months for the founder-CEO), any named exec terminated without cause or resigning for good reason triggers the second trigger. The remaining unvested equity accelerates and the cash-vesting continuation is paid out immediately in cash.

The policy flow at closing is executed in a two-week signing-to-closing checklist that the GC, CFO, and comp-committee chair run jointly with Meridian's deal counsel. The policy brief is the one-sheet reference document the comp-committee chair carries into every closing meeting.

## Summary

- The CoC policy is a pre-committed answer, adopted by the comp committee before any transaction is in motion, that specifies the definition, the acceleration standard, the treatment-at-close options, the § 280G strategy, and the hierarchy among the equity plan, grant notice, and exec severance agreement.
- The modern US-venture-backed default is **double-trigger** (CoC + involuntary termination or resignation for good reason within a 12–18 month window). Pure single-trigger and modified-single-trigger are rare exceptions, limited to narrow role-based cases, and treated as problematic pay practices by ISS and Glass Lewis.
- Treatment of unvested equity at close is a plan-level menu — **assumption, substitution, cash-out, continuation, acceleration, cancellation of underwater options** — with the acquirer typically electing the mix. The policy should permit all options and defer the choice to deal execution.
- The **IRC § 280G / § 4999** overlay turns stacked acceleration into a real tax penalty when CoC-contingent payments exceed 3× the recipient's base amount. Private companies have the § 280G(b)(5)(A)(ii) shareholder-approval cleanse; public companies do not. Policy design should avoid stacking and build a best-net cutback into the exec severance agreement.
- The ESPP's standard CoC treatment is **close-and-purchase** on an accelerated purchase date at the lower of start-of-period and purchase-date FMV; ISOs lose ISO treatment on cash-out but can retain it on § 424(a)-compliant substitution.
- The deliverable is a **1–2 page CoC policy brief** that cross-references the equity plan ([chapter 02](./02-ic-equity-plan-structure.md)), the exec compensation packages ([chapter 04](./04-executive-compensation-packages.md)), the exec severance program ([chapter 08](./08-executive-severance-and-release.md)), and the SEC disclosure obligations ([chapter 09](./09-sec-reg-sk-item-402-disclosure.md)) — and that reads cleanly against the deal-structuring economics in [`startup-finance-fundraising-curriculum`](../../../startup-finance-fundraising-curriculum/) and the transaction-execution workflow in [`startup-exit-curriculum`](../../../startup-exit-curriculum/).
