# 9. SEC Reg S-K Item 402 pre-IPO executive-compensation disclosure

> The S-1 does not invent your executive-compensation story — it surfaces the one you have been writing in comp-committee minutes for the last three years, which is why the practitioner canon is "draft the CD&A three quarters before you need it."

## Motivation

Executive compensation at a private corporation is a management decision subject to the board, the comp committee, and the equity plan. Executive compensation at a *filing* corporation is a disclosure obligation. The Form S-1 and, after effectiveness, the annual proxy statement (incorporated by reference into Form 10-K Part III) require detailed, standardised, machine-readable disclosure of what the corporation paid, promised, and would be obligated to pay each named executive officer. That disclosure is governed by **Regulation S-K Item 402 (17 C.F.R. § 229.402)** and a cluster of adjacent rules (ASC 718 for grant-date fair value; IRC §§ 162(m), 280G, 409A; the JOBS Act for emerging-growth-company accommodations).

The practitioner frame: *the disclosure is the comp architecture seen through investor eyes*. A compensation decision that cannot be explained in two paragraphs of CD&A narrative, or that produces a Summary Compensation Table line that embarrasses the comp committee at a proxy-vote post-mortem, was almost always a design mistake upstream — a peer-group that stretched to justify a number, a one-off special grant that the comp committee did not minute properly, or a severance arrangement whose terms the drafter did not reconcile with the equity plan.

The canonical mistake pre-IPO is to treat Item 402 as a disclosure-counsel problem to be solved in the ninety days before S-1 filing. That timing fails on two axes. First, the facts that must be disclosed (grants, performance decisions, peer-group selection, change-of-control exposure) are made over the preceding several years, and the comp committee's minutes either support the required narrative or they do not. Second, drafting the CD&A late forces the comp committee to confront design mistakes at the one moment they are least fixable — the disclosure deadline. The remedy is the "draft the CD&A three quarters before you need it" discipline this chapter describes.

## The disclosure framework

### Reg S-K Item 402 and the Named Executive Officer

Item 402 of Regulation S-K (**17 C.F.R. § 229.402**) is the catalogue of required executive-compensation disclosures for registrants under the Securities Act and Exchange Act. It applies in the S-1 at IPO and in the annual proxy statement thereafter.

The disclosures are organised around the **Named Executive Officers (NEOs)**, defined in **Item 402(a)(3)** as:

- The person who served as **principal executive officer** (CEO) during the last completed fiscal year;
- The person who served as **principal financial officer** (CFO) during the last completed fiscal year;
- The **three most-highly-compensated executive officers** other than the CEO and CFO who were serving at fiscal year-end; and
- Up to two additional former executive officers who would have been among the three most-highly-compensated but for the fact that they were not serving at fiscal year-end.

For most pre-IPO corporations this list is CEO, CFO, and three of {COO, CTO, CPO, CRO, Chief Legal Officer, Chief Scientist} — the exact three fall out of the compensation arithmetic, not the org chart.

### Smaller reporting companies and emerging growth companies

Most pre-IPO startups file their S-1 as an **Emerging Growth Company (EGC)** under the JOBS Act of 2012 (**§ 102(c)**) and often also as a **Smaller Reporting Company (SRC)** under the SEC's size thresholds. Both regimes allow *scaled* executive-compensation disclosure:

- **EGC accommodations.** Three NEOs rather than five. Two years of Summary Compensation Table history rather than three. **No Compensation Discussion & Analysis required.** No say-on-pay vote during the EGC period. No pay-versus-performance disclosure during the EGC period.
- **SRC accommodations.** Overlap substantially with EGC accommodations; the key practical difference is that SRC status persists after EGC status expires (five years post-IPO, or earlier on revenue, debt-issuance, or large-accelerated-filer triggers — flag with <!-- needs-research: confirm the EGC-status loss triggers currently in effect: revenue threshold, non-convertible-debt threshold, large-accelerated-filer trigger, and the five-year sunset. --> ).

The scaled-disclosure path still requires most of the architecture — Summary Compensation Table, Outstanding Equity Awards, Director Compensation, and (post-EGC) Pay Versus Performance. Flag the EGC and SRC paths as the pre-IPO default when scoping the disclosure build.

## The CD&A — Item 402(b)

### What the CD&A is

The **Compensation Discussion & Analysis** (CD&A), governed by **Item 402(b)**, is a narrative — not a table — that walks the reader through *why* the corporation paid its NEOs the amounts shown in the subsequent tables. Required subject matter includes:

- The corporation's compensation **objectives** — what the program is designed to reward.
- Each **element of pay** — base salary, annual cash bonus, long-term equity, benefits, perquisites, severance and change-in-control arrangements — and the role each plays in the overall mix.
- **How amounts are determined** — the comp committee's process, use of consultants, benchmarking methodology.
- **Peer group selection and benchmarking** — the peer group used, how it was constructed, and how the corporation's pay positions against it (e.g., 50th percentile base, 75th percentile equity).
- The **relationship between compensation and risk management** — Item 402(s) also requires risk-related disclosure outside the CD&A for larger filers.

The CD&A is *not* required for EGCs. Many EGCs include a shorter voluntary **Executive Compensation Overview** that performs the same investor-communication function at reduced regulatory exposure; disclosure counsel and the comp committee should discuss which path to take.

### The "three quarters out" drafting cycle

The practitioner-canon pre-IPO cycle is to draft the CD&A (or the Executive Compensation Overview, for EGCs) three quarters before it must be filed:

- **Q1 — Benchmarking refresh and philosophy articulation.** The comp consultant (Compensia, Radford, or a boutique — see [chapter 05](./05-compensation-committee.md)) refreshes the peer group. The comp committee re-articulates the compensation philosophy and the target market positioning. The output is a philosophy memo and a peer-group memo both suitable for CD&A quotation.
- **Q2 — Compensation decisions with CD&A rationale embedded in comp-committee minutes.** Each merit cycle, each promotion, each refresh grant, each special grant is minuted with the *decision rationale*: why this amount, benchmarked how, approved by whom, informed by what performance assessment. The GC and the Head of People review each decision for disclosure risk.
- **Q3 — CD&A first draft.** Disclosure counsel drafts the CD&A against the Q1 memos and Q2 minutes. Gaps surface — "we never minuted why we did that" — and either the fact is reconstructed from contemporaneous records or the decision rationale is clarified now, while it is still fixable.
- **Q4 — CD&A locked for filing.** The draft is reviewed by the comp committee, by the audit committee for ASC 718 consistency, and by the full board. The CD&A is paginated with the Summary Compensation Table and the supporting tables.

The discipline is not that the CD&A text is literally frozen three quarters out — the facts of Q3 and Q4 will update it. The discipline is that the comp committee has already seen the structure, the peer group, and the narrative *at the moment the decisions are made*, and is making decisions with the disclosure footprint in mind.

## Summary Compensation Table — Item 402(c)

### Columns

The **Summary Compensation Table (SCT)**, governed by **Item 402(c)**, is the single most-read exhibit in the entire disclosure. Columns:

- **Name and Principal Position**
- **Year** (three fiscal years for CEO and CFO at steady state; two for other NEOs; **one year** for EGCs electing scaled disclosure, two for subsequent filings as an EGC)
- **Salary** — cash base pay earned in the fiscal year
- **Bonus** — discretionary cash bonus (non-performance-plan)
- **Stock Awards** — **grant-date fair value under ASC 718** of RSU / RSA grants made in the fiscal year
- **Option Awards** — **grant-date fair value under ASC 718** of option grants made in the fiscal year
- **Non-Equity Incentive Plan Compensation** — performance-based cash bonuses earned in the fiscal year (whether paid or accrued)
- **Change in Pension Value and Non-Qualified Deferred Compensation Earnings** — rare at startups
- **All Other Compensation** — perks, 401(k) match, insurance premiums, relocation, tax gross-ups
- **Total**

### The ASC 718 grant-date-fair-value measurement problem

The Stock Awards and Option Awards columns use **ASC 718 grant-date fair value** — the same measure as the audited financial statements. For options, that is a Black-Scholes or lattice-model fair value as of the grant date; for RSUs it is the fair value of the underlying stock at grant. This value can diverge dramatically from "realised" value — a CEO granted options with a $5M grant-date fair value in year T may realise $20M or $0 depending on share-price performance between grant and exercise. Investors read the SCT total as "CEO pay" when it is in fact "accounting-recognised compensation" — a known investor-communication issue the CD&A narrative must address, often with a supplemental "realised pay" table (not required by Item 402 but widely used).

## The equity-award tables

### Grants of Plan-Based Awards — Item 402(d)

The **Grants of Plan-Based Awards table** (**Item 402(d)**) disaggregates the Stock Awards and Option Awards columns of the SCT by individual grant made during the fiscal year. For each NEO and each grant: grant date; estimated future payouts under non-equity incentive plans (threshold / target / maximum); estimated future payouts under equity incentive plans (threshold / target / maximum); all other stock awards (RSUs); all other option awards; exercise price; grant-date fair value. The table **reconciles with the SCT grant-date fair value** — a tie-out disclosure counsel verifies before filing.

### Outstanding Equity Awards at Fiscal Year-End — Item 402(f)

The **Outstanding Equity Awards table** (**Item 402(f)**) shows the *standing position* of each NEO's unexercised and unvested equity at fiscal year-end: option awards split into exercisable and unexercisable tranches, each with the number of underlying shares, exercise price, and expiration date; stock awards (RSUs and RSAs) split into vested and unvested tranches, each with the number of shares and market value at year-end. This table is the primary mechanism by which the market understands the NEO's go-forward incentive alignment.

### Option Exercises and Stock Vested — Item 402(g)

The **Option Exercises and Stock Vested table** (**Item 402(g)**) reports the *flow* events during the fiscal year — option exercises and RSU / RSA vesting events — with the number of shares and value realised at exercise or vesting.

## Pension benefits and non-qualified deferred compensation

**Items 402(h) and (i)** cover defined-benefit pension plans and non-qualified deferred compensation. Both are rare at pre-IPO startups — flag that the corporation has none, and the tables are omitted or shown with "N/A." If the corporation adopts a NQDC plan (see [chapter 04](./04-executive-compensation-packages.md)), the Item 402(i) disclosure becomes material and must be built out.

## Potential Payments Upon Termination or Change-in-Control — Item 402(j)

### What it requires

**Item 402(j)** requires a hypothetical disclosure of what each NEO *would receive* under each of several termination and change-in-control scenarios *as of fiscal year-end* — treating the triggering event as if it had occurred on the last day of the fiscal year. The scenarios typically disclosed:

- Termination **without cause**
- Termination **for cause**
- **Change-in-control without termination** (single-trigger acceleration, if any)
- **Change-in-control with termination** (double-trigger acceleration)
- **Death**
- **Disability**
- **Good-reason resignation**

For each scenario and each NEO: cash severance; accelerated equity (number of shares, intrinsic value at year-end stock price); continued benefits (COBRA, life insurance); tax gross-ups (280G); any other payments. Table-and-narrative format.

### Where upstream policy decisions show through

Item 402(j) is the disclosure where **executive severance** (see [chapter 08](./08-executive-severance-and-release.md)) and **change-of-control equity policy** (see [chapter 07](./07-change-of-control-equity-policy.md)) show through to investors in quantified form. A single-trigger acceleration policy that the comp committee adopted three years earlier becomes a line item investors read and vote on. The disclosure is typically the single most time-consuming exhibit to prepare: for each NEO and each scenario, the drafter must compute equity acceleration under the equity plan, cash severance under the executive severance plan, 280G cutback or gross-up under the CoC agreement, and 409A payment-timing constraints, then reconcile the arithmetic against the plan documents.

## Director Compensation Table — Item 402(k)

**Item 402(k)** requires a Director Compensation Table for each **non-employee director**: cash retainer, committee-chair retainer, meeting fees (increasingly rare), equity grants (grant-date fair value under ASC 718), and all other compensation. Employee directors (typically the CEO) are not included — their director service is captured in the NEO disclosures. The non-employee director compensation program is a comp-committee decision (see [chapter 05](./05-compensation-committee.md)) and should be set with the Item 402(k) footprint in mind.

## CEO pay ratio — Item 402(u)

**Item 402(u)** requires disclosure of:

- The CEO's **annual total compensation** (as reported in the SCT);
- The **median employee's** annual total compensation (computed on the same SCT basis);
- The **ratio** of CEO to median employee total compensation; and
- A **methodology description** — how the median employee was identified (which "consistently applied compensation measure" was used), whether statistical sampling was used, any cost-of-living adjustments, and any annualising adjustments for part-year employees.

The ratio does not need to be re-identified every year — the median employee can be used for up to three years absent material changes in employee population or compensation arrangements. The reputational stakes are high: the ratio becomes a headline number in press coverage and proxy-advisor reports, and the methodology is scrutinised. Prepare carefully with the Head of People, Finance, and disclosure counsel in a joint working session well before filing.

## Pay versus performance — Item 402(v)

**Item 402(v)** requires a table correlating NEO "compensation actually paid" (**CAP**) with company performance measures over multiple fiscal years:

- Required for fiscal years ending on or after a specified effective date <!-- needs-research: confirm the current effective date of Item 402(v); the final rule was adopted in 2022 with first-filing effectiveness tied to fiscal years ending on or after Dec 16, 2022, but confirm current status and any amendments. -->.
- Table columns typically include SCT total compensation, CAP, company TSR, peer-group TSR, net income, and a **company-selected measure** of financial performance that the registrant designates as its most important performance measure for linking CAP to performance.
- Steady state is **five years**, phased in from three years for new filers.

The **CAP measure** adjusts SCT grant-date fair values to reflect **year-end fair values of outstanding unvested awards** plus **vesting-date fair values of awards that vested during the year**, with offsets for prior-year fair values of awards still outstanding. This is a complex calculation that is a known source of filing errors — the compensation consultant and the external auditor should both review the CAP arithmetic in parallel.

EGCs are **not required** to provide Pay-versus-Performance disclosure during their EGC period. Build the data model anyway during the EGC years; the first non-EGC proxy will require it on an accelerated timeline.

## The accounting, tax, and disclosure interaction

Item 402 does not sit alone. Four adjacent regimes shape the numbers in the tables:

- **FASB ASC 718** governs the grant-date fair value shown in SCT Stock Awards and Option Awards and in the Grants of Plan-Based Awards table. The audit firm's valuation workpapers are the source document for these columns.
- **IRC § 162(m)** caps deductibility of compensation above $1M per covered employee at the public-company level. The cap re-emerges post-IPO as a tax item that disclosure counsel and the CFO must reflect in the CD&A.
- **IRC § 280G** imposes an excise tax on "excess parachute payments" in change-of-control scenarios, which the Item 402(j) disclosure must either show as a gross-up (controversial — ISS and Glass Lewis typically oppose) or as a cutback (the modern default).
- **IRC § 409A** governs payment-timing of deferred compensation. The Item 402(j) scenarios must respect 409A's six-month-delay rule for specified employees and other timing constraints.

The disclosure drafter must reconcile all four regimes to the same numbers in the same tables. Discrepancies between the audit workpapers and the Item 402 tables are the single most common filing-review comment.

## The pre-IPO draft-forward discipline

The S-1 preparation cycle rewards one specific habit: **the comp committee treats each quarter's compensation decisions as if they will appear in next year's CD&A.** Concretely:

- The GC and the CFO review each comp-committee decision with disclosure counsel in advance of the meeting.
- The comp-committee minutes capture the decision *rationale* — the peer-group reference, the performance assessment, the benchmarking percentile — in language that can be lifted directly into the CD&A narrative.
- The Head of People maintains a running "disclosure diary" — a per-NEO log of grants, promotions, title changes, and comp changes that will populate the SCT, Grants of Plan-Based Awards table, and Outstanding Equity Awards table at filing time.
- The audit firm's ASC 718 workpapers are built contemporaneously, not reconstructed at filing time.

The failure mode this avoids is the "we never documented why we did that" conversation ninety days before S-1 filing, when the disclosure counsel asks why the CEO received a $4M special grant in year T-2 and no one on the current comp committee can reconstruct the rationale.

## The outside advisor stack

A pre-IPO corporation ramping into Item 402 disclosure typically engages:

- **Disclosure counsel** — outside securities counsel (the firm running the S-1), who owns the final Item 402 text and the SEC-staff comment letters.
- **Compensation consultant** — Compensia, Radford, Semler Brossy, FW Cook, or a boutique — who owns the peer group, the benchmarking memos, and the CD&A philosophy inputs (see [chapter 05](./05-compensation-committee.md)).
- **Audit firm** — who owns the ASC 718 grant-date-fair-value calculations and the tie-out between the Item 402 tables and the audited financial statements.
- **Proxy advisor engagement (post-IPO)** — ISS and Glass Lewis both publish policy frameworks that influence say-on-pay votes; the IR team and the comp committee establish engagement rhythms in year one as a public company. See also [`../mod-111-corporate-governance-board-operations-and-officer-duties/`](../mod-111-corporate-governance-board-operations-and-officer-duties/).

## A worked example

A pre-IPO corporation — call it **Lanterne Analytics, Inc.** — is two quarters out from its S-1 filing. The corporation plans to file as an EGC. Headcount is 420; the comp committee has been operating for three years; the CEO, CFO, Chief Revenue Officer, Chief Product Officer, and Chief Technology Officer are the five most-highly-compensated executive officers (as EGC, three NEOs are required — the corporation will disclose CEO, CFO, and CRO).

**Where Lanterne stands.** The Head of People and the GC are running the pre-IPO draft-forward discipline. Comp-committee minutes for the last six quarters contain explicit CD&A-ready rationale on each major decision. Compensia has refreshed the peer group three times in the last two years; the current peer group is a 15-company set of US-listed SaaS companies at $300M–$1.5B revenue with similar growth profiles. The audit firm's ASC 718 workpapers tie out to the equity ledger.

**The CD&A outline.** Although EGC filing does not require a formal CD&A, Lanterne will include an **Executive Compensation Overview** of approximately eight pages. Sections: (1) Compensation Philosophy — pay-for-performance at the 50th percentile base, 65th-percentile equity, with upside tied to multi-year growth. (2) Elements of Pay — base, annual bonus (performance plan), long-term equity (annual RSU grant with 4-year vesting), benefits, severance and CoC. (3) Peer Group — the 15-company set, with the methodology memo quoted. (4) 2026 Decisions — the merit cycle, the two promotion grants (CTO and CPO were promoted mid-year), the new-hire grant for the CRO who joined 11 months before filing. (5) Risk — the clawback policy adopted 18 months ago, the hedging and pledging prohibition.

**The five tables that go in.** Summary Compensation Table (two fiscal years, three NEOs). Grants of Plan-Based Awards (fiscal 2026 only). Outstanding Equity Awards at Fiscal Year-End (full standing position). Option Exercises and Stock Vested (fiscal 2026 flow — the CEO exercised early options; two of the three NEOs had RSUs vest). Potential Payments Upon Termination or Change-in-Control (seven scenarios × three NEOs = 21 rows plus narrative — the CFO has owned this build-out for four months).

**Director Compensation Table.** Seven non-employee directors; cash retainer $50k; committee-chair retainers for Audit ($20k), Comp ($15k), and Nom-Gov ($10k); annual equity grant with grant-date fair value <!-- needs-research: confirm the current-market non-employee director equity-grant fair value for a pre-IPO SaaS corporation at this stage; a commonly cited range is $200k–$400k annualised. -->.

**CEO pay ratio.** Not required for EGCs during the EGC period; Lanterne will build the data model this quarter so the ratio is production-ready for the first non-EGC proxy.

**Pay versus performance.** Not required for EGCs during the EGC period; Lanterne will build the CAP calculation workpapers in parallel with the audit firm, so the first non-EGC year has three years of CAP history ready to disclose.

**Minute-capture discipline the Head of People and the GC are running.** Every comp-committee meeting has a standing agenda item: "disclosure-readiness review." Every decision is captured with: (a) the peer-group reference, (b) the performance-assessment input, (c) the benchmarking percentile, (d) the committee's explicit rationale. The GC maintains a running CD&A-skeleton document that every decision slots into. Disclosure counsel has reviewed the skeleton twice in the last six months.

## Summary

- Reg S-K Item 402 (17 C.F.R. § 229.402) governs executive-compensation disclosure in the S-1 and the annual proxy. The disclosure is the comp architecture seen through investor eyes; mistakes become proxy-vote and reputation events.
- The Named Executive Officers are CEO, CFO, and the next three most-highly-compensated executive officers under Item 402(a)(3); EGCs disclose three NEOs under JOBS Act § 102(c) scaled disclosure, with no CD&A required.
- The required exhibits are the CD&A (Item 402(b)), Summary Compensation Table (402(c)), Grants of Plan-Based Awards (402(d)), Outstanding Equity Awards (402(f)), Option Exercises and Stock Vested (402(g)), pension / NQDC (402(h) / (i)), Potential Payments on Termination or CoC (402(j)), Director Compensation (402(k)), CEO Pay Ratio (402(u)), and Pay versus Performance (402(v)).
- Stock Awards and Option Awards in the Summary Compensation Table use ASC 718 grant-date fair value, which diverges from realised value — a known investor-communication issue the narrative must address.
- The "draft the CD&A three quarters before you need it" discipline forces the comp committee to confront design mistakes while they are still fixable: Q1 benchmarking, Q2 decision-making with CD&A-ready minutes, Q3 first draft, Q4 lock. See [chapter 04](./04-executive-compensation-packages.md), [chapter 05](./05-compensation-committee.md), [chapter 07](./07-change-of-control-equity-policy.md), and [chapter 08](./08-executive-severance-and-release.md) for the upstream policy decisions that surface in Item 402.
- The outside advisor stack is disclosure counsel + comp consultant + audit firm pre-IPO, with ISS / Glass Lewis engagement added at post-IPO. Item 402(j), (u), and (v) in particular require coordinated drafting across all three.
