# Exercise 06 — Franchise-tax & annual-report calendar authoring

> Estimated time: **~2 hours** · Related chapter: [03 — The corporate record and the compliance calendar](../03-corporate-record-and-compliance-calendar.md)

## Problem statement

You have inherited a corporation with no rolling compliance calendar. The company operates in five states, is Delaware-incorporated, and is on a calendar fiscal year. Your job is to build the corporation's **rolling 24-month compliance calendar** covering every federal, Delaware, and state-of-operation filing — with owners, cadences, reminder lead-times, and cost estimates.

## Fact pattern

- Delaware C-Corporation.
- Fiscal year: December 31.
- Formed 2024-06-01. Foreign-qualified in CA, NY, TX, WA, and MA (assume qualified as of today).
- Commercial registered agent (choose one of CSC, CT, Cogency, InCorp) is agent of record in Delaware and in each of the five foreign-qualification states.
- Board: five directors (two founders + three independent / investor). Board meets quarterly on the third Thursday of the last month of each quarter.
- Stockholders: founders + a handful of angels + two priced-round investors (Seed and Series A).
- Officers: CEO, CTO, COO, CFO, Secretary (the COO). The CFO is the compliance-calendar owner for tax filings; the Secretary is the owner for corporate filings.
- Payroll: employees in all five foreign-qualification states, run through an HRIS + PEO combination.
- Equity: an equity incentive plan with regular ISO exercises expected each calendar year.

## Requirements

### Part A — Master 24-month calendar

Produce a rolling 24-month compliance calendar in tabular form (spreadsheet or markdown table) with, at minimum, the following columns:

- **Date** (or date window).
- **Filing / task** (e.g., "Delaware Annual Report and Franchise Tax," "California Statement of Information," "IRS Form 3921 to employees," "Q3 board meeting").
- **Cadence** (annual, biennial, quarterly, one-time).
- **Statutory / regulatory basis** (e.g., 8 Del. C. § 502; Cal. Corp. Code § 1502; IRC § 6039 / Form 3921 instructions; DGCL § 211(b)).
- **Owner** (CFO, Corporate Secretary, external counsel, external tax firm).
- **Reminder lead-time** (e.g., "60 days" for the annual report; "14 days" for a routine renewal).
- **Estimated cost** (filing fee + estimated tax where computable; a placeholder with a `<!-- needs-research: ... -->` note where the cost varies by facts you have not fixed).
- **Notes** (dependencies, e.g., "requires Delaware Certificate of Good Standing dated within 30 days," or "board approval required").

The calendar must include, at minimum:

**Federal filings**
- Federal Form 1120 (annual, due April 15 for calendar-year filers; six-month automatic extension via Form 7004).
- IRS Form 3921 for each ISO exercise in the calendar year — to employees by January 31, to IRS by February 28 (paper) / March 31 (electronic).
- IRS Form 3922 for any ESPP transfers (if applicable).
- Any federal estimated-tax payment dates.

**Delaware filings**
- Delaware Annual Report and Franchise Tax (due March 1 annually for corporations).
- Delaware LLC franchise tax ($300 flat, due June 1) — only if the corporation has a Delaware LLC subsidiary.

**State-of-operation filings** (for each of CA, NY, TX, WA, MA)
- State annual / biennial report (e.g., California SI-550 annual; New York Biennial Statement; Texas Public Information Report; Washington Annual Report; Massachusetts Annual Report).
- State franchise / entity tax (e.g., California FTB Form 100 with $800 minimum; New York corporation franchise tax; Texas franchise tax / Public Information Report; Massachusetts corporation excise; Washington business & occupation tax if applicable).
- State registered-agent renewal.

**Corporate-governance cadence (self-imposed but calendar-required)**
- Annual stockholder meeting under DGCL § 211(b) (in-lieu-of by written consent is typical for private companies; date it consistently).
- Quarterly board meetings.
- D&O insurance renewal (annual, on policy anniversary).
- Directors' Certificates of Good Standing renewal (typically annually or ahead of any material transaction).

**Ongoing calendar hygiene**
- Quarterly compliance-calendar review (owner: Corporate Secretary).
- Annual compliance-calendar audit (owner: Corporate Secretary + external counsel).

### Part B — Runbook per filing

For each of the following filings, produce a one-page runbook: what triggers the deadline, what documents must be assembled, who signs, where the filing is submitted, and how the confirmation is stored in the corporate record.

1. **Delaware Annual Report and Franchise Tax.**
2. **California FTB Form 100 and California Statement of Information (SI-550).**
3. **New York Biennial Statement and NY franchise tax.**
4. **IRS Form 3921** for the calendar year's ISO exercises.
5. **Annual stockholder consent in lieu of meeting** satisfying DGCL § 211(b).

### Part C — Reminder architecture

Describe how you would operationalise the calendar so that no filing is missed:

- What tool holds the calendar (Google Calendar / Notion / Asana / Athennian / Diligent Entities / Carta Compliance)?
- Who receives what reminders, at what lead-time, on what channel?
- What is the escalation path if a filing is not confirmed 5 business days before deadline?
- What is the annual audit process to reconcile "filings on the calendar" against "filings actually made" against "filings required"?

### Part D — Cost summary

Produce a one-page total-annual-cost summary: federal, Delaware, each state, registered-agent fees, D&O renewal (if you can estimate a first-year band), and any external counsel or filing-service fees. This is the number the CFO uses to build the compliance-overhead line item in the operating budget.

## Starter guidance

- Delaware's franchise-tax dates and rate structure are on the Delaware Division of Corporations website (https://corp.delaware.gov/); confirm the current-year minimum and maximum before publishing a dollar figure.
- California's SI-550 must be filed within 90 days of foreign qualification and then annually by the end of the month of qualification anniversary; California's FTB imposes an $800 annual minimum franchise tax on corporations.
- New York's biennial statement is due every two years, in the month of qualification anniversary.
- Texas's franchise tax and Public Information Report are due May 15 annually.
- Massachusetts's annual report for corporations is due within 2.5 months of fiscal-year end (March 15 for a calendar-year filer).
- Washington's B&O tax cadence depends on the corporation's revenue tier.
- Use `<!-- needs-research: ... -->` for any figure or cadence you cannot confirm from a primary source (state Secretary of State site, state tax authority site, IRS instruction) before publishing.

## Deliverables

- `compliance-calendar.md` (or `.xlsx`, `.csv`) — the 24-month calendar (Part A).
- `runbooks/` — one file per runbook in Part B.
- `reminder-architecture.md` — the reminder / escalation / audit design (Part C).
- `cost-summary.md` — the annual-cost summary (Part D).

## Acceptance criteria

The package is acceptable if:

1. Every filing has a date, an owner, a statutory basis, a lead-time reminder, and a cost estimate (with `<!-- needs-research: ... -->` where a figure could not be confirmed).
2. The runbooks are executable — a new corporate secretary could carry out each without asking follow-up questions.
3. The reminder architecture would catch a filing 30 days before deadline, not the day after.
4. The cost summary is a real budget line item, not a range with no midpoint.
5. Nothing on the calendar is a duplicate or is scheduled on a weekend / federal holiday without a "practical due date" adjustment.
