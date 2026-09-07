# Exercise 02 — Founders' restricted stock and § 83(b) authoring

> Estimated time: **~4 hours** · Related chapters: [02 — Founders' restricted stock, vesting, and the repurchase right](../02-founders-restricted-stock-and-repurchase.md) · [03 — The § 83(b) election and the founder tax clock](../03-83b-election-and-founder-tax-clock.md)

## Problem statement

You continue the same three-founder scenario from exercise 01 (Alex Chen — CEO; Priya Rao — CTO; Marcus Hill — VP GTM). The founder agreement is drafted and the equity split is set. Formation day is next Monday. Your job is to author the **Stock Purchase Agreements** for each founder and the **§ 83(b) elections** each founder will file, and to stand up the **corporation's 83(b) tracker** so that no future issuance ever slips the 30-day window.

Assume the corporation is a Delaware C-corporation with 10,000,000 authorised common shares at $0.0001 par (you can adjust with a written justification if needed to accommodate the seed option pool or other headroom). Assume the founder agreement specifies the split you produced in exercise 01; if you did not do exercise 01, use 45 / 35 / 20 for Alex / Priya / Marcus. Assume Priya has 3 months of pre-formation full-time service on the project and Alex has 8 months of prior-employer part-time work on the underlying memo and prototype.

## Requirements

### Part A — Three Stock Purchase Agreements

Author a Stock Purchase Agreement for each founder. Each SPA must cover, at minimum:

1. **Parties, recitals, and effective date.**
2. **Purchase price and consideration.** Cash amount per share (par is the default; deviations require a written reason) and, where applicable, the description of pre-formation IP being contributed as additional consideration. Per chapter 02, do not use "services rendered." Reconcile any IP contribution with the PIIA's Prior Inventions schedule (which exercise 03 will produce) — call out that reconciliation explicitly in the SPA.
3. **Vesting schedule.** 4-year vesting, 1-year cliff, monthly thereafter is the default. If you propose prior-service credit for any founder (Priya's 3 months, Alex's 8 months, or otherwise), justify the credit on the record and state the vesting-start date explicitly.
4. **Repurchase right at cost on unvested shares.** Trigger (cessation of service, for any reason). Scope (all unvested shares). Price (original purchase price per share). Exercise window (e.g., 90 days from separation). Board-approval mechanic. Cross-reference the § 144 cleansing per [chapter 06](../06-founder-conflict-of-interest.md) if the departed founder was a director.
5. **Separation-trigger treatment.** Voluntary resignation, termination for cause (with a narrow definition), termination without cause (with any accelerated vesting — commit to a specific number of months), death or disability, and change-of-control acceleration (double-trigger; state the acceleration fraction; single-trigger is deferred to `startup-exit-curriculum` and should be explicitly noted as such).
6. **Right of first refusal (ROFR)** on transfers of vested shares, permitted-transferee carveouts (family, trusts), and the legend / book-entry notation.
7. **Standard founder representations** — legal capacity; no conflicting prior-employer obligation (cross-reference to the PIIA carveout schedule); no prior grant of rights in contributed IP; tax-advisor acknowledgment; accredited investor / knowledgeable purchaser rep under § 4(a)(2) / Regulation D.
8. **§ 83(b) acknowledgment** — the founder acknowledges the 30-day deadline, has been advised to consult tax counsel, and understands the corporation is not responsible for filing.

Each SPA should reference the initial board consent that will authorise the issuance ([mod-101 chapter 02](../../mod-101-legal-entity-formation-and-corporate-structure/02-stand-up-the-entity.md)) and confirm that the share ledger will reflect the issuance on formation day.

### Part B — Three § 83(b) elections

Author a § 83(b) election for each founder that satisfies **Treas. Reg. § 1.83-2(e)**. Each election must include:

1. Taxpayer name, address, and taxpayer identification number (use `[SSN]` as a placeholder — do not invent one).
2. Description of the property (share count, class, corporation name, jurisdiction of incorporation).
3. Date of transfer and taxable year for which the election is made.
4. Nature of the restrictions (the vesting schedule from the SPA — restate concisely).
5. Fair market value at time of transfer, ignoring lapse restrictions.
6. Amount paid for the property.
7. Statement that copies of the election have been furnished as required.

You may use IRS Form 15620, the Rev. Proc. 2012-29 sample language, or your own template — all satisfy the regulation if the required elements are present. Cite which template you used. See the `<!-- needs-research -->` marker in chapter 03 on the current Form 15620 status if you are drafting for production use.

### Part C — 30-day filing checklist (per founder)

Produce a per-founder filing checklist per chapter 03's "How to file" section:

1. Sign three copies.
2. Identify the correct IRS Service Center (use the founder's home state — cite where you looked it up on irs.gov "Where to File Paper Tax Returns").
3. Mail via USPS Certified Mail with Return Receipt Requested (or an IRC § 7502(f) / IRS Notice 2016-30 approved private delivery service — name the service and cite the approved-list source).
4. Provide a copy to the corporation for the corporate record.
5. Calendar the deadline with reminders (chapter 03 recommends 7-day and 2-day advance reminders).

### Part D — Corporation's 83(b) tracker

Author the corporation's ongoing 83(b) tracker as a table (spreadsheet, CSV, or Markdown table) with columns per chapter 03: recipient name, share count, transfer date, 30-day deadline, filing status, tracking number, receipt-return date, archive location, tracker-owner sign-off. Populate the tracker with the three founders' expected entries. Add a written policy paragraph describing:

- Who owns the tracker (corporate secretary / COO / GC).
- The "no receipt, no ledger entry" hygiene.
- The reminder cadence.
- The escalation path if a filing has not been confirmed within the reminder window.

### Part E — Cap-table snapshot on issuance day

Produce a one-page cap-table snapshot as of the moment of issuance:

- Each founder's share count, per-share price, aggregate consideration paid, and initial percentage of outstanding.
- Total shares outstanding, total shares authorised, and remaining authorised-but-unissued shares (with an explicit note reserving whatever share count you plan for the seed-stage option pool, or a written assumption if you defer the pool to a later grant).
- A one-paragraph note reconciling the cap table with the SPAs, the (forthcoming) initial board consent, and the § 152 consideration determination.

## Starter guidance

- Do **not** invent IRS forms, docket numbers, or § 1.83-2(e) required elements — reference Treas. Reg. § 1.83-2(e) and Rev. Proc. 2012-29 (the sample text has been publicly available since 2012).
- The Rev. Proc. 2012-29 sample text is public at https://www.irs.gov/pub/irs-drop/rp-12-29.pdf; cite it if you use it.
- "Cause" definitions should be narrow (fraud, willful misconduct, uncured material breach after written notice, felony conviction involving moral turpitude). "Failure to perform assigned duties" is not narrow.
- Prior-service credit that reaches back before formation must be documented — chapter 02 supports it "if defensible on the record." A written recital in the SPA is defensible; a hand-shake is not.
- Do not attempt to write single-trigger acceleration into the SPA — chapter 02 says the founder-market-standard baseline is double-trigger and single-trigger is deferred to `startup-exit-curriculum`. Explicitly note the deferral in your SPA.
- The corporation's repurchase right should be a *right*, not an obligation. Some SPAs also include a right (not obligation) to repurchase *vested* shares at fair market value on separation — chapter 02 covers this variant; explain your choice.
- Reference the initial board consent that authorises the issuance without drafting it yourself — the corporation-side authorisation lives in mod-101.
- Every fair-market-value assertion in the 83(b) elections should be $0.0001 unless you have a written reason to say otherwise.

## Deliverables

- `spa-founder-a-alex-chen.md`, `spa-founder-b-priya-rao.md`, `spa-founder-c-marcus-hill.md` — three executed-ready SPAs. Part A.
- `83b-election-alex-chen.md`, `83b-election-priya-rao.md`, `83b-election-marcus-hill.md` — three § 83(b) elections in filing-ready form. Part B.
- `83b-filing-checklist-per-founder.md` — filing checklists. Part C.
- `83b-tracker.md` (or `.csv`) — the corporation's ongoing tracker plus policy paragraph. Part D.
- `cap-table-snapshot-formation-day.md` — the one-page snapshot. Part E.
- `spa-design-choices-memo.md` — 1–2 page memo documenting every material choice you made (per-share price, vesting variants, acceleration fractions, "for cause" definition, ROFR scope, prior-service credit rationale).

## Acceptance criteria

The package is acceptable if:

1. Each SPA covers all eight clause categories in Part A and internally reconciles with the founder agreement produced in exercise 01 (or with the fallback 45 / 35 / 20 split).
2. Consideration is *real* — cash and/or contributed IP — not "services rendered." Payment mechanics (check, wire) are described.
3. Vesting is 4/1 default unless a written justification supports a variant. Prior-service credit is documented with a specific vesting-start date.
4. The repurchase right is drafted with trigger, scope, price, exercise window, and board mechanic.
5. Each § 83(b) election satisfies all seven Treas. Reg. § 1.83-2(e) required elements. Missing any element is a defect.
6. The filing checklist names the specific IRS Service Center for each founder's home state and cites where the list was found on irs.gov.
7. The tracker's "no receipt, no ledger entry" hygiene is stated explicitly. The owner is named.
8. The cap-table snapshot's math is arithmetically correct (share counts and percentages reconcile). The § 152 consideration determination is referenced.
9. Statutory citations (Treas. Reg. § 1.83-2, DGCL § 152, Rev. Proc. 2012-29) are correct.
10. No filing-related date is left as `[TBD]` — every deadline is populated relative to a stated formation date.
