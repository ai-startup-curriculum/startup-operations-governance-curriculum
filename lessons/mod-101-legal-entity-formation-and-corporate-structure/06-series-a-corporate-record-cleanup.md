# 6. The Series-A "corporate-record-in-shambles" diagnostic and cleanup

> Almost every incoming COO or GC inherits a corporate record that would fail Series-A diligence today. This chapter is the diagnostic and the cleanup.

## Motivation

The pattern is consistent: a startup founded 12–24 months ago, no corporate secretary, formation kit from Clerky or Stripe Atlas, one part-time counsel, a Carta account with a cap table that mostly matches reality, and — under the hood — a set of governance defects that a first-year associate at Series-A counsel will surface in the first pass of diligence. The COO / GC / CFO who joins at Series-A is expected to (a) find every defect, (b) prescribe the cleanup, and (c) get the record to "financeable" before the term sheet's closing condition on "clean corporate records" locks in.

This chapter is the diagnostic checklist and the cleanup playbook.

## The diagnostic — the eight recurring defects

Almost every messy corporate record contains some subset of these. Assume all eight are present until proven otherwise.

### 1. Missing board consents / minutes

**Symptom:** the minute book has the initial formation consent and nothing since. Founders have been running the company; officers have been signing contracts; the board has not been holding meetings or documenting decisions.

**Why it matters:** any material corporate action that should have been board-approved (equity grants, financings, key contracts, officer changes, adoption of policies) is technically unauthorised. In a diligence context, Series-A counsel will insist on ratification and, in some cases, re-execution.

**Diagnostic questions:** how many equity grants have been made since formation? How many financings (SAFEs, notes, warrants)? Any bank facility, real-estate lease, or contract with a "board approval" execution requirement? Any officer changes since formation? Do minutes / consents exist for each?

**Fix:** conduct a full-year (or full-formation-to-present) board consent in writing that (i) ratifies all prior actions, (ii) explicitly approves every equity grant and every financing at the terms actually executed, and (iii) is signed by every director. Where a director has changed, the consent may need to be executed by the current board with a specific ratification-of-prior-actions resolution and, where possible, corroborating documentation.

### 2. Stock plan not adopted (or not stockholder-approved)

**Symptom:** options were granted to employees before the corporation adopted an equity incentive plan; or the plan was adopted by the board but never approved by stockholders; or the plan's share reserve is less than the shares actually granted.

**Why it matters:** IRC § 422(b)(1) requires stockholder approval of an incentive stock option plan within 12 months before or after board adoption for ISOs granted under the plan to qualify as § 422 ISOs. A grant made before valid plan adoption is not a § 422 ISO and typically becomes an NSO — with materially different tax mechanics for the employee. Grants in excess of the plan's authorised share reserve are, in effect, ungranted; the corporation has no authority to issue those shares under the plan. SEC Rule 701, the federal exemption from securities registration that covers most compensatory issuances by private companies, also requires a written compensatory benefit plan.

**Fix:** if the plan was never validly adopted, adopt it now via board consent and stockholder consent, and re-issue the affected grants with new grant dates (with the tax-and-vesting consequences that entails; often, employees accept the re-issuance because the alternative is that their "options" were never valid). If the plan was validly adopted but the share reserve is exceeded, increase the reserve by board and stockholder consent (a charter amendment may be required if the reserve consumes authorised shares that need to be increased).

### 3. Stock issued without board approval

**Symptom:** the share ledger (or Carta) shows an issuance for which there is no corresponding board consent authorising the issuance.

**Why it matters:** DGCL § 152 requires the board (or a duly-authorised committee) to determine the consideration for and authorise the issuance of shares. Shares issued without valid board authorisation may be voidable.

**Fix:** ratify each unauthorised issuance in a comprehensive board consent that (i) recites the issuance, (ii) approves the consideration received, and (iii) ratifies the issuance. Where the issuance was to an insider, additional care is required to comply with DGCL § 144 (interested-director transactions) — see the founder-conflict discussion in [mod-102](../mod-102-founding-team-legal-architecture/).

### 4. Missing or defective 83(b) elections

**Symptom:** a founder or early employee who received restricted stock cannot produce a signed and mailed § 83(b) election with the certified-mail receipt.

**Why it matters:** the § 83(b) 30-day deadline is absolute (Treas. Reg. § 1.83-2(b)). A missed § 83(b) turns each vesting event into an ordinary-income tax event, calculated at the then-current fair-market value. A founder with unvested stock and a missed 83(b) can face an ordinary-income tax bill on each vesting tranche — often on illiquid stock. There is no cure at the tax-authority level. The corporation cannot fix a missed 83(b) after the fact.

**Fix:** identify every founder and every restricted-stock recipient. For each, obtain and archive their signed 83(b) with proof of timely mailing. Where the election is missing and the 30-day window has closed, escalate to tax counsel. Options in practice include: (a) accepting the tax consequence and modelling it; (b) if the vesting is early enough, a possible corporate-share-repurchase-and-re-issuance under a new grant date (a substance-over-form structure that tax counsel should own); and (c) disclosing the defect on the Series-A schedule of exceptions with a specific representation carve-out.

### 5. Missing founder Stock Purchase Agreements

**Symptom:** a founder is shown on the cap table as holding shares, but there is no executed Stock Purchase Agreement, no evidence of consideration paid, and no vesting schedule of record.

**Why it matters:** without an SPA and a repurchase right, "vesting" is a fiction — the corporation has no legal basis to repurchase unvested shares on separation. A founder who leaves without a repurchase right walks away with 100% of their originally-issued shares, no matter how little time they served. This is the "dead-equity" pattern that mod-102 addresses at depth.

**Fix:** obtain an executed SPA from every founder with a documented vesting schedule and repurchase right — even retroactively — as a condition of Series-A closing. In some cases, this requires the founder to accept new vesting terms; the alternative is the deal does not close.

### 6. Stale registered agent

**Symptom:** the Delaware registered agent on file is a founder's personal address, a former counsel's firm, or a commercial agent whose invoices have gone unpaid.

**Why it matters:** service of process from a lawsuit, a subpoena, or a state notice goes to the stale address and is not forwarded. A default judgment can be entered against the corporation without its knowledge. Loss of good standing follows unpaid franchise-tax invoices.

**Fix:** immediately engage or reactivate a commercial registered agent (CSC, CT, Cogency, InCorp — see [chapter 03](./03-corporate-record-and-compliance-calendar.md)) and file a change of registered agent with the Delaware Division of Corporations. Confirm the same for every state of qualification.

### 7. Missing or unfiled franchise tax / annual reports

**Symptom:** Delaware's franchise-tax dashboard shows overdue balances; California's Statement of Information shows a delinquency; the corporation is in "Not in Good Standing" or "Voided" status in one or more states.

**Why it matters:** Delaware charges penalties and interest for late franchise-tax payments, and a corporation whose franchise tax is unpaid for two consecutive years is administratively "voided" — a status that requires a formal revival to close a financing. Foreign-qualification states impose their own penalties and can suspend the corporation's authority to do business.

**Fix:** pay all delinquent Delaware franchise tax with penalties and interest; file every delinquent annual report; order fresh Certificates of Good Standing from Delaware and every qualification state; add every filing to the compliance calendar with owners and reminders.

### 8. Cap table that does not reconcile to the share ledger

**Symptom:** the Carta cap table shows 8,000,000 shares issued; the share ledger in the minute book shows 7,850,000; the sum of executed Stock Purchase Agreements shows 8,150,000. Nobody knows which number is right.

**Why it matters:** ownership is a legal question, not a database question. In a financing, the pre-money capitalisation is a term of the transaction; if the number cannot be defended against the underlying documents, the transaction stalls.

**Fix:** treat the underlying legal documents (executed SPAs, board consents authorising each issuance) as the source of truth. Reconcile the share ledger to those documents. Reconcile Carta (or the equivalent tool) to the share ledger. Where a discrepancy cannot be resolved, ratify or void the affected issuances through a comprehensive board and stockholder consent. This is often the single most time-consuming cleanup task.

## The cleanup playbook — the order to execute

Cleanup is done in a specific order, because later fixes depend on earlier ones.

1. **Reconstruct the cap table and share ledger from underlying documents.** Every issuance traced to its board consent and its SPA. Every gap flagged.
2. **Reactivate the registered agent and file every overdue franchise-tax / annual-report filing.** Get to good standing before doing anything else that requires the corporation to be in good standing.
3. **Adopt (or ratify) the equity incentive plan with valid stockholder approval.** Confirm the share reserve is sufficient for grants made to date; if not, increase the reserve and, if needed, amend the charter to increase authorised shares.
4. **Ratify every historic equity grant** — approve each grant retroactively via a comprehensive board consent that identifies each grantee, grant date, share count, exercise price, and vesting schedule.
5. **Retrieve every 83(b) election** and archive with certified-mail proof. Escalate the missing ones to tax counsel.
6. **Execute or re-execute every missing founder SPA** with documented vesting and repurchase right.
7. **Author a comprehensive omnibus board consent and stockholder consent** covering all ratifications. Attach the reconstructed cap table, share ledger, and grant schedules as exhibits.
8. **Obtain fresh Certificates of Good Standing** from Delaware and every state of qualification.
9. **Refresh the compliance calendar** — every future filing has an owner, a two-week advance reminder, and rollover into the following year.
10. **Draft the Series-A "schedule of exceptions"** honestly. Cleanup does not always retire every defect; disclosure is the professional handling of what remains.

## The COO / GC's first-30-days deliverable

An incoming COO or GC hired at seed / Series-A frequently produces a "State of the Corporate Record" memo in the first 30 days. It contains:

- **Findings** — every defect against the eight-item diagnostic, with severity, likely diligence impact, and cost to cure.
- **Cleanup plan** — the ordered list above, with owners (usually external counsel plus the corporate secretary), estimated timeline (typically 30–90 days for a moderately messy record), and estimated cost (counsel fees, tax penalties, Delaware franchise-tax back-payments).
- **Prevention plan** — the compliance calendar going forward, the corporate-secretary discipline that will be maintained (board consents at every material action, minute-book indexing, 83(b) tracking for every restricted-stock recipient).
- **Board approval** — the plan itself is approved by the board via written consent so that the cleanup work is authorised and funded from the corporate account.

## Concrete example: the "our first employee's ISOs are not ISOs" finding

A Series-A candidate startup is preparing for diligence. Its first employee, hired 14 months ago, received a grant of 40,000 options with an exercise price of $0.05, labelled on the offer letter as "Incentive Stock Options (ISOs)." Review of the corporate record shows: the equity incentive plan was adopted by board consent on 2025-03-15; the plan was never approved by the stockholders. The employee has been exercising options as they vest, expecting ISO tax treatment.

- **Under IRC § 422(b)(1)**, the plan needed stockholder approval within 12 months before or after board adoption. Stockholder approval was never obtained; the 12-month window has closed. The grant is not a § 422 ISO. The exercises were NSO exercises, taxable as ordinary income at exercise.
- **Fix:** counsel obtains stockholder consent approving the plan now (which cures ISO eligibility for grants going forward), amends the outstanding grant to reflect its NSO status, and issues corrected tax reporting to the employee. The employee's incremental tax cost is quantified; the corporation makes them whole via a supplemental payment (or does not, per its severance / cleanup policy). The Series-A schedule of exceptions discloses the historical ISO/NSO reclassification. The lesson is put on the compliance calendar: for every subsequent stock-plan amendment or reserve increase, stockholder consent is obtained within the § 422 window.

## Summary

- The corporate-record-in-shambles pattern is nearly universal at Series-A. Assume the eight defects are present until proven otherwise.
- Cleanup runs in a specific order: reconstruct → reactivate → ratify plan → ratify grants → 83(b)s → founder SPAs → omnibus consent → good-standing certificates → compliance calendar → schedule of exceptions.
- Some defects (missed 83(b)s, in particular) cannot be fully cured; disclosure is the professional handling of what remains.
- The COO / GC's first-30-days deliverable is a "State of the Corporate Record" memo — findings, cleanup plan, prevention plan, board approval.
- Compliance is a discipline maintained forward, not a project run once. The [chapter 03](./03-corporate-record-and-compliance-calendar.md) calendar is the discipline.
