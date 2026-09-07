# Exercise 07 — Founder-diligence failure teardown and retroactive cleanup

> Estimated time: **~5 hours** · Related chapter: [08 — Founder-diligence failure teardown and retroactive cleanup](../08-founder-diligence-failure-teardown.md)

## Problem statement

You are the incoming COO / GC at a **different corporation** than the earlier exercises' three-founder team. You joined 5 weeks ago. The corporation was formed 26 months ago using an incorporation service; it has raised a seed round; a Series-A term sheet from a Tier-1 lead investor is expected in 6–10 weeks. There has been no corporate secretary. Your first mandate is a **Founder Documentation State** memo that diagnoses the founder-side defects, prescribes the retroactive cleanup, and identifies which items are curable, which are disclosable, and which will be schedule-of-exceptions items on the Series-A SPA.

Chapter 08 walks the four recurring defects and the cleanup playbook. This exercise runs you through the full cycle on a specific fact pattern.

## The four founders and their documentation state

### Founder A — Jordan (CEO)

- SPA: on file. 4/1 vesting, 1-year cliff, vesting-start = formation date. Repurchase right at cost included. Standard reps and covenants.
- 83(b): filed timely, receipt archived.
- PIIA: on file. Present-assignment language. DTSA whistleblower notice included. Prior Inventions schedule complete.
- Employment agreement: executed.
- **Status:** Clean.

### Founder B — Sam (CTO)

- SPA: on file. 4/1 vesting, 1-year cliff. Repurchase right at cost included.
- **83(b): never filed.** Sam forgot; the 30-day deadline lapsed 24 months ago. The corporation's 409A has moved materially since formation (from $0.0001 par to a $0.42-per-share common valuation at the seed round).
- PIIA: on file. Present-assignment language. DTSA whistleblower notice included.
- Employment agreement: executed.
- **Status:** Missed 83(b). Not curable via repurchase-and-reissuance (FMV has moved).

### Founder C — Riley (VP Product; joined 4 months after formation)

- SPA: on file. 4/1 vesting, 1-year cliff, vesting-start = Riley's actual start date. Repurchase right at cost included.
- 83(b): filed timely, receipt archived.
- **PIIA: 2015-vintage template.** No DTSA whistleblower notice. Uses "agrees to assign" (future-promise) language, not "hereby assigns." No California Lab. Code § 2870 carveout (Riley is based in California).
- Employment agreement: executed.
- **Status:** Defective PIIA on three counts (DTSA notice missing, wrong assignment tense per *Stanford v. Roche*, missing state carveout).

### Founder D — Casey (Head of Growth; "promoted" to founder-scale grant at month 12)

- **SPA: never signed.** Casey was granted 1,200,000 shares of restricted stock at month 12 by board consent, but no SPA was ever executed to document the vesting schedule, the repurchase right, or the founder reps.
- **83(b): never filed.** No SPA, so no transfer date established; but the shares were issued and Casey is a legal owner as of the board consent.
- **PIIA: not fully executed.** Casey signed an offer-letter-embedded 3-paragraph confidentiality clause when hired as an employee, but never signed the full PIIA.
- Employment agreement: an outdated offer letter that predates the promotion.
- **Status:** All four defects present in some form.

## Requirements

### Part A — Founder-by-founder diagnosis

For each of the four founders, produce a diagnostic entry (~half a page each) covering:

1. **Defects present** — mapped to chapter 08's four categories.
2. **Severity** — curable / disclosable / closing-condition-blocker.
3. **Time sensitivity** — what has to happen in the next 2 weeks vs. before Series-A closing.
4. **Cross-references** — which items depend on other items being resolved first (e.g., Casey's SPA has to exist before Casey's PIIA can be reconciled to a clean state).

### Part B — Personnel matrix

Produce a personnel matrix per chapter 08 that captures, for every current founder:

- Name and role.
- SPA executed (date, vesting schedule, repurchase right present).
- 83(b) filed (date, receipt archived).
- PIIA executed (date, effective date, present-assignment language, DTSA notice, state carveout).
- Employment agreement executed.
- Defects and cleanup status.

Add columns for the retroactive-cleanup work: cleanup owner, target completion date, board-consent authorising the cleanup, disclosure treatment on the Series-A schedule of exceptions.

### Part C — Retroactive-cleanup documents

Author the retroactive cleanup for each founder:

#### For Founder A (Jordan)

- No action needed. Confirm the file is complete and add Jordan's entries to the matrix.

#### For Founder B (Sam) — missed 83(b)

Produce:

1. **Tax-exposure memo.** Model Sam's § 83(a) ordinary-income exposure at each historical vesting event against the applicable common-stock 409A on that date (assume par at formation, $0.05 at 12 months, $0.42 at the seed round 18 months in, and $0.55 at your current date). Attach the calculation.
2. **Amended-return plan.** A short plan for Sam to amend the prior-year returns and pay the associated tax with interest and penalties. Note that the corporation's payroll-tax reporting also needs adjustment for the historical vesting events.
3. **Tax-gross-up analysis (optional).** Whether the corporation should adopt a policy of grossing up Sam's tax exposure. If yes, produce the § 144 cleansing consent (Jordan and the outside director as disinterested directors; Sam recuses). If no, produce the memo explaining why.
4. **Repurchase-and-reissuance analysis.** Chapter 08 says this is not viable once FMV has moved. Confirm and document the rationale.
5. **Disclosure treatment.** Draft the schedule-of-exceptions entry for the Series-A SPA.

#### For Founder C (Riley) — defective PIIA

Produce:

1. **Retroactive PIIA execution.** A current-form PIIA (drawing on exercise 03's template) with present-assignment language, DTSA notice, complete Prior Inventions schedule, and Cal. Lab. Code § 2870 carveout plus § 2872 written notification. The executed document is dated as of today with a "made effective as of" recital tied to Riley's actual start date. Do **not** backdate the signature.
2. **Parallel express IP assignment.** A stand-alone express assignment covering all IP Riley contributed from her start date through the retroactive PIIA execution date, to close any gap that a court might find the retroactive PIIA does not cover. Chapter 08 recommends this belt-and-suspenders approach.
3. **Reconciliation with Riley's Prior Inventions schedule.** Any pre-employment IP Riley claims as prior work should be listed; anything she is now assigning should be explicitly assigned (not carved out).
4. **Disclosure treatment.** Draft the schedule-of-exceptions entry.

#### For Founder D (Casey) — the four-defect founder

Produce:

1. **Retroactive SPA.** A current-form SPA (drawing on exercise 02's template) with:
   - Vesting schedule backfilled to run from Casey's original grant date (24 months into the vesting) — meaning some fraction of Casey's shares are already vested, and the corporation's repurchase right applies only to the currently-unvested portion. Show the vesting math.
   - The repurchase right at cost, ROFR, transfer restrictions, and standard reps.
   - Casey's acknowledgment that this SPA is executed retroactively and reflects the parties' intent from the original grant date.
   - Reference to the board consent that ratifies the retroactive execution.
2. **83(b) analysis.** Chapter 08 walks Casey's situation: the shares were issued at the board consent (transfer date passed), so the 30-day 83(b) window closed long ago. The corporation is in the same missed-83(b) position as Sam. Document why repurchase-and-reissuance is not viable (FMV has moved), and produce the disclosure treatment.
3. **Retroactive PIIA.** Current-form PIIA + parallel express IP assignment covering Casey's contributions from her original employee start date to date. Same "made effective as of" recital approach as Riley.
4. **Updated employment agreement.** A current-form employment agreement replacing the outdated offer letter, cross-referencing the new SPA and PIIA.
5. **Disclosure treatment.** Draft the schedule-of-exceptions entries.

### Part D — Comprehensive ratifying board consent

Author a single comprehensive board consent that:

1. Ratifies the retroactive execution of every document listed above.
2. Cleanses each § 144 conflict — each affected founder recuses from their own ratification item.
3. Authorises the tax-gross-up (if you adopted that path for Sam) and any other compensation adjustments.
4. Ratifies historical actions the retroactive documents cover (Casey's month-12 grant; Riley's employment onboarding).
5. Acknowledges the disclosure treatments on the Series-A schedule of exceptions.
6. Records the corporation's adoption of the go-forward prevention discipline (Part F).

### Part E — Founder Documentation State memo

Chapter 08 identifies the "Founder Documentation State" memo as the deliverable an incoming COO / GC produces in the first 30 days. Author it. It should:

- Summarise the diagnostic (Part A) in one paragraph per founder.
- Reference the personnel matrix (Part B).
- Present the cleanup plan (Part C) with owners and target dates.
- Reference the comprehensive board consent (Part D).
- Identify which items are curable, which are disclosable, and which the Series-A lead investor will require additional disclosure or negotiation on.
- Cross-reference the mod-101 entity-side "State of the Corporate Record" memo that a companion diagnostic would produce.

The audience is the CEO and (via the CEO) the board. The tone is diagnostic and prescriptive, not accusatory.

### Part F — Prevention discipline

Author a written prevention discipline the corporation adopts going forward, per chapter 08's "Prevention discipline going forward" section:

1. The 83(b) tracker (referencing exercise 02's template) with the "no receipt, no ledger entry" rule.
2. PIIA-before-access hygiene (referencing exercise 04's trade-secret baseline).
3. § 144 cleansing on every founder-scale grant, with a compensation-committee formation timeline (chapter 05 / mod-105 owns comp-committee depth).
4. Annual template review by counsel.
5. Personnel matrix as a living document reviewed at every board meeting.

### Part G — Series-A schedule of exceptions

Consolidate the disclosure treatments from Parts C into a draft schedule-of-exceptions section that will attach to the Series-A SPA. Each entry:

- Identifies the defect.
- Identifies the cure (or partial cure).
- Identifies any residual exposure.
- Is written for the lead investor's counsel — clear, factual, non-defensive.

## Starter guidance

- Chapter 08's "concrete example: the four-founder mess" is the model for this exercise. Reread it before drafting.
- **Do not backdate signatures.** Chapter 08 is explicit: retroactive execution with a "made effective as of" recital is defensible; backdated signatures are not. All retroactive documents are dated today, with an effective date tied to a real historical event.
- The missed 83(b) is not curable once FMV has moved. Do not pretend otherwise. The options are amended returns, tax gross-up (with § 144 cleansing), or disclose-and-accept.
- Casey's retroactive SPA is a real-world negotiation: Casey has to agree to have vesting applied to shares that (in the absence of an SPA) she legally owned outright. Chapter 08 notes the alternative is that the corporation acknowledges Casey is fully-vested with no repurchase right — which the lead investor will not accept. Casey's incentive to sign is that the corporation will not close Series-A without the fix.
- Every retroactive document requires a matching board consent. Chapter 08 says a single comprehensive consent is efficient at cleanup time.
- The schedule of exceptions is not a place to be defensive. Chapter 08 says diligence counsel accepts honest disclosure; they do not accept concealment.
- The mod-101 entity-side diagnostic is a companion, not part of this exercise. Cross-reference it, do not duplicate it.
- Reference the `<!-- needs-research -->` markers in earlier chapters (IRC § 1202 post-OBBBA, DGCL § 144 post-SB 313) — do not fabricate current-state numbers.

## Deliverables

- `founder-diagnostic-per-founder.md` — Part A.
- `personnel-matrix.md` (or `.csv`) — Part B.
- `retroactive-cleanup-founder-b-sam.md` — Part C, Founder B package.
- `retroactive-cleanup-founder-c-riley.md` — Part C, Founder C package.
- `retroactive-cleanup-founder-d-casey.md` — Part C, Founder D package.
- `comprehensive-ratifying-board-consent.md` — Part D.
- `founder-documentation-state-memo.md` — Part E.
- `prevention-discipline.md` — Part F.
- `series-a-schedule-of-exceptions.md` — Part G.

## Acceptance criteria

The package is acceptable if:

1. Each founder is correctly diagnosed against chapter 08's four defects.
2. Sam's missed-83(b) treatment does not falsely claim a filing-side cure. The tax-exposure model shows the arithmetic. The gross-up decision (yes / no) is defended.
3. Riley's retroactive PIIA uses present-assignment language ("hereby assigns"), includes the DTSA notice, and includes Cal. Lab. Code § 2870 carveout + § 2872 notice.
4. Riley's parallel express IP assignment is executed as a separate document to close the pre-execution-date gap.
5. Casey's retroactive SPA backfills the vesting schedule from her original grant date and reflects the currently-vested vs. currently-unvested split arithmetically.
6. Casey's retroactive PIIA + express IP assignment covers her contributions from her employee start date forward.
7. **All retroactive documents are dated today with "made effective as of" recitals.** No backdated signatures.
8. The comprehensive board consent ratifies every retroactive execution, cleanses each § 144 conflict, and records the disclosure treatments.
9. The Founder Documentation State memo is diagnostic and prescriptive, not accusatory.
10. The prevention discipline is operational (named owners, defined cadence) rather than aspirational.
11. The schedule of exceptions is honest and non-defensive, and each entry states the defect, the cure, and any residual exposure.
12. Statutory citations (17 U.S.C. § 101, Treas. Reg. § 1.83-2, IRC § 83, DGCL § 144, Cal. Lab. Code §§ 2870 / 2872, 18 U.S.C. § 1833) are correct.
