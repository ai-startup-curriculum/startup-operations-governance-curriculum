# Exercise 07 — Change-of-control equity policy drill

> Estimated time: **~6 hours** · Related chapter: [07 — Change-of-control equity policy](../07-change-of-control-equity-policy.md)

## Problem statement

Breakwater Compute is a Delaware C-corp building a managed GPU-training platform. It is a Series-C corporation with ~400 employees (roughly 220 engineering, 50 research, 70 GTM, 40 G&A, 20 operations) and a last-round post-money of ~$1.9B. The company has an equity incentive plan ("the 2021 Plan") adopted at Series-A and amended twice; a 2023 ESPP with a quarterly offering period (offerings open on the first business day of January, April, July, October) and a 15% discount; executive employment agreements for the CEO, COO, CFO, CRO, GC, and three VPs; and an outstanding grant inventory of ~2,800 option grants and ~1,100 RSU grants across 400 current and ~140 former-but-still-vesting holders.

Last Thursday the CEO received an unsolicited expression of interest from Harbor Analytics, a publicly listed strategic competitor, suggesting an all-stock-plus-cash acquisition at a headline price in the $2.6–$3.1B range. The CEO and board chair have agreed to engage with Harbor through a 30-day exclusivity window, during which the CFO and GC must walk the comp committee through the current CoC equity policy, identify gaps that will become visible in diligence, and surface the amendments the comp committee should adopt *before* a term sheet is signed.

The current CoC posture Breakwater inherited is: (a) a plan-level default of **double-trigger** acceleration (CoC + involuntary termination without cause or resignation for good reason within 12 months); (b) a **single-trigger** CoC-acceleration provision in the hired-CEO's 2022 employment agreement (negotiated when the CEO joined from a public-company role); (c) a **modified-single-trigger** provision for the VP of AI Research (6-month post-close window during which the VP may resign for any reason and receive full acceleration); (d) three outstanding RSU grants issued in Q4 2024 whose grant agreements say "double-trigger acceleration applies subject to a reasonable period following the Change of Control" without defining "reasonable period"; and (e) an ESPP whose next offering period opens the first business day of the next calendar quarter — which, based on Harbor's indicated signing cadence, is likely to straddle signing.

Your role: you are the CFO (or an outside operating advisor engaged by the comp committee chair) working with the GC. Produce the audit, the gap list, the amendment package, the IRC § 280G analysis plan, the transaction-type-overlay analysis, and the board brief that the comp committee will walk the full board through at a special meeting scheduled 10 days from today.

## Requirements

### Part A — Audit the existing policy

Produce a written audit of Breakwater's current CoC equity policy. Cover:

1. **CoC trigger definitions in the 2021 Plan** — the plan-level definition of "Change of Control," the plan-level definition of "Cause" and "Good Reason," and any carve-outs (e.g., for internal reorganisations, going-public transactions, equity financings above a stated threshold). Note any ambiguity that an acquirer's counsel will flag.
2. **Double-trigger / single-trigger split by role** — produce a matrix: role → acceleration type (plan-default double-trigger, exec-agreement single-trigger, exec-agreement modified-single-trigger) → source document (plan vs. grant agreement vs. employment agreement). Cover the eight executives named in the problem statement plus the three ambiguous Q4 2024 RSU grants.
3. **ESPP-in-a-transaction treatment** — the current ESPP's language on offering periods that straddle a CoC: whether contributions continue, whether the offering is cut short with an early purchase date, whether the ESPP is terminated, and whether participants' accrued contributions are refunded.
4. **Exec-severance-agreement CoC-acceleration terms** — for each of the eight executives, the severance payable on CoC-plus-qualifying-termination (base × multiple, bonus treatment, COBRA period, equity acceleration), and the interaction with the plan-level acceleration provisions.
5. **IC-level CoC provisions** — the standard RSU and option grant-agreement language the plan administrator has been using since 2021, whether it has drifted (any version-control gaps in the grant-agreement templates), and any one-off grants with bespoke acceleration language outside the standard template.

Cross-reference `../04-executive-compensation-packages.md` for the composition of the exec packages and `../08-executive-severance-and-release.md` for the severance-mechanics piece.

### Part B — Identify the gaps

Produce a written gap list naming each specific gap, the evidence, and the risk if left unresolved. Cover at minimum:

1. **Single-trigger exposure that creates a § 280G problem** — which executives have single-trigger or modified-single-trigger acceleration that, when combined with cash severance and bonus, will plausibly exceed the 3× base-amount safe harbor under IRC § 280G.
2. **IC-level grants without clear acceleration language** — the three Q4 2024 RSU grants with the undefined "reasonable period" clause, plus any other grants where the acceleration mechanics are ambiguous (e.g., grants issued during the ~3-week window when the grant-agreement template was reverted to a prior version).
3. **ESPP period straddling signing** — the specific offering period in question, the number of participants, the aggregate accrued contributions, and the policy decision the comp committee needs to make (continue, early-purchase, terminate-and-refund) before the deal is announced.
4. **Outstanding RSUs without a defined double-trigger expiration** — the window (6 months? 12 months? 24 months?) within which an involuntary termination counts as the second trigger. Flag which grants have no such definition.
5. **Any other latent gap** the audit surfaced — e.g., former-employee grants still vesting under a post-termination exercise window, grants to board directors (if any) with non-standard acceleration, or international-employee grants where local-law treatment conflicts with the plan.

### Part C — Draft the policy update

Produce the amendment package the comp committee needs to adopt before a term sheet is signed. Cover:

1. **Plan-level amendments** — any amendments to the 2021 Plan's CoC provisions (e.g., defining "reasonable period," tightening the Good Reason definition, adding an ESPP-in-transaction protocol). Note which amendments require stockholder approval and which do not.
2. **Grant-level amendments** — the specific amendments to the three ambiguous Q4 2024 RSU grants and any other grants that need remediation. Include the mechanics for obtaining grantee consent where consent is required.
3. **Exec-agreement amendments** — whether any exec agreement needs to be amended (e.g., converting the hired-CEO's single-trigger to a modified-single-trigger, or adding a § 280G cutback / gross-up provision). Note the comp-committee-approval and stockholder-approval mechanics.
4. **Plan-level vs. grant-level vs. exec-agreement-level hierarchy** — a written statement of which document controls when they conflict (standard practice: the more employee-favorable term controls unless the plan explicitly overrides), and the specific conflict-resolution rules the amended policy will adopt.

### Part D — IRC § 280G exposure analysis

Produce the § 280G analysis plan. Cover:

1. **Named-exec exposure** — a per-exec table identifying each of the eight executives, their base amount (5-year W-2 average per IRC § 280G(b)(3)), their projected parachute payments (cash severance + bonus + equity acceleration value), and whether the projected parachute exceeds 3× base amount. Where equity-acceleration value is not yet knowable (deal price not final), flag the sensitivity range.
2. **IRC § 4999 excise-tax exposure** — the 20% excise tax exposure on the executive side and the lost-deduction exposure on the corporation side under IRC § 280G(a).
3. **Private-company shareholder-approval cleanse** — the workflow under IRC § 280G(b)(5)(A)(ii) and 26 C.F.R. § 1.280G-1 Q&A-6 and Q&A-7 for cleansing the parachute payments via a > 75% disinterested-shareholder vote. Cover: who votes (holders of outstanding voting stock, excluding the disqualified individuals and their related parties), what is disclosed (the material facts of all payments subject to the vote), the waiver mechanics (each affected exec must waive their right to the payment unless the vote passes), and the timing (the vote must occur before the CoC closes).
4. **Shareholder-vote timeline and 75%-threshold mechanics** — the specific calendar: when the waivers are signed, when the disclosure statement is finalised, when the vote is solicited, and when the vote must close relative to the expected signing / closing dates. Note the practical risk that any single large-block holder refusing to vote drops the vote below 75%.
5. **Alternative structures if the cleanse fails** — cutback provisions (reduce payments to 2.99× base amount), gross-up provisions (corporation pays the exec's excise tax), and best-of-net approaches (compare cutback vs. non-cutback and apply whichever leaves the exec better off).

### Part E — Transaction-type-overlay analysis

Produce a written analysis of how the CoC policy flows through under each of the three plausible deal structures Harbor has indicated. Cover:

1. **Stock-for-stock** — treatment of options and RSUs (assumption, substitution, or cash-out), tax treatment under IRC § 368 reorg rules, and the comp committee's policy decisions on whether to insist on assumption vs. cash-out of specific grants.
2. **Cash-and-stock (mixed consideration)** — allocation of consideration between cash and stock components across the grant inventory, and the comp committee's decision on whether vested-and-exercised holders are treated the same as unvested-but-accelerated holders.
3. **All-cash** — cash-out mechanics for options (spread value) and RSUs (full value), the escrow / holdback treatment of accelerated-but-unvested grants, and the comp committee's decision on whether to insist on continued vesting of a retention-pool subset even in an all-cash deal.

Cross-reference `startup-exit-curriculum` for the underlying transaction-execution mechanics (reorg tax treatment, escrow structures, assumption-vs-substitution choice). Do NOT re-derive the deal mechanics here — focus on the policy decisions the comp committee must make *before* signing. Cross-reference `startup-finance-fundraising-curriculum` where the capitalisation-table and liquidation-preference waterfall interacts with the CoC policy (e.g., preferred-stock participation changing the per-share consideration available to common and option holders).

### Part F — 1-page CoC-policy brief for the full board

Produce a 1-page (one-page, hard limit) brief the comp committee chair will walk the full board through at the special meeting. Cover:

- The current CoC posture (two bullets).
- The gaps the audit surfaced (three bullets, the most material).
- The amendments the comp committee is asking the board to approve or ratify (three to five bullets).
- The § 280G exposure summary (one bullet with the named execs at risk and the cleanse-vote plan).
- The transaction-type-overlay (one bullet).
- The two or three decisions the board specifically needs to make at this meeting (e.g., approve the plan amendment, authorise the § 280G cleanse-vote process, approve the ESPP-in-transaction protocol).

## Starter guidance

- Chapter 07 is the primary reference. The plan-level vs. grant-level vs. exec-agreement-level hierarchy and the double-trigger / single-trigger / modified-single-trigger taxonomy are developed there.
- Chapter 04 (executive compensation packages) is where the composition of exec packages is laid out; chapter 08 (executive severance and release) is where the severance mechanics live. Both are relevant to Part A and Part D.
- The § 280G cleanse workflow is a well-defined regulatory procedure under IRC § 280G(b)(5)(A)(ii) and 26 C.F.R. § 1.280G-1. Cite the specific regulatory sections (Q&A-6 "shareholder approval requirements"; Q&A-7 "adequate disclosure"). Do not paraphrase them from memory — if you are unsure of the exact mechanics, flag with `<!-- needs-research -->`.
- The three Q4 2024 RSU grants with the undefined "reasonable period" are a drafting defect that is going to be visible in diligence. Your job is not to assign blame — it is to produce the remediation.
- The ESPP-in-transaction decision is time-sensitive. If the offering period opens before signing and closes after signing, the comp committee is going to have to make a decision in the next 10 days — before the board meeting if practical.
- The transaction-type overlay (Part E) is a policy exercise, not a deal-mechanics exercise. The comp committee is deciding what Breakwater will insist on at the term-sheet stage, not re-deriving the tax treatment of a § 368 reorg. Keep the altitude high and cross-reference `startup-exit-curriculum`.
- The board brief (Part F) is one page. Not two pages with small font — one page. The comp committee chair's job is to make the decisions legible to a board that is simultaneously processing an unsolicited bid.

## Deliverables

- `coc-policy-audit.md` — Part A.
- `coc-policy-gap-list.md` — Part B.
- `coc-policy-amendment-package.md` — Part C.
- `280g-exposure-analysis.md` — Part D.
- `transaction-type-overlay.md` — Part E.
- `board-brief-coc-policy.md` — Part F (one page).

## Acceptance criteria

The package is acceptable if:

1. The audit (Part A) produces a role-by-role acceleration matrix covering all eight named executives and the three ambiguous Q4 2024 RSU grants, each with the source document named.
2. The gap list (Part B) names at least one specific exec with § 280G exposure, the specific three Q4 2024 RSU grants with the "reasonable period" defect, the specific ESPP offering period that straddles signing, and at least one additional latent gap the audit surfaced.
3. The amendment package (Part C) produces a specific, enumerable policy-update list — plan-level amendments, grant-level amendments, and exec-agreement amendments — with the approval mechanics (comp committee only, board, stockholder vote) named for each.
4. The § 280G analysis (Part D) names which executives are at risk of exceeding 3× base amount, cites IRC § 280G(b)(5)(A)(ii) and 26 C.F.R. § 1.280G-1 for the cleanse workflow, and lays out the 75%-threshold vote mechanics and the waiver timing. The IRC § 4999 excise-tax exposure is named explicitly.
5. The transaction-type overlay (Part E) covers all three deal structures (stock-for-stock, cash-and-stock, all-cash) and names the specific policy decisions the comp committee must make before signing — not the underlying deal mechanics, which are cross-referenced to `startup-exit-curriculum`.
6. The board brief (Part F) is one page and names two or three specific decisions the board is being asked to make at the special meeting.
7. Every regulatory citation uses the specific section (IRC § 280G, IRC § 280G(b)(5)(A)(ii), IRC § 4999, 26 C.F.R. § 1.280G-1 Q&A-6, Q&A-7) rather than a generic "under Section 280G" reference.
8. Nothing left as `[TBD]` or `[FILL IN]`.
