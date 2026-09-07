# Exercise 01 — Co-founder equity-split conversation drill

> Estimated time: **~3 hours** · Related chapter: [01 — Co-founder equity split and the founder agreement](../01-co-founder-equity-split-and-founder-agreement.md)

## Problem statement

You are the incoming COO / GC for a hypothetical three-founder AI-infrastructure startup that is 30 days away from formation. The founders have circled a "we'll do 50 / 30 / 20 because Alex had the idea" hand-shake and are ready to send an incorporation package to Clerky. Nothing is on the record. Your job — before the shares are issued — is to run the equity-split conversation to the standard chapter 01 describes and produce a **defensible founder agreement** that (a) prices the seven variables on the record, (b) memorialises roles and decision authority, (c) prescribes walk-away and re-vesting mechanics, and (d) sets the anti-conflict baseline the PIIA and employment agreement will echo.

You will not write the SPA or the PIIA yet (those live in exercises 02 and 03). You are writing the *founders' contract with each other* — the governance document that sits underneath the corporation's formal instruments.

## The founding team

- **Alex Chen** — proposed CEO. Originated the specific product idea 8 months ago while a Staff ML Engineer at a public cloud company; wrote a 30-page technical memo and a working prototype. Walking away from a $460k total-comp package (base + RSUs vesting). Domain expertise: distributed inference infrastructure. No prior founding experience. Cash to contribute: $50k.
- **Priya Rao** — proposed CTO. Full-time on the project starting 3 months ago (took unpaid leave from a Series-C startup). Has authored the current architecture and about 40% of the prototype code. Prior Distributed Systems PhD; two prior startups (one exited modestly, one failed). Walking away from a $340k total-comp package. Cash to contribute: $10k. Has been recruited by Alex; would not be doing this without Alex's ask.
- **Marcus Hill** — proposed VP GTM / founding go-to-market. Not yet full-time — currently a VP Sales at an enterprise SaaS company, will start full-time on the formation date. Long-standing customer relationships in the target market that Alex and Priya lack entirely. Walking away from a $380k OTE package. Cash to contribute: $5k. Not a technical contributor; will not touch the codebase.

All three intend to be W-2 employees ([chapter 07](../07-founder-employment-relationship-and-departure.md)) and expect to serve on the initial board.

## Requirements

### Part A — Structured equity-split conversation

Produce a written record of the equity-split conversation that walks through **all seven variables from chapter 01**:

1. Idea attribution
2. Time commitment starting today
3. Opportunity cost
4. Domain expertise and prior credibility
5. Cash contribution
6. IP contribution
7. Expected role and long-term function

For each variable: (a) state the founder-by-founder facts, (b) state where the three founders agree and disagree, and (c) commit to a directional adjustment (up / down / neutral for each founder). The output should be legible enough that a Series-A investor's counsel reading it two years from now can reconstruct the reasoning.

### Part B — Final split with rationale

Propose the specific equity split you would land on. Show your work: the numbers *and* the reasoning that connects them to Part A. Expected format: table with each founder's percentage, absolute share count against a 10,000,000-share initial authorised pool (leaving headroom for a seed option pool — cite your assumption), and a one-paragraph rationale per founder.

You are not being graded on hitting a "correct" split — you are being graded on whether the split is *defensible* against the seven-variable analysis you produced in Part A.

### Part C — Founder agreement

Draft the founder agreement covering, at minimum:

1. **Equity split** — with the Part B rationale attached as a recital or exhibit.
2. **Roles, titles, and functional-area ownership** — including who is the sole CEO (chapter 01 requires this).
3. **Decision authority ladder** — individual authority (with dollar and headcount thresholds), majority-of-founders authority, and unanimous-of-founders authority. Acknowledge board and (eventual) investor protective-provision limits.
4. **Dispute-resolution mechanics** — escalation ladder for the small case and the deadlock mechanism for the large case (given a three-founder board without an outside director on day one).
5. **Walk-away and re-vesting mechanics** — narrative description of the treatment for voluntary resignation, termination for cause (with a defined-narrowly "for cause"), termination without cause (with any acceleration), death or disability, and change-of-control (double-trigger baseline; single-trigger deferred to `startup-exit-curriculum`).
6. **Anti-conflict baseline** — no-moonlighting, no-competitive-activity, pre-existing-IP disclosure, and corporate-opportunity notification, calibrated to what each founder is actually walking into (Marcus's transition, Priya's PhD spinoff overlap if any, Alex's prior-employer overlap).

The founder agreement should explicitly note that the SPA (exercise 02) and the PIIA (exercise 03) will make specific provisions binding on the corporation and the founder respectively, and that this founder agreement is the founders' contract with *each other*.

### Part D — Boundary-issue call-outs

Identify at least three anti-pattern risks specific to this founding team that a diligence reader will surface, and document how the founder agreement mitigates each. Candidates include (not exhaustive): Marcus's pre-formation part-time status; Priya's prior employer's PIIA obligations that may cover work from her 3-month unpaid leave; Alex's continuing RSU vesting at the prior employer during transition; the three-founder-director board with no outside tiebreaker; the disparate cash contributions.

## Starter guidance

- Do not converge on the split before running Part A. The purpose of the exercise is that the *conversation happens on the record*.
- Read chapter 01 sections "The variables the split should actually price," "Structural options for the split," and "Anti-patterns to name and avoid" before starting.
- The "narrow for-cause" definition should not include "failure to perform assigned duties." Use fraud, willful misconduct, uncured material breach, or felony conviction as your baseline and adjust from there with reasoning.
- For dispute resolution on a three-founder-director board without an outside director, chapter 01 identifies three viable tiebreaker mechanics — pick one and defend it. Do not leave the deadlock unaddressed.
- If you propose non-standard vesting (backloaded, longer cliff, prior-service credit), justify it against chapter 02's default; SPAs come next exercise but the agreement should signal the vesting intent.
- Do not include an SPA or a PIIA inside the founder agreement — cross-reference them.
- Anything you cannot verify from the fact pattern above, assume with a written assumption; do not invent facts about founder backgrounds beyond what is given.

## Deliverables

- `equity-split-conversation-memo.md` — Parts A and B. The seven-variable analysis and the final split with rationale.
- `founder-agreement.md` — Part C. The signed-ready founder agreement.
- `boundary-issues-memo.md` — Part D. Anti-pattern risks and mitigations.

## Acceptance criteria

The package is acceptable if:

1. All seven variables from chapter 01 are addressed for each founder, with facts, points of agreement / disagreement, and directional adjustment.
2. The final split is *defensible* against the analysis — a reader can trace each number back to a variable.
3. The founder agreement covers all six clause categories from chapter 01's "What a founder agreement actually contains" and does not leave any category as `[TBD]`.
4. The "for cause" definition is narrow and specific.
5. The dispute-resolution mechanism handles the deadlock case for a three-founder board with no outside director.
6. Walk-away and re-vesting mechanics distinguish all five separation triggers from chapter 01, with treatment for each.
7. Anti-conflict language references the PIIA and employment-agreement echoes without duplicating their legal text.
8. Part D identifies at least three real anti-pattern risks in this founding team and shows how the founder agreement mitigates each.
9. Nothing invented — every founder fact used is traceable to the fact pattern or to a written, flagged assumption.
