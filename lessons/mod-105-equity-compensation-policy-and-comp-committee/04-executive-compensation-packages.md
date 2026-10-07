# 4. Executive compensation packages

> An executive package is not "base + stock" — it is a seven-piece instrument (base, bonus, equity, PSU overlay, severance, CoC acceleration, indemnification) and every piece is independently negotiable, independently taxed, and independently legally reviewable.

## Motivation

The common failure mode at Series-A and Series-B is to extend an executive offer that looks like an engineering offer with a bigger number — a base-salary field, an equity-grant field, and a "we'll give you severance if things go south, don't worry" verbal addendum. The person on the other side of the table runs a different playbook. A seasoned CFO / CRO / CPO / GC walks into the negotiation expecting a priced package across seven line items, each of which has a market comparable and a legal construct behind it.

The corporation that treats the exec offer as "base + stock" ends up (a) under-pricing the package against the market and losing the candidate on cash OTE, (b) over-pricing it on equity because that was the only lever anyone thought to pull, (c) agreeing verbally to severance and change-of-control terms that the corporation's own equity plan and standard documents cannot actually deliver, and (d) stacking double-trigger accelerations across the exec bench in a way that will blow up a § 280G parachute analysis three years later at the sale.

This chapter walks the full exec-package anatomy, flags where the numbers come from (and where you must call Compensia / Radford / Pave rather than invent them), and names the tax statutes — IRC § 162(m), IRC § 280G / § 4999, IRC § 409A — that constrain pre-IPO and post-IPO design. CoC equity policy architecture is deferred to [chapter 07](./07-change-of-control-equity-policy.md); exec severance architecture to [chapter 08](./08-executive-severance-and-release.md); SEC disclosure obligations to [chapter 09](./09-sec-reg-sk-item-402-disclosure.md).

## The EXEC-COMP shape

An executive package has seven components. Each is drafted and negotiated separately; each lives in a distinct document; each has an independent legal regime.

1. **Base salary.** The cash paycheck. The smallest component of the package by economic value for most C-suite roles.
2. **Target bonus.** Annual cash bonus expressed as a percentage of base, paid on MBO achievement and/or company-level KPIs.
3. **On-target earnings (OTE).** Base + target bonus. The number the candidate will state when asked "what's your current comp?"
4. **Equity grant.** New-hire grant of stock options or RSUs expressed as a percentage of fully diluted (or, post-IPO, as a target grant value in dollars translated to shares at grant-date FMV).
5. **Performance-share overlay.** PSUs (performance stock units) and/or MBO cash-and-equity grants that vest on company performance or individual-objective achievement. Appears pre-IPO at growth stage and becomes standard post-IPO.
6. **Severance.** Cash + benefits continuation + accelerated vesting payable on involuntary termination without cause (and, under a double-trigger construction, following a change of control).
7. **Change-of-control (CoC) acceleration.** Equity-vesting acceleration triggered by a CoC — single-trigger (CoC alone) or double-trigger (CoC plus qualifying termination within a defined window).

An eighth component — **indemnification and D&O** — is sometimes miscategorised as "legal paperwork." For an exec it is part of the package. See [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/) for the officer-appointment / D&O side.

Base, bonus, and equity sit in the offer letter and the equity-grant notice. Severance and CoC acceleration sit in an executive severance agreement (sometimes called a CIC agreement). The indemnification agreement is its own one-page document executed in parallel with officer appointment.

## Base and target bonus

### Target-bonus percentages by seat

Exec target bonus is sized as a percentage of base. The commonly cited ranges are:

- **VP-level seats** (VP Eng, VP Product, VP People, GC-at-VP-grade): target bonus of <!-- needs-research: confirm against Compensia / Radford / Pave 2025–2026 private-company exec surveys; a defensible band is 20–40% of base for most VP seats, higher for revenue-adjacent VPs. -->.
- **C-suite non-GTM** (CFO, COO, CPO, CTO, CHRO, GC-at-C-grade): target bonus of <!-- needs-research: confirm against Compensia / Radford exec surveys; commonly cited 40–60% of base for pre-IPO C-suite. -->.
- **CEO**: target bonus of <!-- needs-research: confirm against Compensia / Radford CEO surveys; hired-CEO target bonus is commonly 50–100% of base at growth-stage private; founder-CEO cash comp is a separate conversation driven by cap-table ownership. -->.
- **CRO / VP Sales (variable-heavy OTE).** The GTM leader's OTE is intentionally weighted toward variable comp — a 50/50 or 60/40 base-to-variable split is standard, with the variable portion gated on bookings / ARR / plan attainment. The variable half is itself a mix of commission (plan-driven) and MBO (strategic-objective-driven). <!-- needs-research: confirm current-market CRO base/variable split and the plan-attainment payout curve from Pave / RepVue / Compensia. -->

OTE is the headline number the candidate will negotiate against. The corporation should know its OTE band for each exec seat *before* opening the search, benchmarked against a specific survey, and should know what percentile of the band each offer is landing at.

### Benchmarking data sources

Three vendors dominate private-company exec comp benchmarking: **Compensia** (bespoke advisory + the Radford survey resale), **Radford** (survey direct), and **Pave** (real-time compensation-data platform aggregating customer payroll data). A Series-B+ corporation typically subscribes to one of the three; a Series-A corporation often buys a one-off benchmarking study from Compensia or a comp-advisory boutique when preparing a VP / C-suite search. The compensation committee reviews the benchmarking methodology at least annually (see [chapter 10](./10-compensation-committee-charter-and-cadence.md)).

## Equity grant sizing by seat

Exec equity grants are sized as a percentage of fully diluted (pre-IPO) or as a target dollar value translated to shares at grant-date FMV (post-IPO). The sharp cliff the hiring team must understand:

**Founder-CEO equity is a cap-table dimension, not a comp-table dimension.** A founder-CEO holding 25–45% of fully diluted at Series-A is holding that stake because they founded the company, not because the comp committee priced the position at 25–45% of fully diluted. The hired CEO who replaces or succeeds the founder-CEO is priced *against the exec market*, not against the founder's cap-table share.

Hired-exec grant bands commonly cited for Series-B / C private companies (**flag every number here**):

- **Hired CEO**: <!-- needs-research: Compensia / Radford exec-grant surveys; commonly cited 3–8% of fully diluted at the hire moment, with refresh grants on top. -->
- **CFO**: <!-- needs-research: commonly cited 1–3% of fully diluted. -->
- **COO**: <!-- needs-research: commonly cited 1–3% of fully diluted; often paired with the CEO on compensation and sometimes exceeds CFO. -->
- **CRO / VP Sales**: <!-- needs-research: commonly cited 0.75–2% of fully diluted; variable-comp heavier so equity sometimes lower than non-GTM C-suite. -->
- **CPO / CTO / Chief Scientist**: <!-- needs-research: commonly cited 1–2.5% of fully diluted at the hire moment, depending on how technical the market defines the role. -->
- **VP Eng / VP Product (non-C-suite)**: <!-- needs-research: commonly cited 0.4–1.0% of fully diluted. -->
- **GC**: <!-- needs-research: commonly cited 0.4–1.0% of fully diluted at Series-B; higher if GC also runs corporate development. -->

Refresh grants (annual or biannual) layer on top of the new-hire grant. The policy for refresh cadence and sizing is the comp committee's call (see [chapter 06](./06-equity-refresh-and-promotion-grants.md)).

## Performance-share overlay

PSUs and MBO grants are an *overlay* on the time-based new-hire grant, not a replacement for it.

### PSUs (performance stock units)

PSUs vest on company-level performance measured over a performance period (typically three years for public companies). Common performance metrics:

- **Revenue or ARR growth** against a plan target or against a peer group.
- **EBITDA / operating margin** against plan.
- **Relative TSR** (total shareholder return) against a defined peer index — most relevant post-IPO.

Pre-IPO, PSUs appear at growth-stage when the compensation committee wants to tie a portion of the CEO / CFO / CRO package to a specific performance outcome the board can measure. Post-IPO, PSUs are the norm — ISS and Glass Lewis both prefer performance-vesting over pure time-vesting for exec grants (see "ISS / Glass Lewis" section below). Pre-IPO corporations design the PSU construct knowing it will be scrutinised at IPO under the compensation discussion-and-analysis (CD&A) disclosure in SEC Reg S-K Item 402 (see [chapter 09](./09-sec-reg-sk-item-402-disclosure.md)).

### MBOs (management by objectives)

MBO grants vest on *individual* objective achievement — a defined set of personal goals set at the start of the performance period, reviewed by the CEO (for the CEO's direct reports) or the compensation committee (for the CEO). MBOs are typically cash and sometimes equity. The construct is simpler than PSUs but has a weaker tie to shareholder-visible performance.

## Severance

Market-standard exec severance for pre-IPO private-company execs:

- **6–12 months of base salary** paid as salary continuation or lump sum.
- **Target bonus for the year** paid pro-rata or in full.
- **Benefits (COBRA) continuation** for the severance period.
- **Accelerated vesting** of some or all unvested equity (the amount and the trigger are the subject of the CoC-acceleration section below).

CEO severance is typically at the top of the range (12 months); VP severance at the bottom (6 months). Severance is paid *subject to a release of claims* — the exec signs a general release in exchange for the severance package. Release architecture, revocation periods under ADEA / OWBPA, and 409A-compliant payment timing are all covered in [chapter 08](./08-executive-severance-and-release.md).

### IRC § 409A six-month-delay rule

Post-IPO, severance for a "specified employee" (broadly, a top-50 officer of a public company) is subject to the **IRC § 409A(a)(2)(B)(i) six-month-delay rule** — separation payments that constitute deferred compensation under § 409A cannot be paid until six months after separation. Pre-IPO this rule does not bite (the corporation has no public-company specified employees), but the severance agreement is drafted *now* to be compliant at IPO so the corporation does not have to re-paper the exec bench at the S-1 moment. See 26 C.F.R. § 1.409A-1(i) for the specified-employee definition and § 1.409A-3(i)(2) for the delay-rule mechanics.

## Change-of-control acceleration

### Single-trigger vs. double-trigger

- **Single-trigger acceleration.** Vesting accelerates on the change of control itself, independent of whether the exec is terminated. Market-disfavoured outside the hired-CEO exception. ISS and Glass Lewis both flag single-trigger acceleration as a "problematic pay practice." Buyer-side M&A diligence will discount the headline deal value for single-trigger constructs because the executive is being paid to leave at close rather than stay.
- **Double-trigger acceleration.** Vesting accelerates only if *both* (a) a change of control occurs *and* (b) the exec is terminated without cause or resigns for good reason within a defined window (typically 12 or 18 months post-closing). This is the market standard for CFO / COO / CPO / GC / VP seats.

The hired CEO sometimes negotiates **modified single-trigger** or **full single-trigger** acceleration — this is a case-by-case negotiation and sits with the compensation committee. Policy details, "good reason" definitions, cutback vs. gross-up language, and the mechanics of acceleration for performance-vesting grants are all in [chapter 07](./07-change-of-control-equity-policy.md).

## IRC § 162(m) — the $1M deductibility cap

**IRC § 162(m)(1)** disallows the corporate income-tax deduction for compensation paid to a "covered employee" of a publicly held corporation in excess of $1M in a taxable year. "Covered employee" includes the CEO, CFO, and the three other highest-paid officers (and, under the TCJA 2017 amendments, once covered always covered).

**Pre-IPO**: a private C-corp is *not* subject to § 162(m) — the "publicly held corporation" trigger has not fired. Exec cash comp above $1M is fully deductible.

**At IPO**: § 162(m) kicks in, and the $1M cap bites immediately on exec cash comp. The TCJA 2017 amendments eliminated the former "performance-based compensation" exception (IRC § 162(m)(4)(C) as it existed pre-TCJA), so there is no longer a path to deduct performance-based cash or equity comp above the $1M cap. Grandfathering under TCJA § 13601(e)(2) survives only for compensation payable under a *written binding contract* in effect on November 2, 2017 and not materially modified thereafter — a narrow and shrinking set.

**Practical implication for pre-IPO design.** Build the exec packages now knowing that at IPO the $1M cap will apply and that above-$1M cash comp is non-deductible. The exec can still be paid above $1M — the corporation just loses the deduction. The compensation committee's job is to make the trade-off deliberately rather than discover it at the first post-IPO 10-K.

## IRC § 280G and § 4999 — golden parachutes

**IRC § 280G** disallows the corporate deduction for "excess parachute payments" and **IRC § 4999** imposes a 20% excise tax on the recipient. The analysis is triggered on a change of control when "parachute payments" (CoC-contingent compensation) to a "disqualified individual" (broadly, an officer, shareholder, or highly compensated individual) exceed **3× the individual's "base amount"** (the five-year average W-2 compensation ending in the year preceding the CoC). If the 3× threshold is breached, the entire amount in excess of 1× the base amount is treated as an excess parachute payment.

**Private-company 280G cleanse.** **IRC § 280G(b)(5)(A)(ii)** provides a private-company exception: a corporation whose stock is not readily tradeable on an established securities market can "cleanse" parachute payments by obtaining the approval of more than 75% of the voting power of disinterested shareholders, after adequate disclosure to those shareholders. The 280G cleanse is a standard transaction-closing workflow at a private-company sale — see **`startup-exit-curriculum`** for the transaction-execution playbook.

**Policy design implication for mod-105.** The compensation committee should design exec packages so that CoC payments do not *inadvertently* breach 3× base amount across the exec bench — in particular, do not stack full single-trigger acceleration across every officer, do not promise tax gross-ups for § 4999 excise tax (ISS and Glass Lewis flag gross-ups as a problematic pay practice), and consider "cutback" provisions (reduce the parachute payment to 2.99× base amount if that produces a better net-after-tax outcome for the exec, i.e., the "best-net" or "modified-cutback" construct). Transaction-level 280G *execution* belongs to `startup-exit-curriculum`; mod-105 covers the *policy* design that keeps the transaction-level 280G workflow tractable.

## ISS and Glass Lewis — "say on pay" and the pre-IPO defensibility test

**Say on pay** — the shareholder advisory vote on exec compensation required by Dodd-Frank § 951 (codified at 15 U.S.C. § 78n-1) — applies to public reporting companies. Pre-IPO corporations do not run the vote. But the IPO prospectus (S-1) will disclose the exec compensation program in full under SEC Reg S-K Item 402 (see [chapter 09](./09-sec-reg-sk-item-402-disclosure.md)), and the first post-IPO proxy will put the program up for a say-on-pay vote within the SEC-prescribed window.

ISS (Institutional Shareholder Services) and Glass Lewis publish annual voting policies that institutional holders rely on to form their say-on-pay vote recommendation. The pre-IPO corporation designs its exec program to be *ISS-defensible at IPO*. The high-leverage policy areas:

- **Pay-for-performance alignment.** TSR vs. CEO realised pay. ISS runs quantitative screens (the "quant pay-for-performance" test) that compare the subject corporation to a peer group. <!-- needs-research: confirm the current ISS pay-for-performance quantitative screens — Relative Degree of Alignment (RDA), Multiple of Median (MOM), Pay-TSR Alignment (PTA) — against the latest ISS Benchmark Policy. -->
- **Problematic pay practices.** Excessive severance (over 3× base + bonus is a red flag), single-trigger CoC acceleration, § 4999 excise-tax gross-ups, excessive perks, repricing of underwater options without shareholder approval.
- **Equity plan burn-rate, overhang, and dilution tests.** ISS runs a quantitative burn-rate test and an "equity plan scorecard" (EPSC) when the corporation seeks shareholder approval of a new or amended equity plan. <!-- needs-research: confirm current ISS EPSC thresholds and burn-rate benchmarks against the latest ISS US Equity Compensation Plans FAQ. -->

Pre-IPO: assume these policies will be enforced at the first post-IPO proxy. Design the exec program accordingly.

## Exec-offer package authoring — the document stack

A fully priced exec offer is five documents, not one:

1. **Offer letter.** Base, target bonus, OTE, start date, title, reporting line, at-will statement, conditions precedent (background check, I-9, references, where applicable immigration, board approval of the hire for a C-suite seat).
2. **Equity-grant notice.** Share count, grant date, vesting schedule, exercise price (for options), early-exercise permission (if any), post-termination exercise window.
3. **Executive severance agreement.** Severance amount and trigger, release-of-claims requirement, § 409A-compliant payment timing, good-reason definition, change-of-control definition. Full architecture in [chapter 08](./08-executive-severance-and-release.md).
4. **CoC addendum (or CIC agreement).** Acceleration construct (single vs. double trigger), acceleration percentage, performance-grant treatment, § 280G cutback or best-net language. Full architecture in [chapter 07](./07-change-of-control-equity-policy.md).
5. **Indemnification agreement.** Officer indemnification obligations, advancement of expenses, D&O insurance coverage reference. See [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/) for the officer-appointment and D&O interface.

The hiring workflow is in [`../mod-104-hiring-onboarding-and-hr-operations/08-executive-hiring-playbook.md`](../mod-104-hiring-onboarding-and-hr-operations/08-executive-hiring-playbook.md). The compensation-committee approval of the full exec package is in [chapter 10](./10-compensation-committee-charter-and-cadence.md).

## A worked example — VP Sales (CRO) offer at a Series-B SaaS company

**The corporation.** "Lintelmetric, Inc.," a fictional Series-B SaaS company, 110 employees, ARR run-rate ~$18M, just closed a $45M Series-B at a $220M post-money. Hiring a first full CRO (previously the founder-CEO was running sales). The board compensation committee has approved the package envelope; the final offer is being drafted by the Head of People in consultation with outside comp counsel.

**The candidate.** Senior VP of Sales from a $120M-ARR competitor. Current OTE ~$550k (60/40 split), restricted-stock position worth low seven figures, interviewing with three Series-B companies.

**The offer package.**

- **Base: $320k.** Benchmarked at the <!-- needs-research: confirm against Compensia / Pave 2025–2026 CRO survey; the band for CRO at $15M–$30M ARR Series-B is commonly cited around $280k–$360k base. --> percentile for a Series-B CRO.
- **Target variable: $213k.** 60/40 base/variable split <!-- needs-research: confirm current-market CRO base/variable split; 60/40 is commonly cited for Series-B SaaS CROs but 50/50 is also market. -->, with 70% commission plan + 30% MBO. Full OTE: $533k.
- **Equity grant: new-hire grant of <!-- needs-research: confirm against Compensia Series-B exec-grant table; commonly cited CRO new-hire grant is 0.75–1.5% of fully diluted at the hire moment. -->% of fully diluted,** structured as ISOs to the § 422(d) $100k/year limit and NSOs above, 4-year vest with a 1-year cliff, exercise price = § 409A FMV at grant date.
- **Performance overlay: MBO grant of $75k cash** tied to three objectives set jointly with the CEO (hiring the first two sales directors, delivering an ARR plan, standing up a revenue-ops function) — no PSU overlay at this stage because the corporation is pre-IPO and the comp committee is deferring PSU adoption to Series-C.
- **Severance: 9 months of base + target bonus + 9 months of COBRA + 12 months of accelerated vesting** on involuntary termination without cause (also triggered on resignation for good reason). Release of claims required. § 409A-compliant payment timing.
- **CoC acceleration: double-trigger, 100% of unvested equity**, on a change of control plus involuntary termination (or good-reason resignation) within 18 months post-closing. § 280G cutback: "best-net" — reduce payments to 2.99× base amount if net-after-tax outcome to exec improves. No § 4999 gross-up.
- **Indemnification agreement** executed in parallel with CRO appointment as a Section 16 officer (effective at IPO) and as an officer under Delaware General Corporation Law § 145 pre-IPO.

**Document stack delivered to candidate.** Offer letter, equity-grant notice (to be issued post-start-date on board approval of the grant), executive severance agreement, CoC addendum, indemnification agreement. All five reviewed by outside employment counsel and outside corporate counsel; compensation committee minutes record approval of the full package envelope.

## Summary

- The executive package is a seven-piece instrument — base, target bonus, equity, PSU/MBO overlay, severance, CoC acceleration, indemnification. Each piece has an independent legal regime and should be designed and negotiated separately.
- OTE is the headline negotiation number for most execs; CRO / VP Sales OTE is variable-heavy (50/50 or 60/40 base/variable) and gated on bookings / ARR / plan attainment. Hired-exec equity is sized against Compensia / Radford / Pave exec-grant tables, not against founder cap-table share.
- Pre-IPO C-corps are not subject to IRC § 162(m)'s $1M deductibility cap, but the cap bites at IPO and the TCJA 2017 performance-based-comp exception is gone — design exec packages mindful of post-IPO deductibility. IRC § 280G parachute analysis is a routine CoC workflow; the compensation committee's policy job is to avoid inadvertently stacking double-trigger accelerations into a § 280G trip-wire, and the private-company § 280G(b)(5)(A)(ii) cleanse requires 75% disinterested-shareholder approval at the transaction.
- IRC § 409A(a)(2)(B)(i) imposes a six-month delay on separation payments to "specified employees" post-IPO — pre-IPO severance documents should be drafted to be compliant now so the corporation does not re-paper at IPO.
- ISS and Glass Lewis "say on pay" voting policies apply post-IPO, but the pre-IPO corporation designs the exec program to be ISS-defensible at IPO — pay-for-performance alignment, no problematic pay practices (excessive severance, single-trigger acceleration, § 4999 gross-ups), equity plan burn-rate / overhang / dilution within the ISS EPSC bands. Policy specifics refresh annually; confirm against the current ISS and Glass Lewis policy documents.
- The exec offer is a five-document stack — offer letter, equity-grant notice, severance agreement, CoC addendum, indemnification agreement. CoC equity policy details live in [chapter 07](./07-change-of-control-equity-policy.md); severance architecture in [chapter 08](./08-executive-severance-and-release.md); SEC Reg S-K Item 402 disclosure in [chapter 09](./09-sec-reg-sk-item-402-disclosure.md); comp committee charter and cadence in [chapter 10](./10-compensation-committee-charter-and-cadence.md). Transaction-level § 280G execution belongs to `startup-exit-curriculum`.
