# 3. The corporate record and the compliance calendar

> The minute book is the corporation's memory. The compliance calendar is what keeps it from lapsing.

## Motivation

A corporation is a legal person that exists only in paper. If the paper is missing, disorganised, or contradicts itself, the corporation cannot prove that its board authorised the transactions its officers signed, cannot prove who owns its equity, and cannot demonstrate to Series-A counsel that its governance is real. The corporate record is not an archive kept "for compliance" — it is the primary evidence the corporation produces every time an investor, an acquirer, a lender, or a regulator asks how a decision was made. And every jurisdiction the corporation operates in imposes filings and taxes on a schedule; missing them creates penalties, back-taxes, and — in some cases — loss of good standing that blocks the ability to sue, close a financing, or complete an M&A transaction.

This chapter defines what belongs in the corporate record and what belongs on the compliance calendar.

## The minute book: what belongs, and how it is organised

The "minute book" is the corporation's book of records. Historically a physical binder; today, a curated cloud folder (or a Carta / Pulley / Athennian corporate-record module) with structured sub-folders and an index. Whatever the format, the contents are the same.

**Formation and charter section**
- Filed and date-stamped Certificate of Incorporation and any subsequent Certificates of Amendment, Certificates of Designation, and Restated Certificates. Always keep the state-stamped copy, not just the signed submission.
- Action of Incorporator.
- Bylaws (current version) and every prior version with an adoption-date memo.
- Certificates of Good Standing from Delaware (obtained periodically; required at every financing closing and any M&A transaction).

**Board section**
- Every board meeting: notice, agenda, minutes, resolutions, and pre-read materials.
- Every board written consent under DGCL § 141(f), dated and signed by every director.
- Every board committee charter (audit committee, compensation committee, nominating and governance committee, technology or security committee if separately chartered).
- Every committee meeting or committee consent.
- Officer appointment resolutions and officer resignations.
- Director appointment / election resolutions and director resignations.

**Stockholder section**
- Every stockholder meeting: notice, proxy statement, minutes, and vote-count.
- Every stockholder written consent under DGCL § 228, dated and signed.
- Certificates of Designation and other charter amendments authorised at stockholder-level.

**Equity section**
- The share ledger (stock ledger): every issuance, every transfer, every cancellation, every repurchase, with date, holder, share count, class, certificate number (if certificated) or book-entry reference (if uncertificated per DGCL § 158), and consideration.
- The option ledger: every option grant, holder, grant date, board-approval date, exercise price, vesting schedule, expiration date, and post-termination exercise window; every exercise; every cancellation.
- The convertible-instrument ledger: SAFEs, convertible notes, and warrants outstanding, with principal, cap, discount, maturity, conversion mechanics, and current status.
- Executed Stock Purchase Agreements for every founder and every restricted-stock recipient.
- Executed 83(b) elections with certified-mail receipts.
- The current cap table, reconciled to the share ledger, option ledger, and convertible-instrument ledger.

**Contract section (governance-adjacent, not commercial)**
- Indemnification Agreements (one per director and officer).
- Voting Agreements, Right of First Refusal / Co-Sale Agreements, Investor Rights Agreements, and Registration Rights Agreements (usually starting at the priced-round stage — kept in the minute book once executed).
- Stockholders' agreements (early-stage), if any.

**Regulatory and tax section**
- IRS Form SS-4 confirmation (EIN letter).
- Every Form 3921 (ISO exercise information return) and Form 3922 (ESPP information return) filed.
- Every Delaware annual franchise-tax report and confirmation.
- Every state annual report (California Statement of Information; Delaware annual report; equivalents in each state of qualification).
- Every foreign-qualification Certificate of Authority.
- Every registered-agent designation and every change of registered agent.
- Every state and local business licence.

**Insurance and risk section**
- D&O (directors and officers) policy declarations and policies.
- Employment Practices Liability, Cyber, General Liability, and other operating policies (governance-relevant portions).

**Reference: which authority binds what to the record**

- **DGCL § 224** requires the corporation to maintain a stock ledger.
- **DGCL § 220** grants stockholders the right to inspect books and records for a proper purpose — including the stock ledger. Failure to maintain leaves the corporation exposed at inspection demand.
- **DGCL § 142(a)** and **§ 158** connect officer authorization and share issuance to the record.
- **DGCL § 141(f)** requires unanimous written consent for board action-in-lieu-of-meeting and requires the consent to be filed with the minutes of proceedings of the board.
- **DGCL § 228(e)** requires prompt notice of stockholder action by consent to non-consenting stockholders.

## The share ledger

The stock ledger is the single most important operational record in the minute book. It is the corporation's authoritative source for **who owns what**. Practical requirements:

- Every issuance is recorded on the date of issuance, tied to the board consent that authorised it, and reflects the consideration received.
- Every transfer is recorded on the date of transfer, tied to a stock transfer form and any required corporate consent (right of first refusal, board approval, transfer restriction compliance).
- The corporation's transfer agent is either the corporation itself (via the corporate secretary or Carta / Pulley / equivalent tool acting as a book-entry system) or a commercial transfer agent (usually engaged at the pre-IPO stage).
- The ledger is reconciled to the cap table every time a change is made. A cap table that disagrees with the ledger is a diligence problem waiting to be discovered.

Modern cap-table tools (Carta, Pulley, Shareworks, Global Shares) function as the operational share ledger for most venture-backed startups. That is a fine choice — but note that the tool is an operational instrument; the underlying legal record is still the board consent that authorised each issuance. Data in Carta without a corresponding board consent in the minute book is a defect.

## The compliance calendar

The corporate secretary function owns a rolling 24-month compliance calendar. Every startup calendar contains, at minimum:

### Federal filings

- **IRS Form SS-4** at formation (one-time).
- **Annual federal income tax return** (Form 1120 for a C-corporation), due the 15th day of the fourth month after fiscal-year end (April 15 for a calendar-year corporation), with an automatic six-month extension available on Form 7004.
- **Form 3921** for each ISO exercise during the calendar year, due to the IRS by February 28 (paper) / March 31 (electronic) of the following year, and to the employee by January 31 of the following year.
- **Form 3922** for each ESPP share transfer, same due-date structure.
- **Form 8-K, 10-Q, 10-Q, 10-K, 8-K** — deferred until public-company stage; not in scope for this module.
- **Delaware Form 1120 pre-filing / state coordination** as advised by tax counsel.

### Delaware filings

- **Delaware Annual Report and Franchise Tax** — due March 1 each year for corporations, filed with the Delaware Division of Corporations. The report identifies the corporation's registered office, registered agent, principal place of business, all directors, and one officer.
- **Delaware franchise tax** is calculated by one of two methods:
  - **Authorized Shares Method**: default calculation. Minimum $175 / year for a corporation with ≤5,000 authorized shares; scales up with authorized share count. <!-- needs-research: verify current Delaware Division of Corporations franchise-tax minimum ($175 confirmed historically) and maximum ($200,000, with a "large corporate filer" tier at $250,000) at time of publication. Confirm from https://corp.delaware.gov/. -->
  - **Assumed Par Value Capital Method**: alternative calculation based on issued shares, authorized shares, and gross assets. Minimum $400 / year. For a startup with a large authorized-share pool and low par value, this method usually produces a materially lower tax; the corporation pays the lesser of the two.
- **Delaware LLC franchise tax** (if any Delaware LLC subsidiary): flat $300 / year, due June 1.
- **Amendments and Certificates of Designation**: filed as needed, with the standard Delaware filing fees.

### State-of-operation filings

For each state where the corporation is foreign-qualified (see [chapter 04](./04-foreign-qualification-across-states.md)), the calendar includes:

- The state's annual report / statement of information.
- The state's franchise tax or entity-level tax (California's $800 minimum franchise tax for corporations is the most-cited example; California FTB Form 100).
- Registered-agent renewal in that state.
- State-specific tax filings: sales tax, employment tax, gross receipts tax as applicable.

### Corporate-governance cadence (self-imposed)

- **Annual stockholder meeting** required by DGCL § 211(b). Private companies typically handle this by written consent in lieu of a physical meeting, dated the same day each year to establish a cadence.
- **Board meetings**: commonly quarterly at seed and Series-A; can be more frequent at Series-B+. Every meeting produces minutes; every off-cycle decision produces a written consent.
- **D&O insurance renewal** annually (or at whatever policy period the carrier issues).
- **Registered-agent fee renewal** annually (commercial registered agents typically invoice on the anniversary of engagement).

## The registered agent

Every Delaware corporation must maintain a registered office and registered agent in Delaware (8 Del. C. § 132). Every foreign-qualified corporation must maintain a registered agent in each state of qualification. The registered agent's job is to be reachable in that state during business hours to receive service of process and official state notices, and to forward them promptly to the corporation.

Commercial registered agents named in the plan for this module — **Corporation Service Company (CSC)**, **CT Corporation** (a Wolters Kluwer business), **Cogency Global**, **InCorp** — offer national coverage: one contract, agent-of-record status in every state the corporation qualifies in, and a single dashboard for annual-report and franchise-tax reminders. There are smaller registered-agent providers (Harvard Business Services, LegalCorp, Northwest Registered Agent) that are perfectly fine for a Delaware-only footprint; multi-state operating startups typically standardise on one of the four national providers.

**The "stale registered agent" failure mode.** When a corporation changes address, changes counsel, forgets to pay the registered-agent invoice, or migrates from a founder's personal address to a commercial agent without filing the change, the state's registered-agent record goes out of sync with reality. Service of process — a lawsuit, a subpoena, a state notice — goes to a stale address, is not forwarded, and a default judgment or loss of good standing follows. Series-A counsel treats a stale registered agent as a red flag because it signals the corporate record is generally not being maintained. See [chapter 06](./06-series-a-corporate-record-cleanup.md).

## Certificates of Good Standing

A Certificate of Good Standing is a state-issued document confirming that the corporation exists, is authorised to do business in that state, and has paid all fees and filings due. Series-A financings, credit-facility closings, M&A transactions, and cross-state qualifications all require one or more certificates dated within a short window (typically 30 days) of the closing. The corporation should order certificates from Delaware and each state of qualification as part of its normal closing preparation; certificates from Delaware are available electronically from the Division of Corporations, usually within a few business days.

## Indemnification agreements

Bylaws provide the enabling framework for indemnification under DGCL § 145; individual **Indemnification Agreements** with each director and officer harden that framework into a contract. A typical D&O indemnification agreement:

- Commits the corporation to indemnify to the fullest extent permitted by DGCL § 145.
- Requires advancement of expenses upon receipt of an undertaking to repay if indemnification is ultimately not available.
- Covers pre-appointment conduct if the director/officer served in another capacity, and post-departure claims for conduct while in office.
- Prohibits amendment or termination in a way that adversely affects prior conduct.

These agreements are approved by the board (usually via the Initial Board Consent form) and signed at the time each director or officer is appointed. Missing indemnification agreements is a Series-A diligence finding; more importantly, a director who is sued and discovers the corporation never gave them one is a governance problem the corporation would prefer never to have.

## Concrete example: a first-year compliance calendar

For a Delaware C-corporation formed on 2026-02-01, headquartered in San Francisco with employees only in California, that engaged a commercial registered agent in Delaware:

| Date        | Filing / task                                                         | Owner       |
| ----------- | --------------------------------------------------------------------- | ----------- |
| 2026-02-01  | Formation package: charter, bylaws, board consent, founders' issuances | Counsel     |
| 2026-02-15  | Deadline for last founder's § 83(b) election (14 days after issuance)  | Each founder|
| 2026-02-28  | EIN in hand; bank account opened; foreign-qualified in California      | COO / CFO   |
| 2026-04-15  | Delaware Franchise Tax and Annual Report *for the prior year* — not applicable for a Feb-2026 formation; first Delaware annual report is due 2027-03-01 | Corp Sec    |
| 2026-04-15  | Federal Form 1120 for fiscal year ending 2026-12-31 — not yet due     | CFO / tax   |
| 2026-06-30  | California Statement of Information (Form SI-550) due within 90 days of qualification | Corp Sec |
| 2026-12-31  | Fiscal-year end; begin ISO Form 3921 preparation for any exercises    | CFO / equity|
| 2027-01-31  | Form 3921 statements to employees who exercised ISOs                  | CFO / equity|
| 2027-02-15  | California FTB Form 100 estimated tax payment (varies by revenue)     | CFO         |
| 2027-03-01  | Delaware Annual Report + Franchise Tax (first)                        | Corp Sec    |
| 2027-04-15  | Federal Form 1120 (first)                                             | CFO         |
| 2027-04-15  | California FTB Form 100 (first)                                       | CFO         |

Every deadline goes into a shared calendar with an owner, a two-week advance reminder, and a rollover into the following year's calendar as soon as the current-year task is complete. The Corporate Secretary function owns the calendar; other officers own their filings.

## Summary

- The minute book has a specific structure: formation, board, stockholder, equity, contract, regulatory, insurance. Every corporate action produces an entry; the entry is dated, signed, and indexed.
- The share ledger — not the cap-table dashboard — is the authoritative record of ownership. Every issuance traces back to a board consent.
- The compliance calendar owns federal, Delaware, and each-state-of-operation filings on a rolling 24-month basis. The Corporate Secretary owns the calendar; individual officers own their filings.
- Delaware franchise tax is calculated by two methods; the corporation pays the lower of the two.
- The registered agent is a state-visible representation of the corporation. Keep it current; a stale agent is both a real risk (default judgments) and a signal (diligence red flag).
- D&O indemnification agreements are executed at appointment. Retrofitting them post-crisis is uncomfortable and sometimes ineffective.
