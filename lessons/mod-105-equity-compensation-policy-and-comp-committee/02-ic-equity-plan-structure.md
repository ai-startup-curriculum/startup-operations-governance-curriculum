# 2. The IC equity-plan structure

> An IC equity grant is not one decision; it is a bundle of six — vehicle, schedule, cliff, exercise mechanics, tax election window, and acceleration treatment. Getting any of them wrong is cheap to the recruiter and expensive to the corporation.

## Motivation

The grant-sizing conversation ([chapter 01](./01-grant-guidelines-by-level-and-function.md)) answers "how many shares." This chapter answers "shares in what *form*, vesting on what *schedule*, exercisable under what *mechanics*, taxed under what *regime*, and treated how on *termination* and *change of control*." Those decisions do not usually show up in a candidate's offer-close conversation. They show up two to seven years later, at the Series-C secondary tender, at the IPO S-1 drafting session, at the acquisition closing-balance-sheet true-up, and at the ex-employee's post-termination exercise window.

Getting the plan-structure wrong is expensive in specific and recurring ways:

- **ISO over-grant above the $100k vesting-value limit** (IRC § 422(d)) that nobody tracked at grant time — the overflow quietly becomes NSO, the employee discovers it years later when the tax treatment surprises them, and the corporation's compensation records disagree with the employee's broker records at exercise. The corporation then pays counsel to reconcile the stack.
- **A single-trigger-vested private-company RSU** granted to a senior engineer at Series-C — the shares vest on time, § 409A requires income recognition at vest, the employee owes ordinary-income tax on illiquid shares they cannot sell, and the corporation has to run a tax-equalisation or sell-to-cover programme that it did not budget for. This is the "phantom income" problem that drove the market shift to double-trigger private-company RSUs ("PCRSUs").
- **A missed 30-day § 83(b) election window** after an early-exercise — the employee loses the ability to start the capital-gains clock and the QSBS clock at exercise, and the entire economic value of the early-exercise programme disappears for that employee. The corporation gets the "why did my package become worse than my peer's" email.
- **A badly drafted post-termination exercise window** — a 90-day window that converts ISO to NSO on day 91 (IRC § 422(a)(2)) without the employee understanding the switch, or a 10-year PTEW that creates § 409A problems if structured as a repriced option. Either generates a litigation surface.
- **An inconsistent acceleration provision** across the IC population — some grants with double-trigger acceleration (CoC plus involuntary termination), some without, no written rubric for who got what. At the next acquisition, the acquirer's counsel audits the cap table and the corporation discovers it has three different grant forms in circulation.

The equity economics (dilution, waterfall, 409A methodology, Rule 701 limits) belong to `startup-finance-fundraising-curriculum`. The CoC transaction mechanics belong to `startup-exit-curriculum`. This chapter is about the *plan-structure design decisions* an operator and comp committee own.

## Vesting-schedule architecture

### The 4-year / 1-year-cliff market standard

The dominant US venture-backed startup grant structure is a four-year total vesting period with a one-year cliff: no shares vest for the first 12 months of service, 25% vest on the one-year anniversary, and the remaining 75% vest monthly (36 equal monthly tranches) thereafter. This structure is so dominant that any deviation requires an explicit explanation to the candidate and to the comp committee.

The economics are a compromise. The one-year cliff screens out early-attrition hires who should not take any equity with them. The 36-month monthly tail after the cliff creates a continuous retention gradient — every month the employee stays, a visible chunk vests. The 48-month total period aligns the IC's economic horizon with a plausible Series-B through Series-D arc.

### Alternative schedules

Alternative schedules appear in three recurring contexts:

- **Five-year vesting.** Appears in a small number of post-2020 companies (publicly, Stripe and some unicorn peers) that want a longer retention horizon on senior IC and manager hires. The one-year cliff typically remains; the back-end is 48 months of monthly vesting rather than 36. Rare at seed and Series-A; more common at late-stage private companies with long IPO horizons.
- **Back-loaded vesting (10/20/30/40 or similar).** Senior-IC and executive grants sometimes vest in rising annual tranches rather than evenly. Rare at IC level; more common for executive grants (see [chapter 04](./04-executive-compensation-packages.md)).
- **Performance-vesting (PSUs / performance options).** Vesting conditioned on a specified corporate performance metric — ARR milestone, product-launch milestone, revenue multiple at IPO, or a specific stock-price hurdle in a public-company sense. Rare for IC at private companies because the metric is hard to design and administer; appears in executive grants and in some senior-engineering retention grants at late-stage pre-IPO companies.

The practitioner default for IC: 4-year monthly vest after a 1-year cliff. Any deviation is a comp-committee decision captured in the grant resolution.

### Monthly vs. quarterly vs. annual vesting after cliff

Monthly vesting after the cliff is the modern default. Quarterly vesting (vesting on each quarter-anniversary) is common at a few European-headquartered startups and some older US plans. Annual vesting (one tranche per anniversary, no interim) creates a strong incentive to stay through each anniversary — but also a strong incentive to leave the day after, and most comp committees have moved away from pure annual vesting for IC grants.

## Cliff mechanics

### The one-year cliff and the "no partial credit" default

The one-year cliff means that an employee who leaves on day 364 of service — voluntarily or involuntarily — forfeits 100% of the grant. On day 365, 25% vests in a single tranche. The economics are deliberately binary: the cliff is a retention filter, not a retention gradient.

### Cliff treatment on involuntary termination

The default plan-document language forfeits the entire grant if the employee's service ends before the cliff. A small number of plans provide for pro-rata vesting through the service date if termination is involuntary and without cause ("good leaver" treatment), typically with the corporation's board or comp committee retaining discretion. This is uncommon at the IC level and more common for senior / executive hires with negotiated terms (see [chapter 04](./04-executive-compensation-packages.md)).

A frequent operational error: an IC who is terminated without cause at month 11 is told at offer-letter time "we have standard vesting" but neither the plan document nor the grant notice spells out the involuntary-termination cliff treatment. The employee asks for pro-rata credit at exit; the corporation says "the plan is clear" but the plan is actually silent and the comp committee has discretion. Resolving this at exit creates a severance negotiation the corporation did not plan for. The fix: the plan document and grant notice should spell out cliff-forfeiture explicitly, and the comp committee should have a written rubric for when, if ever, it exercises its discretion to accelerate past the cliff.

### Cliff interaction with promotion grants

A promotion grant ([chapter 03](./03-refresh-promotion-and-retention-grants.md)) issued to a 15-month-tenured employee usually carries its own one-year cliff from the promotion-grant date, not from the employee's original start date. The practitioner's choice is whether to (a) honour the fresh cliff and risk the employee feeling the promotion grant is "less generous than it looks," (b) back-date the cliff to the original hire date (which creates a partial-immediate-vest at grant), or (c) adopt a plan convention that promotion / refresh grants vest monthly from the grant date with no fresh cliff, since the retention-filter purpose of the cliff is already satisfied by the original grant.

Most mature comp-committee practice is option (c) — refresh and promotion grants vest monthly from the grant date, no fresh cliff — explicitly documented in the plan or in a comp-committee resolution.

## ISO vs. NSO vs. RSU per level per country

The vehicle choice is the first fork in grant design. It is driven by employee tax residency, grant size relative to the ISO limit, and corporate stage.

### Incentive stock options (ISOs) — IRC § 422

ISOs are a US-tax-code-created option vehicle (IRC § 422) available only to employees of a US corporation (or a US subsidiary of a non-US parent, subject to specific structure rules). Non-employee directors, consultants, and contractors cannot receive ISOs.

**Tax benefits.** The ISO holder pays no ordinary income tax at exercise. If the holder meets the dual holding requirement — holding the shares for at least two years from the grant date *and* at least one year from the exercise date — the entire gain between the exercise price and the sale price is taxed as long-term capital gain (currently 20% top federal rate plus 3.8% net investment income tax). If either holding requirement is missed, the gain is treated as a "disqualifying disposition" and the spread at exercise is recharacterised as ordinary income.

**AMT exposure.** The spread between exercise price and fair market value at exercise is a preference item for the alternative minimum tax (26 U.S.C. § 56(b)(3)). An employee who exercises deep-in-the-money ISOs can trigger a material AMT liability in the year of exercise, long before any sale produces cash. The AMT liability is a frequent source of surprise and litigation; the corporation's practitioner default is to put an AMT-warning paragraph in every option-exercise package.

**The $100k vesting-value limit — IRC § 422(d).** The aggregate fair market value of stock (determined at grant date) with respect to which ISOs are exercisable for the first time by an employee during any calendar year cannot exceed $100,000. The excess is treated as an NSO. The limit is applied to the *vesting schedule*, not to the grant size — a $400k-at-grant grant vesting ratably over four years keeps $100k/year inside the ISO envelope; a $400k grant with first-year full vest keeps $100k inside and $300k outside. The ordering rules (26 C.F.R. § 1.422-4) apply the limit chronologically to the order in which options first become exercisable in the year.

**Post-termination 3-month rule.** IRC § 422(a)(2) requires the ISO holder to exercise within three months of termination of employment to preserve ISO status (12 months in the case of disability). The 90-day post-termination exercise window ("PTEW") commonly cited in grant notices is the ISO-preserving window. Any exercise after that window is an NSO exercise regardless of what the grant notice calls the option.

**The ISO disqualification pattern on post-termination extension.** Some corporations offer extended PTEWs (e.g., 10-year post-termination exercise, matching the option term) as a candidate-friendly feature. The extension automatically disqualifies the option as an ISO on day 91 of the extension, converting it to NSO treatment for tax purposes. This is a legitimate design choice — the corporation is accepting NSO treatment in exchange for the retention and recruiting benefit of a longer window — but it must be disclosed and understood.

### Non-qualified stock options (NSOs)

NSOs are the "everything else" option vehicle. The holder pays ordinary income tax on the spread between exercise price and FMV at exercise (IRC § 83(a)); the corporation gets a corresponding compensation-expense deduction (IRC § 83(h) subject to the deduction limits of IRC § 162(m) for executives). Subsequent gain is capital gain if the holder holds the shares.

NSOs are typically used in three contexts:

- **ISO overflow.** Grants exceeding the IRC § 422(d) $100k vesting-value limit for the year — the excess is NSO.
- **Non-employee grants.** Advisors, consultants, directors, contractors — none are ISO-eligible.
- **Post-termination exercise extensions.** As described above.

NSOs are also the default option vehicle for non-US employees because ISOs are not available to them.

### Restricted stock units (RSUs)

RSUs are a promise to deliver shares (or cash equivalent) at a future vest / settlement date. The holder owes ordinary income tax at settlement (not grant). At a public company, RSUs are the dominant equity vehicle because the ordinary-income-at-vest problem is solved by same-day sale to generate the cash to pay the tax ("sell-to-cover").

At a private company, time-only-vested RSUs create the phantom-income problem described below, and the modern market solution is double-trigger PCRSUs.

### Country selection

- **US employees.** ISO up to the $100k vesting-value limit, NSO above. Early-stage startups default ISO-first; late-stage private companies with liquidity on the horizon often shift to RSUs for new hires. See [chapter 03](./03-refresh-promotion-and-retention-grants.md) for the stage-based vehicle shift.
- **UK employees.** The Enterprise Management Incentive (EMI) scheme is the HMRC-approved tax-advantaged option scheme for qualifying companies (gross assets under £30M, fewer than 250 employees, qualifying trades). EMI options receive significant capital-gains-treatment benefits and are a near-automatic choice for UK employees of qualifying companies. Non-qualifying companies grant plain unapproved options (equivalent to US NSOs). <!-- needs-research: confirm current EMI qualifying thresholds and any post-2024 HMRC updates to the EMI regime. -->
- **Canadian employees.** The Canadian stock option tax regime distinguishes "qualified" from "non-qualified" options; the 2021 federal budget introduced a $200,000 annual qualifying-vest threshold similar in spirit to the US ISO $100k limit. <!-- needs-research: confirm current Canadian stock-option tax rules, the $200k annual vesting threshold, and CCPC-specific treatment. -->
- **EU employees.** Highly jurisdiction-specific. Germany (phantom-equity / "virtuelle Mitarbeiterbeteiligung" has historically dominated because of the dry-income problem at vest; the 2024 Future Financing Act reforms were intended to improve the real-equity regime). France (BSPCE for qualifying companies, otherwise plain options with specific tax regimes). Netherlands, Spain, Italy, Portugal — each has its own regime. <!-- needs-research: compile current-year summaries of the German Future Financing Act (Zukunftsfinanzierungsgesetz) 2024 implementation, French BSPCE qualifying rules, and Dutch stock-option tax reform. -->

The international vehicle choice is a per-country workstream requiring local counsel and local payroll support (see `mod-113-international-expansion-and-global-workforce` once that module is live).

## Private-company RSUs and the double-trigger pattern

### Why time-only-vested private-company RSUs break

A time-only-vested RSU vests on a calendar schedule and settles at vest. At settlement, the holder owes ordinary-income tax on the fair market value of the shares (IRC § 83(a); 26 C.F.R. § 1.83-6). At a public company this is manageable — the holder sells enough shares at settlement to cover the tax. At a private company the shares are illiquid, there is no public market, and the holder owes tax on paper gains without any way to generate cash.

The 409A implications are worse: a time-only-vested RSU with settlement at vest at a private company may be treated as deferred compensation under IRC § 409A, with the attendant 20% additional tax plus interest penalty on non-compliance. The industry workaround is to vest and settle promptly, which triggers the dry-income problem.

### The double-trigger structure

The modern private-company RSU ("PCRSU") solves both problems by requiring two vesting conditions: (a) a time-based service requirement (typically 4-year monthly vest after a 1-year cliff — same shape as options), *plus* (b) a performance-based liquidity-event condition. The RSU does not settle, and no ordinary-income tax is owed, until both conditions are satisfied.

The second trigger is typically defined as the earlier of (a) an IPO or specified public-market registration event, (b) a change of control (acquisition / merger), or (c) a specific liquidity event defined in the plan document.

The structure solves the phantom-income problem (no tax until there is actual liquidity) and the § 409A problem (the performance condition is a substantial risk of forfeiture that defers the compensation).

### The 7-year expiration risk

The second trigger cannot be *open-ended indefinitely* without creating § 409A problems. The practitioner solution is to cap the time-based component at 7 years from the grant date — if the second trigger has not occurred by then, the RSU expires. This is the "7-year expiration" risk that late-stage private-company employees discover when the IPO slips. The expiration causes the time-vested portion to be forfeited.

Comp-committee discipline: at Series-C and beyond, run a quarterly scan of the earliest-granted PCRSUs against the 7-year expiration clock, and brief the committee on any grants within 18 months of expiration. The remediation options — grant extensions, special liquidity programmes, cash bonuses — are all expensive, and the lead time to plan them is material.

### The Carta PCRSU documentation pattern

Carta publishes template plan documents and grant notices for PCRSUs that have become close to a de facto industry standard. <!-- needs-research: confirm the current state of the Carta PCRSU template suite and whether the industry has consolidated on a single documentation pattern or has multiple co-existing patterns (e.g., Carta vs. Shoobx / Fidelity Private Shares vs. bespoke counsel drafts). -->

## Early-exercise programmes

### What early exercise is

An early-exercise programme permits the option-holder to exercise *unvested* options. The holder pays the exercise price for all exercised-but-unvested shares and receives shares subject to a repurchase right in favour of the corporation. If the holder leaves before the shares vest, the corporation repurchases the unvested shares at the original exercise price.

The economic rationale is tax-side: by exercising early at a low exercise price (ideally when the exercise price equals FMV, so the spread is zero), the holder starts (a) the capital-gains clock for subsequent appreciation, and (b) the five-year QSBS clock under IRC § 1202.

### The IRC § 83(b) election

The § 83(b) election (IRC § 83(b); 26 C.F.R. § 1.83-2) is the mechanism that makes early exercise work. By filing an 83(b) election within **30 days** of the early exercise, the holder elects to be taxed on the spread between exercise price and FMV at the time of exercise rather than at the time the forfeiture-right lapses (vest). If the exercise price equals FMV at the time of exercise, the taxable spread is zero — the 83(b) election costs nothing to file and starts both the capital-gains and QSBS clocks running.

The 30-day deadline is strict. There is no cure for a missed deadline. The practitioner default: the corporation's equity administrator sends the holder a pre-filled 83(b) form and a certified-mail label within 24 hours of exercise, and tracks confirmation of filing.

### Forfeiture-right structure that preserves ISO qualification

The repurchase right must be structured to preserve ISO qualification. The relevant rules (26 C.F.R. § 1.422-2 and § 1.421-1) require that the shares, once exercised, be shares of the corporation (not a mere contractual right), and that the forfeiture provision not disqualify the option as an ISO. The practitioner default is to grant the option as an ISO, permit early exercise of the ISO, impose a corporation repurchase right at the original exercise price on termination before vest, and have counsel confirm each step preserves ISO status.

### When early-exercise programmes appear

Early-exercise programmes almost always appear at pre-Series-B startups, where the FMV (and therefore the exercise price for new grants) is still low enough that the economic tax-side benefit is meaningful. By Series-B the FMV has typically risen enough that the up-front exercise cash cost outweighs the tax deferral benefit for most employees. The programme is often sunset formally at Series-B or discontinued informally by the corporation ceasing to approve early-exercise requests.

The *economic analysis* of whether an early-exercise is a good decision for a specific holder — exercise cost, AMT exposure, probability of vest, QSBS five-year hold — is covered in `startup-finance-fundraising-curriculum` under the tax-preference-economics chapter. The *plan-structure decision* — whether to offer the programme at all, and how to document it — is the comp-committee's.

## QSBS-eligible planning — IRC § 1202

### The three gating tests

Qualified Small Business Stock (QSBS) treatment under IRC § 1202 permits an individual holder to exclude a portion of federal capital-gains tax on the sale of qualifying stock. The three gating tests:

- **Aggregate-gross-assets test.** At the time of issuance of the stock, the corporation's aggregate gross assets must be less than $50M (IRC § 1202(d)). Once a corporation crosses the $50M AGA line, newly issued stock is permanently ineligible for QSBS. Stock issued before the AGA line remains eligible — the line is *per issuance*, not per corporation.
- **Five-year holding period.** The holder must hold the stock for at least five years before sale to qualify for the gain exclusion (IRC § 1202(a)(1)). Options do not qualify until exercised; the QSBS clock starts at exercise (or earlier if § 83(b) election is filed on an early exercise), not at grant.
- **Active-business and qualifying-trade requirements.** The corporation must satisfy an active-business test (80% of assets used in a qualifying trade or business) throughout substantially all of the holder's holding period (IRC § 1202(c), (e)).

### The per-issuer gain exclusion

The exclusion is a per-issuer, per-shareholder cap. <!-- needs-research: confirm the current per-issuer, per-shareholder gain-exclusion cap under IRC § 1202(b)(1); the historical cap has been the greater of $10M of eligible gain or 10× the holder's aggregate basis in the stock, but monitor 2024–2025 legislative proposals and any amendments. -->

### Practical implication for the plan structure

The AGA $50M deadline is a planning event. Many capital-light SaaS and AI-infrastructure startups cross the $50M AGA line somewhere between Series-B and Series-C, depending on how much of the raise sits as cash. The practitioner's plan-structure response:

- Encourage early-exercise with § 83(b) election for employees entering before the AGA line, so each employee's QSBS clock starts as early as possible on the maximum share count.
- Shift to NSO rather than ISO when the holder's economics favour it (NSO + 83(b) early-exercise can start the QSBS clock on a larger share count than the ISO $100k-limited portion).
- Track the AGA line explicitly in the quarterly comp-committee report; brief the committee before the line is crossed so grants scheduled around the crossing can be timed deliberately.

For a specific employee's QSBS economics — exercise cost vs. probability-of-vest vs. tax-preference value — defer to `startup-finance-fundraising-curriculum`.

## Secondary-tender pattern at Series-C+

### The structure

A secondary tender offer is a corporation-initiated or investor-led transaction in which existing vested shares are purchased from employees (and sometimes early investors) for cash. The tender provides partial liquidity to vested employees without a public offering or acquisition. At most Series-C+ companies, a tender happens every 12–24 months.

### Securities-law treatment

Issuer tender offers under SEC Rule 13e-4 and third-party tender offers under SEC Rule 14E impose disclosure, filing, and timing requirements. A tender must stay open for a minimum period (currently 20 business days under Rule 14E-1), must disclose specified information to tendering shareholders, and must treat all shareholders of the same class on the same terms. Participation caps (e.g., each eligible employee may tender up to 20% of vested shares, subject to an aggregate dollar cap) are standard structural features.

### Interaction with cross-fund conflicts and governance

A tender led by an existing investor who also sits on the board creates a related-party-transaction surface (`mod-108-governance-and-board-operations`). The practitioner default is a disinterested-director-committee review, an independent fairness opinion where material, and documentation of the arm's-length price determination (`mod-102-corporate-formation-and-governance` on fiduciary duty; `mod-106-409a-and-stock-administration` on the FMV determination).

### Scope boundary

Transaction execution, pricing mechanics, tax-withholding operations, and interaction with the preferred-stock waterfall belong to `startup-finance-fundraising-curriculum` (share mechanics) and `startup-exit-curriculum` (transaction execution). The *comp-committee decision* — whether to permit tenders, what participation cap applies, how tenders interact with grant guidelines and refresh grants — stays here.

## Acceleration mechanics for IC grants

The default for IC grants is **no acceleration** on change of control. The grant continues under the acquirer's successor plan on the same vesting schedule.

Some senior IC and manager-level grants include **double-trigger acceleration**: the vesting accelerates in full or in part if (a) a change of control occurs *and* (b) the employee is involuntarily terminated without cause or resigns for good reason within a specified window after close (typically 12–18 months). The double-trigger structure is retention-friendly for the acquirer (the acquirer gets to retain the employee by not firing them) and employee-friendly (the employee is protected from an acquirer-driven termination that would otherwise forfeit unvested shares).

Single-trigger acceleration — vesting accelerates on change of control regardless of continued employment — is rare for IC. It appears at the executive level and only for specific negotiated roles (see [chapter 04](./04-executive-compensation-packages.md)).

The population-level consistency of acceleration treatment matters: three different acceleration patterns across the IC population creates a diligence surface at acquisition. The comp-committee's job is to adopt a written rubric — e.g., "no acceleration below L5; 50% double-trigger acceleration at L5–L6; 100% double-trigger at L7 and above" — and apply it uniformly.

The *change-of-control-equity-policy* in full — single vs. double trigger, good-reason definitions, parachute-payment § 280G cutback mechanics, the acquirer-successor-plan rollover — is the subject of [chapter 07](./07-change-of-control-equity-policy.md).

## A worked example

**NimbusForge Inc.** is a Delaware C-corporation. It closed a $42M Series B 11 months ago on a $220M post-money valuation. Headcount is 68, with 59 US employees (across California, Washington, New York, and Colorado), 6 UK employees, and 3 Berlin-based employees. Aggregate gross assets today are approximately $38M (most of the Series-B cash is still on the balance sheet). The option pool was topped up at the Series-B close to 12% of the fully diluted cap. The 409A FMV from the most recent valuation (post-Series-B) is $0.84 per share.

**Candidate: Priya Rao, Staff Software Engineer (L5), US-based (Seattle, WA).** The grant guideline ([chapter 01](./01-grant-guidelines-by-level-and-function.md)) for a Staff IC at Series-B at NimbusForge is approximately 0.18% of the fully diluted cap, which at the current cap table is 54,000 shares.

Plan structure:

- **Vehicle.** ISO up to the IRC § 422(d) $100k vesting-value limit; NSO overflow. First-year vest is 13,500 shares (25% of 54,000) at $0.84 FMV, worth $11,340 at grant — comfortably inside the $100k ISO envelope. Years 2–4 vest 13,500 shares each — also inside the envelope at today's FMV. If a Series-C materially raises FMV, future years' ISO envelope may be exceeded; NimbusForge's equity administrator runs the § 422(d) chronological-ordering test each year and flags overflow to the comp committee.
- **Schedule.** 4-year monthly vest with 1-year cliff. 13,500 shares cliff-vest at month 12; 1,125 shares per month thereafter.
- **Cliff treatment.** Plan document is explicit: forfeiture on termination before cliff, with comp-committee discretion. No pre-commitment to accelerate.
- **Early exercise.** Not offered. NimbusForge's practitioner view is that at post-Series-B FMV of $0.84, the up-front exercise cost on 54,000 shares ($45,360) is more friction than most IC-level employees want to absorb, and the tax-preference-math (`startup-finance-fundraising-curriculum`) favours standard-exercise-at-vest for most. The programme was discontinued at Series-A close.
- **QSBS planning.** AGA is $38M today, under the $50M line. Priya's QSBS clock will start when she exercises vested shares. The equity administrator sends her a QSBS-eligibility memo at offer-letter time and a reminder at the 1-year-anniversary vest. NimbusForge projects crossing the $50M AGA line within 6–9 months (at Series-C close); existing grants remain QSBS-eligible on exercise, but post-$50M grants to future hires will not be.
- **Post-termination exercise window.** 90 days post-termination (ISO-preserving under IRC § 422(a)(2)). The grant notice includes an AMT-exposure warning and a reference to the equity-administrator's exercise-education materials.
- **Acceleration.** None at L5. The comp-committee rubric kicks in at L7 and above (double-trigger acceleration up to 100% for executives — see [chapter 04](./04-executive-compensation-packages.md)).

**UK peer: Oliver Hughes, Staff Software Engineer, London.** NimbusForge Ltd (the UK subsidiary) qualifies for EMI (gross assets under £30M, fewer than 250 employees, qualifying trade). Oliver's grant is 54,000 EMI options at the same £-equivalent exercise price. The UK-side tax treatment under the EMI regime provides a significant capital-gains-side benefit on exercise and sale within the EMI envelope, subject to the £250,000 individual EMI limit and the £3M company EMI limit. <!-- needs-research: confirm current UK EMI individual (£250k) and company (£3M) limits under the ITEPA 2003 Schedule 5 regime as of the current tax year, and HMRC's post-2024 Spring Budget treatment of EMI. --> No early-exercise programme in the UK.

**Berlin peer: Lena Keller, Staff Software Engineer, Berlin.** Historically, German venture-backed startups have operated phantom-equity ("virtuelle Mitarbeiterbeteiligung") plans because the dry-income problem at vest under § 19 EStG made real-equity plans economically unattractive for employees. The 2024 Future Financing Act (Zukunftsfinanzierungsgesetz) reforms were intended to improve the tax treatment of real-equity plans at German startups. <!-- needs-research: confirm the current German treatment of employee stock options and virtual-share plans under the 2024 Zukunftsfinanzierungsgesetz; verify § 19a EStG amendments and the valuation / deferral mechanics for qualifying grants. --> NimbusForge's current Berlin plan is a virtual-share plan with 54,000 virtual-share units vesting on the same 4-year / 1-year-cliff schedule, settling in cash on a liquidity event. The company and employee are jointly tracking the Zukunftsfinanzierungsgesetz implementation and will consider migrating to a real-equity plan at the next refresh cycle.

## Summary

- The IC equity grant is a bundle of six decisions — vehicle (ISO vs. NSO vs. RSU), schedule (4-year monthly default), cliff (1-year default), exercise mechanics (standard vs. early with § 83(b)), tax election / QSBS planning, and acceleration treatment on CoC. Each is a comp-committee-visible decision captured in the plan document and grant notice.
- ISOs under IRC § 422 are available only to US employees of US corporations and are limited by the $100k vesting-value cap under § 422(d). The AMT exposure on exercise, the dual holding-period requirement, and the 90-day post-termination exercise window are the recurring sources of surprise.
- Private-company RSUs almost always use a double-trigger (time-vesting plus liquidity-event performance condition) structure to avoid the phantom-income problem at vest and the § 409A deferred-compensation problem. The 7-year expiration risk requires a quarterly tracking workstream at Series-C and beyond.
- Early-exercise with § 83(b) election is a pre-Series-B tool for starting the capital-gains and QSBS five-year clocks on day one. The 30-day § 83(b) election deadline is strict and the practitioner default is to send a pre-filled form and track filing confirmation.
- QSBS under IRC § 1202 has a $50M aggregate-gross-assets ceiling at the time of issuance that caps when future grants can qualify; capital-light SaaS and AI-infra startups typically cross the line between Series-B and Series-C and must plan grant timing accordingly. See `startup-finance-fundraising-curriculum` for the QSBS economic math.
- International grants require local-counsel-driven vehicle selection (EMI in the UK for qualifying companies, BSPCE in France, phantom-equity or Zukunftsfinanzierungsgesetz-compliant real-equity in Germany, etc.). The US-centric plan document does not translate; each country is a separate workstream.
- IC acceleration default is "none." Double-trigger acceleration for senior IC is a written-rubric decision. Executive single-trigger / double-trigger acceleration is governed by [chapter 07](./07-change-of-control-equity-policy.md). The *consistency* of acceleration treatment across the IC population is a diligence surface at acquisition and belongs in the comp-committee's standing rubric.
