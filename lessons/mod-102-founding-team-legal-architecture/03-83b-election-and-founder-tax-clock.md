# 3. The 83(b) election and the founder tax clock

> A single piece of paper, a 30-day IRS deadline, and no cure. This is the highest-stakes item on the founder's formation checklist.

## Motivation

The IRC § 83(b) election is a routine one-page filing that starts the founder's long-term-capital-gains clock and prevents the § 83(a) default rule from producing an ordinary-income tax bill on every future vesting event. It is trivial to file, absolute in its 30-day deadline, and irreparable if missed. It is also — consistently, across every corporate-record cleanup — the *single most common* founder-side diligence defect at Series-A. This chapter treats it in isolation so that the mechanical detail is memorable.

The 83(b) election is not new material in this curriculum — [mod-101 chapter 02](../mod-101-legal-entity-formation-and-corporate-structure/02-stand-up-the-entity.md) introduces it as part of the formation package. This chapter goes deeper on the tax mechanics, the failure modes, the retroactive-cleanup options (limited), and the corporate discipline that keeps the failure rate at zero.

## The § 83 default rule and why founders need the election

**IRC § 83(a)** says: when property is transferred to a person in connection with the performance of services, the person recognises *ordinary income* equal to the fair market value of the property at the time it is no longer subject to a substantial risk of forfeiture, minus what they paid for it.

For unvested founder stock, "no longer subject to a substantial risk of forfeiture" is the vesting date. So under § 83(a), the founder recognises ordinary income at each vesting event, calculated against the (usually much higher) fair market value at *that* vesting date. In year one, the founder owes ordinary income tax on the FMV appreciation on 25% of their shares (the cliff tranche). In each subsequent month, the founder owes ordinary income tax on the FMV appreciation on the newly-vested slice.

The economics of this are catastrophic for a founder of a company that appreciates. Consider the founder who buys 4,000,000 shares of common stock for $400 (par) at formation, when FMV is essentially par. Two years later, the corporation raises a Series-A and the 409A valuation on common stock is $0.80 per share. Under § 83(a), the founder recognises ordinary income on each vesting tranche:

- On the 1-year cliff (1,000,000 shares vesting), ordinary income of ~1,000,000 × ($0.80 − $0.0001) ≈ $799,900. Federal + California ordinary rates can push that to over $400,000 in taxes owed, on illiquid stock.
- On each subsequent monthly vesting slice, the same calculation against the then-current 409A.

The founder cannot sell the stock to pay the tax (private company, no market, transfer restrictions). The tax is owed anyway. This is the founder-broke-by-vesting problem.

**IRC § 83(b)** solves it. Section 83(b) lets the founder elect to recognise the ordinary income now, at the *transfer date* rather than each vesting date. Since the transfer date is formation day, when the founder pays FMV (par) for stock worth roughly par, the ordinary income recognised at election is *zero* — or a small dollar amount if FMV slightly exceeds the purchase price. All future appreciation is capital gain, taxed only on sale, at long-term rates if held more than 12 months from the transfer date.

The 83(b) election is essentially a free option for a founder whose stock is issued at formation-day fair market value. The only reason not to file is: the stock actually is worth materially more than the founder paid for it on the transfer date, in which case the election locks in ordinary income today. Even then, filing is usually correct if the founder expects further appreciation, because it converts future gain from ordinary to capital.

## What "transfer" means, and when the 30-day clock starts

The election must be filed with the IRS "no later than 30 days after the date of the transfer of the property" (**Treas. Reg. § 1.83-2(b)**).

"Transfer" is the transfer of the stock to the founder. For a founder purchasing restricted stock under an SPA:

- The transfer date is the date the SPA is executed and the founder becomes the record owner of the stock (which is also the date the founder pays consideration).
- The transfer date is *not* the date the corporation was incorporated, or the date the SPA was drafted, or the date the founder signed some earlier term sheet.
- The transfer date is *not* the vesting-start date if that date is different from the SPA execution date.

The clock is calendar-day, not business-day, and includes the day of transfer. If the SPA is signed on November 3, the 30th day is December 3. Late = void. There is no equitable exception.

The IRS updated the § 83(b) filing procedures in 2024 to include IRS Form 15620 as a standardised form (in addition to the historically-used Rev. Proc. 2012-29 sample text). The 30-day deadline is unchanged. <!-- needs-research: confirm current IRS guidance and whether Form 15620 is now required vs. optional; historically Rev. Proc. 2012-29 sample language was accepted alongside firm-drafted variants. -->

## What the election contains

The election must include, at minimum (per Treas. Reg. § 1.83-2(e)):

1. The taxpayer's name, address, and taxpayer identification number.
2. A description of the property (share count, class, corporation name).
3. The date of the transfer and the taxable year for which the election is made.
4. The nature of the restrictions to which the property is subject (i.e., the vesting schedule).
5. The fair market value of the property at the time of transfer, determined without regard to any restrictions other than restrictions that by their terms will never lapse.
6. The amount paid for the property.
7. A statement that copies of the election have been furnished to persons as required by the regulations.

The Rev. Proc. 2012-29 sample language covers all of the above and has been the market-standard form for a decade. Any startup-formation counsel and any commercial incorporation service (Clerky, Stripe Atlas, Cooley GO, Orrick) provides an 83(b) form that satisfies the regulations. Use the counsel-provided form, or use Rev. Proc. 2012-29's template, or use IRS Form 15620 — the mechanics of the filing are the same; the substantive content matches the regulation's list.

## How to file: the 30-day mechanical checklist

The election has to be *received* by the IRS Service Center where the founder files their federal income tax return, within 30 days of the transfer. In practice, "received" is proven by USPS Certified Mail with Return Receipt Requested (or, historically, by delivery to an IRS Taxpayer Assistance Center with a stamped copy).

The mechanical checklist:

1. **Sign the election.** Two copies — one to mail to the IRS, one for the founder's records. (Some practices also mail a third copy to include with the founder's Form 1040 for the year, though for tax years after 2015 the requirement to attach a copy to the return was removed.)
2. **Identify the correct IRS Service Center address.** This is the address where the founder files their Form 1040. The IRS publishes the current list (search "Where to File Paper Tax Returns" on irs.gov). The address changes periodically; use the current-year list, not a stale one.
3. **Mail via USPS Certified Mail with Return Receipt Requested.** Alternatively, use a private delivery service on the IRS's approved list (FedEx, UPS overnight, DHL Express — see IRC § 7502(f) and IRS Notice 2016-30). Retain the tracking number and the return receipt.
4. **Provide a copy to the corporation.** The corporation archives it in the corporate record. Every founder's 83(b) filing (with the certified-mail receipt) is a mandatory item in the diligence package.
5. **Calendar the deadline.** The corporate secretary (or COO / GC) maintains a per-founder tracker: transfer date, 30-day deadline, filing date, certified-mail tracking number, return-receipt date, copy archived. Every restricted-stock recipient — founder, early employee, contractor — gets tracked.

An electronic-filing option via the IRS Individual Online Account has been discussed but is not universally available as of writing. <!-- needs-research: confirm whether the IRS has finalised an electronic filing option for § 83(b) elections and, if so, how to use it. As of 2024, paper Certified Mail remains the market-standard defensible method. -->

## The failure modes

Every failure mode below has been observed in Series-A diligence. Assume they exist until you prove they do not.

### The founder never filed

The founder signed the SPA, paid for the shares, and forgot the 83(b). Twelve months later, the corporation raises a priced round; the founder's tax advisor asks for the 83(b) copy; nobody has one; there was no filing.

**Consequence.** § 83(a) applies. The founder owes ordinary income tax on each past and future vesting event at the then-current FMV. If the corporation appreciated between formation and today, the tax bill on already-vested tranches is real and immediately owed (with interest and penalties for underpayment).

**"Cure."** There is no filing-side cure. Options: (a) accept the tax consequence and pay it (with amended returns); (b) if the failure was recent enough that the corporation is *still at formation-day valuation*, consider a formal repurchase of the stock and a re-issuance under a new SPA with a new 30-day 83(b) window — this is a substance-over-form structure that requires tax counsel and should be documented as a bona fide repurchase-and-reissuance, not a paper shuffle; (c) disclose the defect on the Series-A schedule of exceptions with a specific representation carveout.

### The founder filed late

The election was mailed on day 31 (or later). Late filings are void. There is no equitable-tolling doctrine that saves a founder who was travelling, sick, or unaware. Same consequence and same cure options as the never-filed case.

### The founder filed but has no proof

The election was mailed, but not by certified mail; no tracking, no return receipt. The IRS has no record of receipt (or claims it does not); the founder cannot prove timely filing.

**Consequence and cure.** Absent proof, the IRS position is likely to be that no valid election was filed. The § 83(a) default applies. This is why certified-mail-with-return-receipt is the discipline, not a nice-to-have.

### The election is defective on its face

The election was mailed timely but omits a required element from Treas. Reg. § 1.83-2(e) — the vesting-schedule description, the FMV, or the amount paid.

**Consequence and cure.** A defective election may be treated as invalid. Timely filing an *amended* election within the 30-day window is permitted; after the window closes, the amendment cannot cure a substantive defect. Use a template that captures all required elements.

### The election was filed but a copy was not preserved

The corporation cannot produce the founder's 83(b) copy in diligence. The founder claims to have filed but cannot produce the certified-mail receipt.

**Consequence and cure.** This is a records problem more than a tax problem. Ask the founder to request an IRS transcript for the year of filing; a valid election should appear as an attachment on the Form 1040 filed that year (for filings before the attachment-requirement removal) or as a stand-alone submission indexed against the taxpayer's account. The corporation's diligence position improves materially if it can produce *any* documentary evidence.

## The retroactive-cleanup options in detail

The two survivable positions when an 83(b) has been missed:

### Repurchase-and-reissuance under a new grant date

Available only if two conditions hold:

- The corporation is still at essentially formation-day valuation (no financing, no material FMV appreciation). Once FMV has moved materially, the reissuance creates ordinary income on the new grant.
- The transaction is structured as a bona fide repurchase and reissuance, not a paper amendment. Documentation includes (i) a board consent authorising the repurchase, (ii) actual cash consideration flowing from the corporation to the founder for the repurchased shares, (iii) a new SPA with a new grant date and a new vesting schedule (which resets the cliff), (iv) new cash consideration from the founder for the reissued shares, and (v) a new § 83(b) election filed within 30 days.

Tax counsel needs to own this analysis. IRS may challenge a repurchase-reissuance that looks like a paper shuffle rather than a genuine ownership reset. Do this with counsel input, not by copy-editing a template.

### Disclosure and modelling

If the repurchase-and-reissuance is not available, the corporation:

- Quantifies the tax exposure on the founder's already-vested and expected-to-vest tranches, at reasonable expected FMV trajectories.
- Discloses the missed 83(b) on the schedule of exceptions to the Series-A Stock Purchase Agreement.
- Considers whether the founder's compensation package is adjusted (bonus, additional grant, tax-gross-up) to make the founder whole for the incremental tax. This is a corporation-side policy decision; the lead investor will want to know about it.
- The founder amends prior-year returns to report the § 83(a) income already-recognised and pays the associated tax with interest.

None of this is a cure — the tax is owed. The point is to make the situation legible to the investor and defensible in the diligence conversation.

## Adjacent tax mechanics founders should know about

### Qualified Small Business Stock (QSBS) under IRC § 1202

Founder restricted stock in a C-corporation is often § 1202 QSBS. If the § 1202 requirements are met — the corporation is a domestic C-corp; the stock is acquired at original issuance in exchange for money, property, or services; the corporation's gross assets do not exceed the § 1202 cap at issuance; the corporation is engaged in a qualified trade or business; and the founder holds the stock for the required period — the founder can exclude a substantial portion (potentially 100%) of the gain on sale from federal tax, up to a per-issuer cap. <!-- needs-research: § 1202 was amended by the One Big Beautiful Bill Act (P.L. 119-XX, July 2025) — confirm the current gross-asset cap, per-issuer exclusion cap, and the tiered-holding-period rules (historically 5 years for the 100% exclusion) before quoting specific numbers. -->

The § 83(b) election starts the § 1202 holding-period clock at the transfer date (rather than at each vesting date). Missing the § 83(b) has the collateral effect of starting the § 1202 clock later for each unvested tranche. Filing timely is a QSBS-enabling act as well as a § 83(a) defence.

### Wash sales and § 1091

Not directly relevant at formation, but worth flagging: founders selling shares in a public-market context after IPO can create wash-sale issues that reset the § 1202 clock and the capital-gains clock. This lives in `startup-exit-curriculum` and the founder-post-IPO track; mention it here only to note that the holding clock started by § 83(b) is a real asset that the founder should not accidentally break.

### Alternative Minimum Tax on ISO exercises

Not applicable to restricted stock — ISOs are options, not restricted stock. Included here because founders who receive restricted stock at formation *and later* receive additional ISO grants may confuse the tax mechanics. § 83(b) is a restricted-stock instrument; the AMT-on-ISO-exercise question is a stock-option instrument (mod-105 material).

## Corporate discipline that keeps the failure rate at zero

The corporation — not the founder — should own the 83(b) tracking. The mechanic:

1. **Every restricted-stock issuance goes on the tracker on the day it is issued.** Founder name, share count, transfer date, 30-day deadline (calendared with a 7-day and a 2-day advance reminder), filing status, tracking number, receipt date, archive location.
2. **The corporate secretary (or COO / GC / outside counsel) confirms the founder has filed before the 30-day deadline elapses.** This is a checkable, on-paper confirmation with a copy in the corporate record.
3. **A "no 83(b) receipt, no share issuance to the ledger" hygiene** — do not mark the share issuance as complete in the corporate record until the founder has filed and produced the receipt.
4. **Every subsequent restricted-stock issuance** — a promoted employee upgraded to restricted stock, a late-joining co-founder, a new grant against a milestone — repeats the same tracking discipline. The failure rate is zero because the process is a checklist, not a memory.

## Concrete example: the correct formation-day 83(b) flow

Founder A signs the SPA on 2026-05-15, pays $400 for 4,000,000 shares, and receives the shares uncertificated. On the same day:

- The corporate secretary marks 2026-06-14 (30 days later) as the filing deadline on the tracker, with reminders on 2026-06-07 and 2026-06-12.
- Outside counsel provides Founder A with the 83(b) election form pre-populated with the required elements from Treas. Reg. § 1.83-2(e).
- Founder A signs three copies. One is mailed via USPS Certified Mail with Return Receipt Requested to the IRS Service Center where Founder A files their Form 1040. One is retained by Founder A. One is provided to the corporation for the corporate record.
- The USPS certified-mail tracking number and the anticipated receipt-return date are added to the tracker.
- The return receipt is received back from USPS and archived. The tracker is updated to "filed and confirmed."
- Founder A's tax advisor is informed and reports the election on Founder A's federal return (attached copy for pre-2015 rules; no attachment required for later years, but the advisor retains the copy).

Total elapsed time from SPA signing to closed 83(b) tracker: roughly 3–4 weeks. Cost: $0 beyond postage. Downside of skipping: potentially six-figure tax liability on illiquid stock.

## Summary

- § 83(a) taxes restricted stock as ordinary income at each vesting event against then-current FMV. § 83(b) lets the founder recognise the income (usually ~$0) up front and convert future appreciation to capital gain.
- The **30-day deadline is absolute** (Treas. Reg. § 1.83-2(b)). Late = void. No equitable cure.
- File via USPS Certified Mail with Return Receipt Requested (or an approved private-delivery service) to the IRS Service Center for the founder's home. Retain the receipt in the corporate record.
- Use the Rev. Proc. 2012-29 sample language, IRS Form 15620, or the counsel-provided form — all satisfy the regulation if the required elements are present.
- Retroactive cleanup options are narrow: repurchase-and-reissuance while still at formation-day valuation (tax-counsel work), or disclose-and-model. Neither is a cure.
- Corporation-side discipline (tracker, calendared reminders, "no receipt, no ledger entry" hygiene) is what gets the failure rate to zero. Do not rely on the founder to remember.
- The § 83(b) election also starts the § 1202 QSBS holding-period clock, which is one of the largest tax benefits available to a founder. Filing timely is a QSBS-enabling act.
