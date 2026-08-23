# Exercise 03 — Initial board consent & officer-appointment drill

> Estimated time: **~2 hours** · Related chapter: [02 — Stand up the entity](../02-stand-up-the-entity.md)

## Problem statement

Your Delaware C-Corporation has been formed. The incorporator has filed the charter, adopted the bylaws, and appointed the initial directors. Those directors now need to sign the **Initial Board Consent** — the single document that "turns on" the corporation's operating machinery — plus produce every ancillary document the consent references.

This drill produces the complete Day-0 board-side package.

## Fact pattern

Use fact pattern A from exercise 01 (or your own equivalent):

- Delaware C-Corporation, formed today.
- Three co-founders: Alice, Bob, and Carol. All three are initial directors and will serve as CEO, CTO, and COO respectively.
- Authorized shares: 10,000,000 common at $0.0001 par. (Adjust to match what you filed in exercise 02.)
- Planned initial common issuances: 3,000,000 shares to each founder at $0.0001 per share, paid in cash and in exchange for a contribution of pre-formation IP under a separate IP assignment.
- The corporation will adopt an equity incentive plan with a share reserve equal to 15% of the post-issuance fully-diluted capitalisation.
- Fiscal year: calendar year (December 31).
- Bank: any commercial bank of your choice; authorised signatories will be the CEO and the CFO (once appointed).
- The initial board is the three founders. The corporation is not yet ready to designate a lead independent director.

## Requirements

Produce the following documents, dated the same day:

### 1. Initial Board Consent (written consent under DGCL § 141(f))

The consent must cover, at minimum:

- **Ratification of the incorporator's actions**, including adoption of the charter and bylaws.
- **Election / confirmation of the initial officers** — CEO, President (if separate), Secretary, Treasurer, CTO, COO, CFO (if appointed). For each: name, title, and the authority delegated.
- **Fiscal year designation** — December 31.
- **Corporate seal** — adoption or waiver.
- **Corporate bank account** — authorisation to open an account at a specified bank, with named authorised signatories and signing thresholds.
- **Equity incentive plan** — adoption, share reserve, and reservation of shares for issuance under the plan. Include the exhibit reference to the plan document.
- **Form of Stock Purchase Agreement** — approval of the form to be used for founder issuances (and later restricted-stock hires), attached as an exhibit.
- **Founders' initial stock issuances** — approval of each founder's issuance: named founder, class of stock (common), share count, purchase price per share, total consideration, form of consideration (cash and IP), vesting schedule, cliff, and repurchase right. Approval of the IP assignment agreement for each founder.
- **Form of Indemnification Agreement** — approval, attached as an exhibit, with authorisation to enter into an agreement with each director and officer.
- **D&O insurance** — authorisation to bind an initial D&O policy on stated coverage limits.
- **Engagement of counsel and advisors** — authorisation to engage outside counsel and, if applicable, an accounting firm.
- **EIN application and state registrations** — authorisation for the officers to file Form SS-4, register the corporation in the states of operation, and take related actions.
- **Delegation of authority** — a general delegation permitting the officers to take all further actions necessary or advisable to carry out the resolutions.

### 2. Ancillary documents referenced by the consent

- **Equity Incentive Plan** — the plan document (a Cooley / Wilson Sonsini / Orrick model 2020 Stock Plan is a common starting point; use one and cite it).
- **Form of Stock Purchase Agreement** — used for the founder issuances, with vesting, cliff, and repurchase right filled in.
- **Form of Indemnification Agreement** — one form, to be executed with each director and officer.

### 3. Initial Stockholder Consent (written consent under DGCL § 228)

Signed by the founders as the initial stockholders, immediately after they receive their shares:

- Ratification of the board's actions to date.
- **Stockholder approval of the equity incentive plan** for IRC § 422 ISO purposes (see chapter 06 for why this matters).
- Any additional resolutions the board consent contemplated for stockholder approval (e.g., an increase to authorized shares if the initial charter's authorization is insufficient — usually not needed on formation day if the charter was filed correctly).

### 4. Sequence-of-execution memo

A short memo describing the *order* in which the documents must be signed on formation day, and why. Missteps here — signing a stockholder consent before the founders are stockholders, signing a board consent that references an unattached exhibit — are common self-inflicted defects.

## Starter guidance

- The Initial Board Consent is typically 6–12 pages including exhibits by reference. Each resolution should be self-contained ("RESOLVED, that ...") and cite the specific document or dollar amount it authorises.
- Every founder issuance is a separate resolution (or a table within a single resolution) that identifies the founder, the share count, the price, the consideration, and the vesting. Vagueness here is exactly what creates the "stock issued without board approval" defect in chapter 06.
- The equity incentive plan is a lengthy document; you do not need to draft it from scratch. Select a model plan (Cooley GO, Wilson Sonsini "Term Sheet Generator" / model plan, Orrick Start-Up Forms Library, or the NVCA model equity documents suite) and cite the source. Where you would customise the model plan for this corporation (share reserve, evergreen provision, ISO / NSO / RSU authorisation), document the customisation.
- The Indemnification Agreement should reference DGCL § 145 and cover both indemnification and advancement of expenses.
- Confirm every director signs the board consent (DGCL § 141(f) requires unanimity for board written consents absent a bylaw provision otherwise).

## Deliverables

- `initial-board-consent.md` (or `.docx`, `.pdf`) — the signed consent, with all exhibits attached or referenced by exhibit number.
- `equity-incentive-plan.md` — the plan document, with source cited if using a model.
- `form-stock-purchase-agreement.md` — the SPA form, filled in for the specific founder issuances.
- `form-indemnification-agreement.md` — the indemnification agreement form.
- `initial-stockholder-consent.md` — the stockholder consent.
- `sequence-of-execution-memo.md` — the ordering memo.

## Acceptance criteria

The package is acceptable if:

1. Every material formation-day corporate action is authorised by the Initial Board Consent — nothing is left to "implied" authority.
2. Every founder issuance is specifically authorised, with all economic terms named.
3. The equity incentive plan is both board-adopted (by the board consent) *and* stockholder-approved (by the stockholder consent) within the § 422(b)(1) window. The stockholder consent is dated on or after the board consent adopting the plan.
4. Statute citations are correct (DGCL § 141(f), DGCL § 228, DGCL § 145, DGCL § 152, IRC § 422(b)(1)).
5. Exhibits referenced in the consent actually exist and are attached.
6. The sequence-of-execution memo would let a new corporate-secretary hire execute the package without errors.
