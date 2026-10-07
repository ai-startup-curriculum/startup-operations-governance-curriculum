# 6. The annual comp cycle

> A rolling cadence of ad-hoc raises is not a compensation philosophy. It is a drift machine. The annual cycle exists so that every merit, equity, and promotion decision passes through the same calibration, the same budget, and the same ratifying body on the same calendar — once a year, auditably.

## Motivation

Compensation decisions are the output of a corporate process whether the corporation designs that process or not. In the absence of an annual cycle, raises happen when a manager loses sleep over a flight-risk conversation, equity refreshes happen when a VP escalates to the CEO, and promotions happen when someone's title finally embarrasses the hiring manager into fixing it. Every one of those decisions is defensible in isolation; collectively they produce a compensation landscape that no comp committee has ever actually ratified.

The annual cycle is the mechanism that converts the previous year's performance-review conclusions into the current year's comp decisions in a single, repeatable, auditable pass. It forces every manager to make merit, equity, and promotion recommendations against the *same* budget on the *same* calendar; it forces HRBPs and leadership to calibrate those recommendations against each other before any employee is told anything; and it hands the comp committee a complete, pre-calibrated package to ratify — which is what the comp committee's charter actually requires them to do (see [chapter 05](./05-compensation-committee.md)).

The alternative — rolling adjustments outside the cycle — should be reserved for genuinely exceptional retention cases: a VP who has received a credible competing offer, an engineer whose comp has drifted materially below band because of a mis-levelled hire, an acquihire-adjacent retention package. Everything else waits for the cycle. The discipline of waiting is what makes the cycle meaningful.

## The purpose of an annual cycle

### One decision pass, not twelve

The cycle collapses what would otherwise be a continuous stream of comp conversations into a single window. Managers know that merit, equity, and promotion recommendations are due in a specific week. Employees know that the answer to "when will I hear about my raise" is a specific month. The CFO knows that the merit-budget hit lands in a specific pay period. The audit trail — covered in [documentation and audit trail](#documentation-and-audit-trail) below — is a bounded set of artefacts tied to a single cycle, not a scattered email history.

### Comp decisions precede the review conversation

The cycle runs *after* fiscal-year close and *before* performance-review conclusions are communicated. This ordering is deliberate. If a manager tells an employee "you are a top performer this year" and *then* goes to budget-allocation and calibration, the manager has effectively pre-committed to a comp outcome the budget may not support. Comp decisions must be locked — manager-recommended, HRBP-calibrated, leadership-reviewed, comp-committee-ratified — *before* the review conversation happens, so that the review conversation and the comp conversation can land together as a single, consistent message.

### Managers recommend; the committee ratifies

Managers do not *decide* comp in the cycle. Managers recommend; HRBPs calibrate; leadership reviews; the comp committee ratifies. The split exists because the two decisions the manager is uniquely qualified to make (how good was this person's year, and what should their trajectory be) are different from the decisions the corporation needs to make at the aggregate (budget consumption, pay-equity drift, exec comp, 409A implications). The annual cycle is the structural separation of those two decisions.

## Timing

### The default calendar — Q1 for a December fiscal-year-end

For a corporation whose fiscal year ends December 31, the canonical cycle runs in Q1: kickoff in early January once performance-review inputs are stable, manager recommendations due by early-to-mid February, HRBP calibration mid-February, leadership calibration late-February, comp-committee review in early March, communication to employees in mid-March, and grant notices filed through the equity-admin platform (Carta, Shareworks, Pulley) by late March.

### Shifting for other fiscal years

For a June fiscal-year-end, the cycle shifts into Q3; for a September fiscal-year-end, into Q4. The invariant is that comp-cycle kickoff lags fiscal-year close by roughly two to four weeks (long enough for financial-close numbers to stabilise, short enough that the performance-review signal is still fresh), and comp-committee ratification lands before the review conversations.

### The pre-S-1 shift to Q4

Pre-S-1 corporations frequently shift the comp cycle to Q4 even without changing the fiscal year, to align with proxy-season timing and the compensation disclosure obligations that attach once the corporation becomes an SEC registrant. The CD&A (Compensation Discussion and Analysis) in the proxy statement requires a stable prior-year comp record for the named executive officers; aligning the cycle to Q4 means the record is final before the proxy drafting window opens. <!-- needs-research: confirm current SEC guidance on CD&A record-stability expectations and the typical proxy-drafting timeline for a newly public corporation. -->

## Budget allocation

### Merit budget

The merit budget is a percent-of-base-payroll pool that funds all merit increases across the corporation, allocated down to each function. A commonly cited Series-A / Series-B merit-budget range is <!-- needs-research: confirm current merit-budget benchmarks against WTW (Willis Towers Watson), Mercer, PayScale, and Radford compensation surveys; a defensible historical range is roughly 3-5% of base payroll for US tech corporations in a non-inflationary year, with hot-market or inflationary years running higher. -->. The merit budget is set by the CFO and Head of People, approved by the comp committee, and allocated to each function based on headcount and base-payroll weight.

### Equity refresh budget

The equity refresh budget is a percent-of-fully-diluted pool authorised by the comp committee for the annual refresh programme. A commonly cited range at scale is <!-- needs-research: confirm current equity-refresh pool benchmarks; a defensible historical range is roughly 1-3% of fully diluted at Series-B through late stage, with IC and executive pools typically budgeted separately. -->. The sizing math — refresh grants as a percentage of original new-hire grant, scaled by level and performance — is covered in [chapter 03](./03-refresh-promotion-and-retention-grants.md); the cycle consumes the budget that chapter sizes.

### Promotion budget

The promotion budget is a derived number, not a top-down allocation: it is the sum, across all promotions ratified in the cycle, of (new-level base-salary target minus current base salary) plus any equity-promotion grant. The budget is pre-estimated during leadership calibration (based on the slate of promotion recommendations) and reconciled to actual at cycle close.

### Variable / bonus pool

For corporations with a target-bonus programme, the variable pool funds at target-bonus achievement when the corporation hits its planned performance level, adjusted up or down based on corporate performance against plan. Individual bonus payouts are then adjusted around the corporate factor based on individual performance rating. The bonus pool is approved by the comp committee as part of the same cycle, even if the pool is funded against a different performance period.

## Workflow

### Stage 1 — manager recommendations

Each people-manager submits merit, equity, and promotion recommendations for their direct reports against the budget allocation their function received. Recommendations are entered through comp tooling — Pave, Lattice, CompTool, Assemble, or HRIS-native modules (Rippling, Gusto, Workday). The tooling enforces budget bands, flags out-of-band recommendations, and surfaces the performance-review rating alongside each recommendation. The deadline for Stage 1 is typically four to six weeks before cycle close.

### Stage 2 — HRBP / Head of People review

The HRBP for each function calibrates against the manager recommendations and flags outliers: a merit recommendation materially outside the budget band, a promotion recommendation without the prerequisite performance-review rating (see [mod-107 chapter 02](../mod-107-performance-promotion-and-offboarding/02-promotion-architecture.md)), an equity refresh outside the policy band for the employee's level. Each outlier is resolved in a short conversation with the manager and the function leader before Stage 3 opens.

### Stage 3 — leadership / cross-function calibration

VP-level and C-suite review each function's recommendations in aggregate. The purpose is cross-functional calibration — a same-level IC in engineering and a same-level IC in GTM should see broadly similar merit and equity outcomes given broadly similar performance ratings. The finance partner validates budget consumption at this stage: are we on, over, or under the function's allocation, and if over, where is the offset coming from.

### Stage 4 — comp-committee review and approval

The Head of People and CFO prepare a materials pack for the comp committee: aggregate budget consumption, exec-comp recommendations line-by-line, promotion slate, equity-refresh grant list, pay-equity audit summary. Exec comp runs as a separate session with the CEO out of the room for the CEO-comp agenda item. Approvals are ratified at the committee and reported to the full board at the next board meeting. See [chapter 05](./05-compensation-committee.md) for the comp-committee operating norms.

### Stage 5 — communication

Compensation statements are delivered to employees — written documents stating new base, new target bonus, equity-grant notice if applicable, and any benefits changes. Communications are coordinated with the performance-review conversation so that the review and the comp message land together. Pay-transparency obligations vary by state — see [mod-103 chapter 03](../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md) for the pay-transparency architecture and [mod-103 chapter 08](../mod-103-employment-law-and-contract-design/08-state-law-variance.md) for the state-by-state matrix. Grant notices issue through the equity-admin platform at the same time or shortly after.

## Pay-transparency communications

The annual cycle is the moment at which the corporation's internal comp bands and its state-mandated external job-posting ranges must reconcile. If an engineer's new comp sits outside the band the corporation has been posting externally in CA, CO, WA, NY, or IL (and the growing list of other pay-transparency jurisdictions — defer the state-by-state list to [mod-103 chapter 08](../mod-103-employment-law-and-contract-design/08-state-law-variance.md)), the corporation has either an internal-equity problem, an external-posting problem, or both. The cycle is the forcing function to fix it; the HRBP calibration (Stage 2) and the pay-equity audit summary at the comp-committee session (Stage 4) are the mechanisms.

Internal-equity question answering — "my peer makes more than me, why" — is a predictable follow-on to the communication stage. The Head of People and the HRBPs should expect it, be prepared with band-and-rating language, and route edge cases to a formal pay-equity review rather than to one-off manager-level adjustments.

## Calibration norms and drift risks

### Tenure-anchored drift

Merit increases that accumulate year-over-year for tenure rather than for performance. The symptom is a long-tenured IC whose comp has drifted to the top of the band without a corresponding performance signal. The mitigation is explicit calibration — in Stage 2, HRBPs flag merit recommendations whose justification narrative is tenure-weighted rather than performance-weighted.

### Performance-anchored drift

The opposite failure mode — merit increases that collapse to the middle of the budget band regardless of performance rating, because managers find the differentiation conversation hard. Everyone gets 3%. The signal that the performance-review process is supposed to generate is destroyed on contact with the comp cycle. The mitigation is a required distribution — the budget band for a top performer must be meaningfully above the band for an average performer, and the HRBP flags any manager whose recommendations compress to the middle.

### Pay-equity drift

Same-level ICs who end up materially different on the comp band after several cycles, correlated with protected categories (gender, race, age, parental status). The annual cycle is where drift either compounds or gets corrected. The formal pay-equity audit — a statistical regression of comp against level, tenure, performance, and protected-category variables — is architected in [mod-106](../mod-106-compensation-architecture-and-total-rewards/) and is a required Stage-4 artefact for the comp committee.

## Grant notices and the 10b5-1 window

At the private-company stage, grant notices issue immediately after comp-committee ratification and are recorded in the equity-admin platform. At the post-IPO stage, grant issuance must align with the corporation's trading-window policy and any applicable Rule 10b5-1 plans for executives. Equity grants to insiders issued inside a blackout window are a disclosure and Section 16 reporting problem; the cycle calendar should be set with the trading-window calendar in mind, and the comp committee should ratify at a date that lands grant issuance inside an open window. <!-- needs-research: confirm current SEC Rule 10b5-1 amendments (as applicable) and typical trading-window structures for newly public corporations. -->

## Documentation and audit trail

Comp-cycle decisions are a document-retention category. The required artefacts for a cycle:

- Comp-committee meeting materials and minutes (see [chapter 05](./05-compensation-committee.md)).
- HRBP calibration notes — the outliers flagged in Stage 2 and their resolutions.
- Leadership-calibration notes — the cross-functional adjustments made in Stage 3.
- The final approved comp statements and grant notices as delivered to employees.
- The pay-equity audit summary presented to the comp committee.
- Budget-consumption reconciliation (plan vs. actual) at cycle close.

These artefacts are retained for SOX purposes (public corporations), for audit purposes (private corporations preparing for a financing or an exit), and for plaintiffs'-counsel-discovery purposes in the event of a pay-equity claim or wrongful-termination claim where comp decisions become evidence. Retention periods are set by the corporation's document-retention policy; the comp-cycle artefact bundle is treated as a single annual record.

## A worked example — Series-B corporation "Northfield Robotics," fiscal-year-end December 31

Northfield Robotics is a fictional Series-B corporation with ~140 employees, fiscal year ending December 31. The annual comp cycle runs:

- **Jan 10 — cycle kickoff.** Head of People publishes manager-recommendation templates in Pave. Finance confirms budget allocations by function. Comp philosophy and band reference materials are re-circulated to managers.
- **Feb 7 — Stage 1 deadline.** Manager recommendations due. The engineering function has 62 ICs and 8 managers; GTM has 38 and 5; product/design has 18 and 3; G&A has 22 and 4.
- **Feb 10 — Stage 2 HRBP calibration.** HRBPs review all recommendations against policy bands and the previous cycle's performance-review ratings. 14 outliers flagged across all functions; 11 resolved by Feb 17.
- **Feb 25 — Stage 3 leadership calibration.** VPs and C-suite walk the function-by-function slates. Three cross-functional adjustments made (two engineering ICs rated top-performer whose merit % was below the GTM top-performer band, one G&A promotion deferred to next cycle for insufficient performance-review signal). Finance validates budget consumption at 3.9% merit against the 4% allocation.
- **Mar 5 — Stage 4 comp-committee review.** Committee materials delivered 72 hours in advance. Exec-comp session with CEO out of the room for CEO-comp agenda. All recommendations ratified. Reported to full board at the Mar 12 board meeting.
- **Mar 15 — Stage 5 communication.** Comp statements delivered. Managers hold review-plus-comp conversations through Mar 19.
- **Mar 20 — grant notices filed in Carta.** All refresh and promotion grants issued, recorded, and acknowledged.

**Budget shape for the cycle.**

- Merit budget: <!-- needs-research: confirm against current WTW / Mercer / Radford Series-B benchmarks; the 4% figure above reflects a commonly cited historical range for US tech at Series-B in a non-inflationary year. --> 4% of base payroll.
- Equity refresh pool: <!-- needs-research: confirm against current Radford / Pave equity-refresh benchmarks for Series-B; the 2% figure above reflects a commonly cited historical range for fully-diluted refresh-pool consumption. --> 2% of fully diluted.
- Promotion slate: 10 promotions pre-allocated across functions based on the Stage-3 leadership-calibration slate; final slate ratified at Stage 4.

The entire cycle is 10 weeks from kickoff to grant-notice filing. Every artefact described in [documentation and audit trail](#documentation-and-audit-trail) is archived in the corporation's compliance folder with retention keyed to the cycle year.

## Summary

- The annual comp cycle converts performance-review conclusions into comp decisions in a single, repeatable, auditable pass that the comp committee ratifies. Rolling / ad-hoc adjustments outside the cycle are reserved for exceptional retention cases.
- Timing: the cycle runs after fiscal-year close and *before* performance-review conclusions are communicated, so comp decisions are locked when the review conversation happens. Default is a Q1 cycle for a December fiscal year; pre-S-1 corporations often shift to Q4 for proxy alignment.
- Budget allocation covers four pools: merit (percent of base payroll), equity refresh (percent of fully diluted, see [chapter 03](./03-refresh-promotion-and-retention-grants.md)), promotion (derived from the ratified promotion slate), and variable / bonus (funded against corporate performance).
- The workflow runs in five stages: manager recommendations, HRBP calibration, leadership / cross-function calibration, comp-committee review and approval (see [chapter 05](./05-compensation-committee.md)), and communication coordinated with the performance-review conversation and pay-transparency obligations ([mod-103 chapter 03](../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md), [mod-103 chapter 08](../mod-103-employment-law-and-contract-design/08-state-law-variance.md)).
- Active drift risks — tenure-anchored, performance-anchored, and pay-equity — are managed at the HRBP and leadership-calibration stages, with the pay-equity audit architected in [mod-106](../mod-106-compensation-architecture-and-total-rewards/).
- Comp-cycle decisions are a document-retention category: committee minutes, calibration notes, grant notices, and the pay-equity audit summary are retained for SOX, audit, and discovery purposes.
