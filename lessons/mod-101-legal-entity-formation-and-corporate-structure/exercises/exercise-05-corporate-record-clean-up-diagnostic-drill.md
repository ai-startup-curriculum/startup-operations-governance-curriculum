# Exercise 05 — Corporate-record cleanup diagnostic drill

> Estimated time: **~3 hours** · Related chapter: [06 — The Series-A "corporate-record-in-shambles" diagnostic and cleanup](../06-series-a-corporate-record-cleanup.md)

## Problem statement

You are the incoming COO / GC at a startup that has just signed a Series-A term sheet contingent on "delivery of the corporate records in reasonable condition" and "no material corporate defects" at closing. The corporate record has been maintained (loosely) by a founder and a rotating series of counsel over two years. Your job is to diagnose every defect and prescribe the cleanup — before closing.

## Fact pattern

Delaware C-Corporation, formed 2024-06-01, headquartered in San Francisco.

Materials you have inherited:

1. **A Dropbox folder** containing:
   - The filed Delaware Certificate of Incorporation (stamped 2024-06-01).
   - A signed Action of Incorporator adopting bylaws (bylaws attached), appointing two co-founders (Alice, Bob) as initial directors, and resigning.
   - A signed Initial Board Consent dated 2024-06-01: appoints Alice as CEO and Bob as CTO; authorises opening a bank account; authorises the issuance of 3,500,000 common shares to Alice at $0.0001/share and 3,500,000 common shares to Bob at $0.0001/share. **No mention of an equity incentive plan.** **No mention of a form of Stock Purchase Agreement.** **No mention of indemnification agreements.**
   - Two signed Stock Purchase Agreements (Alice and Bob) with a 4-year vesting schedule, 1-year cliff, and repurchase right at cost. Signed 2024-06-14 (two weeks after formation).
   - A single 83(b) election form for Alice, signed 2024-06-14, no proof of mailing.
   - **No 83(b) election** for Bob.
2. **The Carta account** shows:
   - Alice: 3,500,000 common. Vesting: 4-year, 1-year cliff, start date 2024-06-01.
   - Bob: 3,500,000 common. Vesting: 4-year, 1-year cliff, start date 2024-06-01.
   - Employee #1 ("Charlie"): 40,000 options at $0.05 exercise price, granted 2024-09-15, labelled "ISO" on the Carta grant document.
   - Employee #2 ("Dana"): 25,000 options at $0.07 exercise price, granted 2025-01-10, labelled "ISO."
   - SAFE #1: $500,000 investment at a $10M post-money cap, dated 2024-11-01.
   - SAFE #2: $250,000 investment at a $12M post-money cap, dated 2025-03-15.
3. **No board consents** exist in the Dropbox after the 2024-06-01 initial consent.
4. **No stockholder consent** was ever executed.
5. **Delaware franchise-tax status**: last-year filing done; current-year filing overdue by four months, no confirmation of payment.
6. **Delaware registered agent**: Alice's home address in San Francisco.
7. **California Statement of Information**: never filed. California FTB Form 100: never filed.
8. **Employees**: three in California (Alice, Bob, Charlie), one in New York (Dana). No foreign qualification in either state.
9. **No indemnification agreements** with any director or officer.

## Requirements

Produce the following.

### Part A — Diagnostic report

For every defect you can identify, produce a row with:

- **Defect** — one-sentence description.
- **Statute / authority violated or at risk** — the specific citation (e.g., DGCL § 132, IRC § 422(b)(1), Treas. Reg. § 1.83-2(b), Cal. Corp. Code § 2203).
- **Severity** — Critical / High / Medium / Low, with a one-sentence rationale.
- **Likely diligence impact** — closing condition, schedule of exceptions, or comment-and-move-on.
- **Cure available?** — Yes / Partial / No, with a one-sentence rationale.

Aim for exhaustiveness. Walk the eight-item diagnostic from [chapter 06](../06-series-a-corporate-record-cleanup.md) and check for each; you should find several instances of some categories.

### Part B — Cleanup plan

Produce an ordered cleanup plan. For each step:

- **Step name and description.**
- **Documents to produce or amend** — with exhibit-level detail.
- **Owner** (external counsel, corporate secretary, CFO, founders).
- **Estimated timeline** — days from start.
- **Estimated cost** — counsel fees, tax back-payments, filing fees.
- **Dependencies** — which earlier steps must complete first.

Follow the ordering discipline in [chapter 06](../06-series-a-corporate-record-cleanup.md) (reconstruct → reactivate → ratify plan → ratify grants → 83(b)s → founder SPAs → omnibus consent → good-standing certificates → compliance calendar → schedule of exceptions).

### Part C — Bob's 83(b) analysis

Bob has no 83(b) election on file. His stock purchase was on 2024-06-14; the 30-day window closed on 2024-07-14. Today is well past that date.

- Confirm the tax consequence of a missed 83(b) for restricted stock under IRC § 83(a) and Treas. Reg. § 1.83-2.
- Model the exposure: assume the fair-market value of the common at each of Bob's vesting tranches to date has been (i) formation-day FMV of ~$0.0001/share, (ii) a Q4 2024 409A of $0.05/share (post-SAFE-1), and (iii) a Q1 2025 409A of $0.08/share (post-SAFE-2). Compute Bob's ordinary-income exposure on the shares vested through today.
- Identify the possible cures (if any) and the professional-standard-of-care recommendation. Cite Treas. Reg. § 1.83-2(b) as authority for the absence of a late-election remedy.

### Part D — Charlie's ISO status

Charlie's grant was labelled ISO. Analyse:

- Was there a validly-adopted equity incentive plan when the grant was made?
- Was the plan approved by stockholders within the IRC § 422(b)(1) 12-month window before or after board adoption?
- If not, what is the tax consequence for Charlie?
- What are the corporation's options to remediate: adopt a plan now + re-issue the grant; ratify the grant as an NSO and reissue the offer letter; other?
- What is disclosed to the Series-A investors, and how?

### Part E — Foreign-qualification cleanup

Extend the analysis from exercise 04 to this fact pattern:

- Both California and New York have unqualified employee presence.
- California is the HQ.
- Quantify the retroactive California franchise-tax liability (17 months at $800/year minimum, plus any penalties and interest — cite Cal. Rev. & Tax. Code and FTB penalty schedule).
- Quantify the New York exposure under N.Y. B.C.L. § 1312 (court-access limitation) and franchise-tax back-liability.

## Starter guidance

- Every defect should be pinned to an authority. "The board consent is missing for the SAFE issuances" is a defect; the authority is DGCL § 152 (board authorises issuance of stock — analogously, SAFEs are convertible-security issuances that require board approval).
- The cleanup ordering matters. Ratifying grants before the equity plan is validly adopted does not fix the grants; adopt the plan (with stockholder approval) first, then ratify grants under the plan.
- The Series-A schedule of exceptions is a real deliverable — some defects cannot be fully cured (Bob's 83(b), possibly). Draft the disclosure paragraph for each such item honestly.
- Do not invent penalty amounts. Cite the state's statutory or regulatory penalty schedule. Where an amount cannot be confirmed from primary sources, use `<!-- needs-research: ... -->` and estimate a plausible range.

## Deliverables

- `diagnostic-report.md` — the defect matrix (Part A).
- `cleanup-plan.md` — the ordered cleanup plan (Part B).
- `83b-analysis-bob.md` — the tax analysis and remediation memo (Part C).
- `iso-analysis-charlie.md` — the ISO / NSO analysis (Part D).
- `foreign-qualification-cleanup.md` — the CA / NY exposure and cleanup (Part E).
- `state-of-corporate-record-memo.md` — a 1–2 page executive summary suitable for presenting to the board, integrating all findings.

## Acceptance criteria

The package is acceptable if:

1. Every material defect in the fact pattern is identified with authority.
2. The cleanup plan is executable — a corporate secretary with the plan in hand and an external counsel budget could carry it out.
3. Bob's 83(b) and Charlie's ISO analyses cite statute / regulation and land on a specific tax exposure figure.
4. The Series-A schedule-of-exceptions disclosures are drafted, not just referenced.
5. Foreign-qualification cleanup includes a concrete dollar exposure for CA and NY.
6. The executive summary is short enough that a board can read it in five minutes and clear enough that it triggers a specific decision (approve cleanup budget, delegate to counsel, disclose to investors).
