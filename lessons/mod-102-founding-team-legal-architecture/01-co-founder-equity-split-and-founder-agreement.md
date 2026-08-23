# 1. Co-founder equity split and the founder agreement

> Author a founder agreement that will survive a Series-A diligence read — and hold up when a co-founder walks in year two.

## Motivation

The single most-mishandled conversation on a founding team is the co-founder equity split. It is treated as a one-time negotiation over a static pie ("50/50", "60/40"), captured in a two-page hand-shake, and then contradicted 18 months later when one founder is doing 80% of the work, or has quietly left, or is being asked to take a demotion in a Series-A financing. The founder agreement — an under-loved artefact next to the Stock Purchase Agreement and the PIIA — is what turns that conversation into a governance document with mechanical answers to the predictable failures: who decides what, how disputes get resolved, and what happens to a founder's equity when they walk (or are asked to).

This chapter treats the founder agreement as a real governance instrument, not a talismanic Google Doc. It sits *underneath* the corporation's formal Stock Purchase Agreements (which live in [chapter 02](./02-founders-restricted-stock-and-repurchase.md)) and *alongside* the PIIA (which lives in [chapter 04](./04-piia-mutual-ip-assignment.md)); a diligence reader who cannot reconstruct the founder-team's economic and decision-rights architecture from these three documents will find the deal harder to close.

## What a founder agreement actually contains

A defensible founder agreement covers six things. Some clauses are contractual (the founders binding each other); others are the founder-team's *plan* for what the corporation itself will document in the SPAs, PIIA, and board consent. Both belong here.

1. **Equity split, with rationale on the record.** Not "we agreed 55/40/5" — the *reasons* for that split, captured in enough detail that any of the three founders could explain it to a Series-A investor two years later.
2. **Roles, responsibilities, and titles.** Who is CEO, who is CTO, who owns what functional area, and how titles change if the team composition changes.
3. **Decision authority.** What decisions any founder can make alone; what requires a majority; what requires unanimity; what belongs to the board once a board exists.
4. **Dispute-resolution mechanics.** How founder disagreements get worked (not "we'll figure it out"), including an escalation ladder and — for the intractable case — a tie-breaker.
5. **Walk-away and re-vesting mechanics.** What happens to a founder's equity if they voluntarily leave; if they are terminated for cause; if they are terminated without cause; if they die or are disabled.
6. **IP, moonlighting, and pre-existing-work boundaries.** The founder-facing echoes of what the PIIA (chapter 04) and the anti-conflict baseline (chapter 06) will formalise.

The founder agreement does not replace any of the corporation's formal documents; it is the founders' contract with each other about how they will operate the corporation.

## The equity-split conversation the founders frequently mishandle

The failure mode is nearly identical across teams: two or three technical co-founders sit down over a weekend, feel awkward about assigning numbers to each other, converge on 50/50 (or equal thirds), and move on. Six months in, one founder has left; another has been carrying the technical roadmap; a third is now running sales — and there is no mechanism on the cap table for any of that to matter.

### The variables the split should actually price

A rigorous split conversation touches at least seven inputs. There is no formula that turns them into percentages — the point is that all seven get named on the record.

- **Idea attribution.** Who originated the specific idea that the company is now pursuing? An idea originator sometimes deserves a modest premium, sometimes deserves nothing (ideas without execution are cheap). Founder teams routinely over-weight or under-weight this — the fix is to *name it* and put a number on it.
- **Time commitment starting today.** Is every founder full-time from day one? Is one still finishing a PhD? A "part-time founder" is almost always a wrong pattern for a venture-track startup, and the equity split should reflect it if the pattern persists.
- **Opportunity cost.** What is each founder walking away from — a $400k FAANG job, a tenure-track offer, a paid startup role, or unemployment? Opportunity cost is not the whole answer, but ignoring it produces resentment.
- **Domain expertise and prior credibility.** Does one founder bring a decade of enterprise sales, a well-known research reputation, or the customer relationships that will drive year-one revenue?
- **Cash contribution.** Which founders are putting cash into the corporation for its initial capitalisation (paying for the shares — see [chapter 02](./02-founders-restricted-stock-and-repurchase.md)) and how much?
- **IP contribution.** Which founders are assigning material pre-formation IP into the corporation? IP contribution is a real economic input priced by the SPA's consideration section and echoed in the PIIA (chapter 04).
- **Expected role and long-term function.** Who is expected to hold the CEO seat through Series-B, who is the technical anchor, who is likely to grow into a comparable senior role over time?

The founders should walk through each of these explicitly, write down where they agree and disagree, and land on numbers with the *reasoning* attached. The reasoning is the artefact — the numbers change over time; the reasoning is what future counsel, future board members, and future incoming co-founders will re-read to understand the corporate history.

### Structural options for the split

Three shapes of split appear in practice, in rough order of frequency:

1. **Fixed percentages at formation, protected by vesting.** The classic pattern: e.g., 40 / 35 / 25, with each founder on 4-year vesting with a 1-year cliff. Vesting is the corrective mechanism — a founder who walks in year one leaves with almost nothing.
2. **Equal split with vesting.** 50/50 or 33/33/34, with vesting. Simpler socially, harder to defend when the eventual work contributions diverge sharply.
3. **Dynamic / slicing-pie style splits.** Explicit formulas that update equity over time based on time contributed, cash contributed, and role. These sit poorly against a Series-A cap table and are rare in venture-backed companies; if used at all, they are typically converted to a fixed split at first-priced-round.

For a venture-track company, option 1 is the default. The choice worth debating is *the split*, not *the shape*.

### Anti-patterns to name and avoid

- **The 50/50 "we're best friends, we'll never disagree" split with no tie-breaker.** Every two-founder company hits a hard disagreement eventually. Without a tie-breaker, a locked-up decision consumes a board meeting or worse.
- **The "we'll figure equity out later" formation.** Formation happens with stock issued at par; if the split is not set on formation day, it is set at some later grant date at a higher fair-market value, with immediate ordinary-income tax on the founder receiving the top-up. Set the split at formation, put it on vesting, and adjust *by re-splitting the vesting* (via an amendment to the SPAs and a board consent), not by regranting.
- **The founder who "only has 10%" because they joined a month late.** Joining a month late is a rounding error against a four-year effort. If a founder is truly a co-founder, they should be on a co-founder-scale grant with a vesting start date reflecting their actual start. A 10% co-founder is almost always the wrong economic answer and creates a demotivated 10% owner.
- **The "employee-first-then-promoted-to-founder" pattern.** An early employee promoted to founder-level equity months later often has already been granted options at a stale, low strike; grossing them up to true co-founder economics involves ordinary-income tax and, more importantly, a mixed cap-table story a Series-A investor will ask about. If the person is a founder, name them so on formation day.

## Roles, responsibilities, and decision authority

The founder agreement should be explicit about role allocation and decision rights, not because the founders cannot figure it out day-to-day, but because they cannot figure it out in a *disagreement*.

### Roles

Name the CEO. Two-CEO structures survive marketing memos and die under investor pressure; every institutional venture investor will ask "who is the CEO?" and one founder needs to be able to say "I am." Name every other C-level or founder-title role and the functional area each owns (engineering, product, go-to-market, operations, finance). Roles should be described as *what the founder actually owns*, not just a title on LinkedIn.

### Decision authority

A useful default is a three-tier authority ladder:

- **Individual authority.** Each founder can make decisions inside their functional area up to a defined dollar threshold, a defined headcount threshold, and inside a defined subject-matter scope. Typical formation-day defaults: hiring individual contributors inside your function; committing spend up to $10k on a single purchase and $25k in aggregate per month; signing customer contracts up to a defined ACV.
- **Majority-of-founders authority.** Decisions above the individual thresholds but below the level of the board — hires above a certain seniority, spend above a certain dollar amount, non-standard customer terms, adoption of company-wide policies.
- **Unanimous-of-founders authority.** Decisions with founder-level consequences — issuing equity to a new co-founder, dissolving the corporation, materially changing the product's mission or PBC purpose (if applicable), moving the HQ jurisdiction, accepting an acquisition offer below a defined threshold.

Once a board exists (formation day for most Delaware C-corps — see [mod-101 chapter 02](../mod-101-legal-entity-formation-and-corporate-structure/02-stand-up-the-entity.md)) and once outside investors have board seats, some of these decisions escalate to the board or require investor approval under the priced-round protective provisions. The founder agreement should acknowledge that the founders' authority is subject to board and protective-provision constraints — not stand in opposition to them.

### Dispute resolution

For the small case, the escalation ladder should be:

1. Attempt to resolve at the founder level, on the record (email, decision document).
2. Escalate to the board (once a board with outside directors exists) or to a designated founder-tiebreaker.
3. For deadlocked two-founder companies without an outside director, an ex ante tiebreaker — an advisor, a lead investor's designated observer, or the CEO's tie-breaking vote on non-board matters — is the mechanical fix.

For the large case — a founder wants to leave, a founder wants to force another out, or two founders disagree about a fundamental strategic direction — the answer is often mediation, board intervention, or invocation of the walk-away and re-vesting mechanics below. Prescribing mediation in the founder agreement is cheap and useful; prescribing binding arbitration is more contested and typically deferred to counsel input on formation.

## Walk-away and re-vesting mechanics: the "dead-equity" problem

The single most-consequential clause in the founder agreement is what happens when a co-founder walks. Get this wrong at formation, and you inherit a *dead-equity* founder — someone who left the company with 25% of the common stock, no ongoing contribution, and a permanent overhang on the cap table that future rounds must dilute their way through.

### The default without a repurchase right

In the absence of a repurchase right on the corporation's side, issued shares belong to the founder the moment they are issued. Vesting alone is not enough — vesting only matters if there is a mechanism to reclaim unvested shares on departure. Without that mechanism, a founder who walks the day after formation with 25% of the common stock walks away with 25% of the common stock. Vesting on the founder's calendar is meaningless; the shares are already legally theirs.

This is the *dead-equity founder* pattern. It is fatal at Series-A because a lead investor will not fund a company whose common stock is materially owned by a person who no longer contributes; the fix is usually a difficult and expensive negotiation with the departed founder for a buyback at what will inevitably be higher-than-par valuation.

### The correct default: vesting + repurchase right at cost

The market-standard structure combines two mechanisms:

- **Vesting** — a schedule (typically 4 years with a 1-year cliff, covered in [chapter 02](./02-founders-restricted-stock-and-repurchase.md)) that determines what fraction of the founder's shares are "earned" as of any given date.
- **Repurchase right at cost** — the corporation's contractual right (documented in the Stock Purchase Agreement) to buy back the *unvested* portion of the founder's shares, at the original purchase price, upon the founder's separation from the corporation.

Combined, these two mechanisms mean: when a founder separates, the vested portion of their shares stays with them (they own it); the unvested portion may be repurchased by the corporation at cost (they get their nominal purchase price back for those shares, and the corporation reclaims the equity). This is what makes vesting *real*.

### Distinguishing separation triggers

The founder agreement (and the SPA) should distinguish separation types because the equity treatment differs:

- **Voluntary resignation.** Vested shares stay; unvested shares subject to repurchase at cost.
- **Termination for cause.** Vested shares stay; unvested shares subject to repurchase at cost. In some agreements, an additional "clawback" of vested shares is negotiated for termination for cause based on misconduct (fraud, IP theft, gross negligence); this is a heavier stick and needs to be drafted narrowly to survive as enforceable.
- **Termination without cause.** Vested shares stay; unvested shares may still be subject to repurchase at cost, but this is the trigger where the founder agreement often provides for *acceleration* — some or all of the unvested shares becoming vested on the termination date. Common formations: 3–12 months of accelerated vesting on termination without cause.
- **Death or disability.** Common practice is to accelerate a defined portion (often the next 12 months of vesting, or 100%) and to have the estate/family retain the shares under standard transfer restrictions.
- **Change-of-control acceleration.** Whether some or all of the unvested shares vest on a change-of-control (single-trigger) or only on a change-of-control *plus* termination-without-cause within a defined window (double-trigger) is discussed in [chapter 02](./02-founders-restricted-stock-and-repurchase.md); the mechanics themselves belong to `startup-exit-curriculum`.

The founder agreement should describe the intended treatment for each of these triggers; the SPA is what makes the treatment binding on the corporation and the founder.

### The "for cause" definition matters

"For cause" is a term of art. A narrow definition (fraud, willful misconduct, uncured material breach, felony conviction) protects founders from a co-founder-controlled board firing a founder "for cause" as a pretext. An overly broad definition ("failure to perform assigned duties") is a weapon. The founder agreement — and the SPA — should adopt a defined "for cause" standard, and it should not be defined by whoever holds the majority on a founder-only board.

## Concrete example: the two-founder company that avoided the dead-equity trap

Two founders, A and B, form a Delaware C-corp with an equal 50/50 common-stock split, 8,000,000 shares each, on 4-year vesting with a 1-year cliff. The founder agreement provides:

- Each founder purchases their shares for $0.0001 par per share = $800 cash consideration.
- The Stock Purchase Agreement grants the corporation a right of repurchase at $0.0001 per share for all unvested shares on any separation event.
- "For cause" is defined narrowly.
- On termination without cause, an additional 6 months of vesting accelerates.
- On death or disability, an additional 12 months of vesting accelerates.
- On change-of-control, no single-trigger acceleration; on change-of-control plus involuntary termination within 12 months, 100% of unvested shares accelerate (double-trigger).
- Both founders file § 83(b) elections within 30 days ([chapter 03](./03-83b-election-and-founder-tax-clock.md)).

Fourteen months in, founder B walks to take a job elsewhere. B has vested 14/48 = 29.17% of their 8,000,000 shares = 2,333,333 shares. The corporation exercises its repurchase right on the unvested 5,666,667 shares at $0.0001 per share = $566.67 cash back to B. B leaves with 2,333,333 shares of common stock (14.6% of outstanding at that moment) and continues to hold them as a passive stockholder.

At Series-A one year later, the incoming lead investor asks two questions: (i) is departed-founder B still holding a large common-stock position, and (ii) has that position been diluted proportionally with the priced-round math? The answer to (i) is "yes, 2.33M shares, diluted from 14.6% to ~9% after the round"; the answer to (ii) is yes; the investor accepts this because the vesting-and-repurchase mechanics worked. If A had instead walked with the full 8M shares intact, the investor would have required a buyback or renegotiation before funding.

This is why chapter 02's SPA language and this chapter's founder-agreement language have to match. The reason mod-102 has two chapters on this material is not repetition — it is that both documents matter, both fail differently, and both need to be authored deliberately.

## Anti-conflict, moonlighting, and pre-existing-work echoes

The founder agreement should include founder-facing anti-conflict language even though the *legal* enforcement of these obligations sits in the PIIA (chapter 04) and the anti-conflict baseline (chapter 06). Founders often experience the founder agreement as their primary loyalty covenant to the team; making the expectations explicit here reduces future disputes.

- **No moonlighting on competitive activity.** Each founder commits to devote their full professional time and attention to the corporation, subject to defined exceptions (e.g., continued board seats disclosed today, passive investments below a defined threshold).
- **No competing ventures.** Each founder commits not to found or work for a competitor for as long as they are with the corporation.
- **Pre-existing IP disclosure.** Each founder commits to disclose, on formation day, any prior work that they claim is *not* being assigned to the corporation, so that the PIIA's carveout schedule is complete on day one.
- **Notification of outside opportunities.** Each founder commits to notify the other founders of any outside business opportunity that arguably belongs to the corporation (a "corporate opportunity" — see [chapter 06](./06-founder-conflict-of-interest.md)) before pursuing it personally.

None of these clauses substitute for the PIIA, the employment agreement (chapter 07), or the fiduciary-duty framework — they are the founder-team norms that support the legal architecture.

## What Series-A diligence will actually look at

A Series-A diligence request list will not ask for a "founder agreement" by that name. It will ask for:

- Every founder's Stock Purchase Agreement (chapter 02).
- Every founder's § 83(b) election filing and proof of timely mailing (chapter 03).
- Every founder's executed PIIA (chapter 04).
- Every founder's employment or consulting agreement (chapter 07).
- Any prior agreements among the founders regarding equity allocation, roles, or corporate governance (this chapter).
- Any separation agreements or side letters for founders who have departed (chapter 07).

The founder agreement authored to the standard above is what gives diligence counsel a coherent story about why the numbers on the cap table are what they are. Without it, the diligence process falls back on inference, which usually produces a schedule of exceptions and, in the worst case, a re-negotiation of founder economics before closing.

## Summary

- The founder agreement is a real governance document, not a handshake. It covers equity split with rationale, roles and decision authority, dispute resolution, walk-away and re-vesting mechanics, and IP / moonlighting boundaries.
- The equity-split conversation should price at least seven variables (idea, time, opportunity cost, expertise, cash, IP, expected role) and produce numbers *with reasoning on the record*.
- Vesting alone is not enough; vesting + a repurchase right at cost is what prevents a dead-equity founder from holding the company hostage.
- Distinguish separation triggers (voluntary, for cause, without cause, death / disability, change-of-control) and adopt a *narrow* "for cause" definition to prevent weaponisation.
- The founder agreement supports — and does not replace — the SPA (chapter 02), the 83(b) filing (chapter 03), the PIIA (chapter 04), and the founder-employment relationship (chapter 07). All of them show up on the Series-A diligence request list; the founder agreement is what makes them cohere.
