# 8. Founder-diligence failure teardown and retroactive cleanup

> Every incoming COO / GC inherits some subset of these founder-side defects. This chapter is the diagnostic and the retroactive-cleanup playbook.

## Motivation

[mod-101 chapter 06](../mod-101-legal-entity-formation-and-corporate-structure/06-series-a-corporate-record-cleanup.md) covers the *entity*-side of the corporate-record-in-shambles diagnostic — missing board consents, unadopted stock plans, stale registered agents, unreconciled cap tables. This chapter covers the *founder*-side twin: the defects specific to founder documentation that Series-A diligence will surface and that require retroactive cleanup before the round can close.

The four recurring founder-diligence defects are:

1. **Un-signed founder IP assignments** — fatal at Series-A.
2. **Un-filed § 83(b) elections** — creates permanent ordinary-income tax exposure on future vesting.
3. **Missing founder Stock Purchase Agreements** — creates a wild-cap on the cap table (no vesting, no repurchase right).
4. **Un-mutual founder equity treatment** — one founder took an ordinary-income tax hit the others avoided; often traces back to informal side arrangements.

Each is diagnostic-and-cleanup work. Some are fully curable; some are only disclosable. This chapter walks each in the order a triage should tackle them.

## The four defects, diagnosed and cured

### 1. Un-signed founder IP assignments (PIIA)

**Symptom.** A founder is listed on the cap table with material equity, has been actively contributing code and product design for months or years, and does not have a fully-executed PIIA on file. Variants: the PIIA was drafted but never signed; the PIIA was signed but the Prior Inventions schedule is blank; the PIIA was signed but does not contain present-assignment language (uses "agrees to assign" instead of "hereby assigns"); the PIIA does not include a DTSA whistleblower-immunity notice ([chapter 05](./05-dtsa-whistleblower-and-trade-secret-baseline.md)).

**Why fatal.** Without an executed PIIA with present-assignment language, the corporation's ownership of the founder's contributions is contestable. The corporation may have a work-made-for-hire argument under 17 U.S.C. § 101 for copyrightable subject matter created after the founder became an employee, and a "hired to invent" or "shop right" argument for patents, but these are weaker positions than a signed assignment. For pre-employment work (the founder's contributions before the corporation was formed or before the founder became a W-2 employee), the corporation may have no ownership at all without an express assignment.

At Series-A, the lead investor requires clear title to the corporation's core IP as a fundamental representation. An un-executed founder PIIA is either a closing-condition failure or a schedule-of-exceptions disclosure the investor will not accept.

**Diagnostic questions.** For each founder: is there an executed PIIA? Is the Prior Inventions schedule complete? Does the assignment use present-assignment language? Does it include the DTSA notice? Is the state-law invention-assignment carveout included where the founder is or was based in a carveout state? Was the PIIA signed *before* the founder started contributing IP, or after?

**Cure.**

1. Draft (or adopt) a current-form PIIA template with present-assignment language, work-for-hire + assignment-backstop copyright drafting, Prior Inventions schedule, DTSA whistleblower notice, and applicable state-law carveouts.
2. Have each founder execute the current-form PIIA, backdated in *effective date* to a documented true date (the actual date of first IP contribution, or the corporation's formation date, whichever is applicable) with the *signature date* being the actual retroactive signature date. Do not falsify signature dates — retroactive execution with a "made effective as of" recital is defensible; back-dated signatures are not.
3. Have each founder complete the Prior Inventions schedule now, listing everything the founder claims as prior work. Reconcile the schedule against the SPA's consideration language (chapter 02) — pre-formation IP contributed as SPA consideration must be assigned separately (or via express assignment in the PIIA) rather than carved out on the Prior Inventions schedule.
4. Execute a parallel express IP Assignment Agreement covering (a) all pre-employment IP the founder contributed as SPA consideration and (b) any IP the founder created between the corporation's formation and the retroactive PIIA execution date, so that the assignment is unambiguous for any period that a court might find the PIIA does not cover.
5. Archive the executed PIIA and the express assignment in the corporate record; add the executed date and the effective date to the personnel matrix Series-A will read.
6. Disclose the retroactive execution honestly on the schedule of exceptions if a lead investor asks; the disclosure is "we executed retroactive PIIAs on [date] confirming founder assignments; the executed documents cover all founder contributions from [effective date] onward" and is acceptable when the retroactive PIIAs are genuine and complete.

### 2. Un-filed (or defective) § 83(b) elections

**Symptom.** A founder cannot produce a signed and mailed § 83(b) election with a certified-mail receipt within 30 days of the SPA execution date. Variants: never filed; filed late; filed but no proof of mailing; filed but a required element from Treas. Reg. § 1.83-2(e) is missing.

**Why fatal (or not).** As chapter 03 describes, a missed § 83(b) does not stop the corporation from raising a round, but it turns each future vesting event into a § 83(a) ordinary-income tax event at then-current FMV for the founder. The consequence is personal to the founder, but the corporation-side implication is real:

- The founder faces a potentially large personal tax liability that they may need corporation help to satisfy (a supplemental bonus, a loan, a tax gross-up).
- The corporation's compensation-expense reporting and the founder's W-2 reporting must reflect the ordinary income actually recognised at each vesting event. If historical reporting is wrong, the corporation has payroll-tax compliance exposure.
- The § 1202 QSBS holding clock for the founder's shares starts later than it would have with a timely 83(b), potentially reducing the founder's QSBS-eligible gain on eventual sale.
- The lead investor will require disclosure of the defect on the schedule of exceptions and may want to know what the corporation is doing about it.

**Cure options** (from most-desirable to least-desirable):

- **Repurchase-and-reissuance under a new grant date.** Available only if the corporation is still at essentially formation-day FMV (no financing, no material appreciation), and structured as a bona fide repurchase (cash consideration back to the founder for the repurchased shares) followed by a reissuance under a new SPA (fresh cash consideration from founder), a new vesting schedule with a new cliff, and a new timely-filed 83(b). This is tax-counsel work, not template work. IRS may challenge a paper-shuffle version.
- **Amended-return route.** The founder amends their prior-year returns to report the § 83(a) income already-recognised on any past vesting events at the correct FMVs, pays the associated tax with interest and penalties, and (going forward) reports § 83(a) income at each vesting event. The corporation adjusts payroll tax reporting to match. This is the honest and often the only viable path.
- **Tax gross-up.** The corporation, at its policy discretion, provides the founder with a supplemental bonus sized to cover the incremental tax cost of the missed 83(b). This is compensation expense to the corporation; it is a § 144 interested-officer transaction requiring cleansing; and it needs board approval on the record. Not universal; some corporations do not do gross-ups.
- **Disclose and accept.** The corporation and the founder accept the tax consequence, disclose the defect on the schedule of exceptions to the Series-A SPA, and move forward.

**Prevention going forward.** The 83(b) tracker (chapter 03) is the discipline. Every restricted-stock issuance — founder, promoted employee, late co-founder — goes on the tracker on the day of issuance with a calendared deadline. The failure rate goes to zero.

### 3. Missing founder Stock Purchase Agreements

**Symptom.** A founder is on the cap table with material equity, but there is no executed SPA on file. Variants: the founder received the shares via a board consent that referenced a "form of SPA" but no actual SPA was signed; the SPA was signed but has no vesting schedule; the SPA has a vesting schedule but no corporation repurchase right on unvested shares (the "no clawback" defect).

**Why fatal.** Without an SPA with a repurchase right, "vesting" is a fiction (chapter 02). A founder who has left — or who leaves at any point — walks away with the entire pre-departure share position. This is the *dead-equity founder* pattern (chapter 01).

Even for founders who are still with the corporation and have been all along, the missing-SPA defect is a serious diligence issue:

- The corporation cannot enforce vesting; the founder is a fully-vested owner of all issued shares as a matter of law.
- The corporation cannot enforce transfer restrictions; the founder could sell the shares to a third party without triggering ROFR.
- The corporation cannot enforce founder-specific covenants (representations, acknowledgments, § 83(b) confirmations).
- The lead investor will require an executed SPA with a documented vesting schedule and repurchase right as a closing condition.

**Cure.**

1. **For founders still with the corporation:** execute a current-form SPA now, with a vesting schedule that matches what the founder has effectively earned (backfilling the "vesting has been running from [formation date]" with actual dates), and a corporation repurchase right on the currently-unvested portion. The founder must agree to this; the alternative — legally speaking — is that the corporation acknowledges the founder is fully-vested with no repurchase right, which the lead investor will not accept.
2. **For founders who have already left:** contact the departed founder, disclose the situation honestly, and negotiate a retroactive agreement that either (i) confirms the departed founder's ownership of the vested portion under the vesting schedule that would have applied (with the corporation repurchasing the unvested portion at par), or (ii) purchases the disputed shares back from the departed founder at negotiated fair market value. Option (ii) is often the only viable path for a founder who has been out for a while and has no incentive to accept retroactive vesting.
3. **Board consent.** Any retroactive SPA or negotiated buyback is authorised by a board consent, cleansed under § 144 if the affected founder is or was a director, and archived in the corporate record.
4. **Disclosure.** The retroactive SPA execution (or the negotiated buyback) is disclosed on the schedule of exceptions to the Series-A SPA.

The cost of this cleanup is substantial — founders sometimes refuse; departed founders sometimes hold out for cash. The lesson is: execute the SPA on formation day, always. There is no cheap workaround at Series-A.

### 4. Un-mutual founder equity treatment

**Symptom.** One founder has restricted stock with a valid 83(b) filing, at par consideration; another founder has stock issued at a later date at a higher FMV, took an ordinary-income tax hit at issuance, or missed their 83(b) filing. Variants:

- A founder joined 4 months after formation, was granted stock at the higher post-formation FMV, and now has a materially different tax basis.
- A founder was originally granted options (not restricted stock), then "upgraded" to restricted stock via an ordinary-income-triggering conversion.
- A founder's shares were issued in two tranches (formation-day and a subsequent grant), each with their own SPA and 83(b) timeline, and one tranche was mishandled.
- A founder joined after a priced round, received restricted stock at a much higher post-money FMV, filed an 83(b), but now owes real ordinary income at issuance.

**Why it matters.** Each of these is *technically* not fatal — the corporation can be validly formed and the cap table can be defensible. But it creates a legibly-uneven founder story that Series-A diligence will read: why does founder B have a substantially different tax basis than founder A? Why did the corporation grant founder C stock at post-money value 3 months after the seed round rather than at formation? Why does founder D own options and not restricted stock?

Uneven treatment is fine when there is a *reason* — the founder joined later, the corporation had already appreciated, the founder joined post-seed at a real 409A. Uneven treatment without a documented reason looks like sloppy formation, and creates side questions ("did you consider whether the tax hit was actually necessary?") that consume diligence time.

**Cure and prevention.**

1. **Document the reasoning for the un-mutual treatment.** A memo in the corporate record explaining why founder B received the grant on the date and terms they did, referencing the 409A valuation in effect on that date, the timing of B's joining, and any other relevant circumstances.
2. **Consider whether to make founder B whole.** If the un-mutual treatment resulted from a mistake (missed 83(b), late grant that could have been earlier), the corporation may — as a policy matter — make B whole through a supplemental grant or bonus. Any such action is a § 144 cleansed transaction and needs board approval.
3. **Confirm the founder's tax reporting is correct.** A founder who took an ordinary-income hit at issuance should have reported it on the year's W-2 and paid the tax; the corporation's payroll tax reporting should match. Un-matched tax reporting is a compliance defect on the corporation side.
4. **Prevention.** Every founder-scale grant follows the same discipline: SPA on the grant date, 83(b) within 30 days, 409A valuation for any post-formation grant, board consent cleansed under § 144, corporate-record archive. Uniform treatment is achieved by uniform process, not by trying to retroactively equalise different-dated grants.

## The retroactive-cleanup playbook: order of operations

Founder-diligence cleanup runs in a specific order because later fixes depend on earlier ones. This complements the entity-side cleanup playbook in [mod-101 chapter 06](../mod-101-legal-entity-formation-and-corporate-structure/06-series-a-corporate-record-cleanup.md); in practice, the two run in parallel.

1. **Inventory every founder.** Current founders, departed founders, "promoted-to-founder" employees, late-joining co-founders. For each, build a file: SPA, 83(b) receipt, PIIA, offer letter, employment agreement, separation agreement (if departed), all subsequent side letters and amendments.
2. **Diagnose each of the four defects above** against each founder's file. Score severity (curable, disclosable, closing-condition-blocker).
3. **Reach out to departed founders.** These are the hardest conversations and have the longest lead time. Start early. Engage counsel.
4. **Draft the retroactive-cleanup documents.** Current-form PIIAs (with present-assignment language, DTSA notice, Prior Inventions schedule). Current-form SPAs with vesting and repurchase rights. Express IP assignments for pre-employment IP. § 83(b) amendment memoranda where relevant.
5. **Execute the cleanup.** Have every current founder sign the updated documents. Have departed founders sign what they will sign; negotiate buyback for what they will not.
6. **Board consent.** A comprehensive board consent authorises the retroactive execution, cleanses any § 144 conflicts, and ratifies the historical actions the retroactive documents cover.
7. **Corporate-record update.** File everything in the minute book with cross-references from the personnel matrix.
8. **Update the personnel matrix.** For every current and former founder, employee, and contractor: PIIA signed, date signed, effective date, DTSA notice present, 83(b) filed and receipt archived, SPA executed with vesting and repurchase, employment agreement executed. The matrix is what diligence counsel reads.
9. **Draft the schedule of exceptions honestly.** What could not be cured is disclosed. Diligence counsel accepts honest disclosure; they do not accept concealment.

The COO / GC hired at Series-A typically produces a "Founder Documentation State" memo in the first 30 days that runs this diagnostic and the cleanup plan. It sits alongside the mod-101 "State of the Corporate Record" memo.

## Concrete example: the four-founder mess

A four-founder AI-infrastructure startup is preparing for Series-A. The COO joined 5 months ago; the corporation was formed 26 months ago; there has been no corporate secretary; the founders used Clerky at formation and have not touched the corporate documents since. Findings:

- **Founder A (CEO):** SPA on file with 4/1 vesting and repurchase right. PIIA on file, present-assignment language, DTSA notice present. 83(b) filed and receipt archived. Employment agreement executed. Clean.
- **Founder B (CTO):** SPA on file with 4/1 vesting and repurchase right. PIIA on file, present-assignment language, DTSA notice present. **83(b) never filed** — B forgot; the certified-mail deadline lapsed 24 months ago. Employment agreement executed. Corporation-side ordinary-income exposure on all past and future vesting.
- **Founder C (VP Product, joined 4 months after formation):** SPA on file with 4/1 vesting and repurchase right. **PIIA is a 2015-vintage template** — no DTSA notice, no California § 2870 carveout (C is based in California), uses "agrees to assign" language rather than "hereby assigns." 83(b) filed and receipt archived. Employment agreement executed.
- **Founder D (Head of Growth, "promoted" to founder from an early-employee role at month 12):** No SPA on file — D received a grant of restricted stock on the promotion date, ratified by a board consent, but no SPA was ever signed. **PIIA never signed** — D signed an offer-letter-embedded confidentiality clause but no full PIIA. 83(b) never filed because there was no SPA to trigger the 30-day window. Employment agreement in the form of an outdated offer letter.

The cleanup plan:

1. **Inventory and diagnosis** complete (above).
2. **Founder A** — no action needed; confirm the file is complete.
3. **Founder B — missed 83(b)** — engage tax counsel to model the ordinary-income exposure. Corporation is now at a materially higher 409A than formation; repurchase-and-reissuance not viable (the reissuance would create fresh ordinary income). Options: (i) B amends prior-year returns; corporation adjusts payroll tax reporting; (ii) corporation considers a tax-gross-up bonus — § 144 cleansed by disinterested-director approval; (iii) disclose on schedule of exceptions.
4. **Founder C — 2015-template PIIA** — execute a current-form PIIA with present-assignment language, DTSA notice, California § 2870 carveout, complete Prior Inventions schedule. Execute a parallel express IP assignment covering all IP C contributed from her start date to the retroactive PIIA execution date. Archive.
5. **Founder D — missing SPA and PIIA** — execute a current-form SPA now, backfilling the vesting schedule to run from the original grant date, with the corporation's repurchase right on the currently-unvested portion. Execute a current-form PIIA with present-assignment language, DTSA notice, and complete Prior Inventions schedule. Execute an express IP assignment covering the period from D's employee start date through the retroactive PIIA execution date. Consult tax counsel on whether the newly-documented SPA vesting schedule triggers any 83(b) analysis (typically no — the shares were issued at issuance under the board consent even without a formal SPA, so the transfer date has passed and the 30-day window is long closed; the corporation is in the same missed-83(b) position as Founder B for the same reasons).
6. **Comprehensive board consent** — ratifies the retroactive execution of all documents, cleanses the § 144 conflicts (each founder recuses from their own item), and authorises the tax-gross-up if the corporation chooses that path.
7. **Corporate-record update, personnel matrix update.**
8. **Schedule of exceptions to the Series-A SPA** — discloses the missed 83(b)s (Founders B and D), the retroactively-executed PIIAs (Founders C and D), and the retroactively-executed SPA (Founder D). Each is a legible and cured (or disclosed) item.

Total cleanup time: approximately 6–10 weeks with counsel and tax-counsel time. Total cost: substantial legal fees, plus the tax-gross-up amounts if the corporation adopts that policy, plus the payroll-tax adjustments. Total avoidance-at-formation cost: essentially zero — every one of these defects was avoidable with a formation-day checklist.

## Prevention discipline going forward

The Series-A cleanup is a one-time (expensive) event. Post-Series-A, the corporation adopts a discipline that keeps the defect rate at zero:

- Every restricted-stock issuance goes on the 83(b) tracker on the day of issuance, with calendared deadlines and a "no receipt, no ledger entry" rule.
- Every new hire, contractor, and founder signs a current-form PIIA before starting work; no access to code or confidential information without a signed PIIA.
- Every founder-scale grant is a board-approved, § 144-cleansed, 409A-supported transaction with a documented SPA, vesting schedule, and 83(b).
- The personnel matrix is a living document owned by the corporate secretary and reviewed at every board meeting.
- Template PIIA, SPA, offer letter, and employment agreement are reviewed annually by counsel to catch drift.

The mod-104 (HR operations) chapter on onboarding is where this discipline lives operationally for non-founder employees. This chapter's ownership is: the founder-specific piece, and the retroactive-cleanup diagnostic that an incoming COO / GC will need in the first 30 days.

## Summary

- Every incoming COO / GC inherits some subset of four recurring founder-diligence defects: un-signed founder IP assignments, un-filed § 83(b) elections, missing founder SPAs, and un-mutual founder equity treatment.
- Un-signed founder IP assignments are curable via retroactive PIIA execution plus express IP assignment covering the pre-execution period; the executed retroactive documents are what diligence counsel reads.
- Un-filed § 83(b) elections have no filing-side cure; options are limited to repurchase-and-reissuance (only while at formation-day FMV), amended returns, tax gross-up, or disclose-and-accept.
- Missing founder SPAs are curable for current founders (execute retroactively with vesting and repurchase right) and typically require negotiated buyback for departed founders.
- Un-mutual founder equity treatment is often not-fatal but must be *documented* — the reasoning belongs in the corporate record.
- The retroactive-cleanup playbook runs in a specific order: inventory → diagnose → outreach to departed founders → draft → execute → board consent → update the record → schedule of exceptions.
- Prevention discipline going forward is what keeps the defect rate at zero: 83(b) tracker, PIIA-before-access hygiene, § 144 cleansing on every founder-scale grant, annual template review.
