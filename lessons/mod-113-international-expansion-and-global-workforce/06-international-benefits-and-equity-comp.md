# 6. International benefits and equity compensation

> A US ISO / NSO / RSU plan does not port to Germany, France, or the UK — the tax treatment of the same option differs by country in ways that can convert an intended incentive into a punitive personal tax outcome. Design the international benefits and equity stack per country, from the beginning.

## Motivation

An early-stage US startup builds its comp-and-benefits stack around US defaults: employer-sponsored medical/dental/vision (see [mod-106](../mod-106-compensation-architecture-and-total-rewards/)), a 401(k), and a US stock-plan issuing ISOs and NSOs with a standard early-exercise mechanic. Every one of those defaults has an international analogue — the analogue is materially different, is bounded by statutory minimums and tax regimes the US plan does not consider, and requires country-specific plan design to produce the intended employee outcome.

The consequence of not planning for this is that the group hires an experienced ML researcher in Berlin, offers them a standard NSO grant, and the researcher discovers on exercise that they owe German income tax on the option spread at the wage-tax rate (including social contributions), potentially at a moment when the underlying shares are still illiquid — a tax bill from an unrealised paper gain. The same fact pattern in the UK could be structured under EMI with capital-gains treatment; in France, under BSPCE with favourable treatment; in Israel, under a § 102 track that defers taxation until sale. Different structures, different pre-registration and administrative requirements, materially different employee outcomes.

This chapter frames the international benefits stack (health, pension, retirement) and the country-specific equity-comp regimes (UK EMI, French BSPCE, German dual-employer stock-option treatment, Israeli § 102), and closes with the FX / tax-residency / social-security-totalisation practicalities that shape the international-employee experience.

**Ownership boundary before we begin:** this chapter owns the **international benefits and equity-comp overlay**. It defers to [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/) for the underlying equity-plan and comp-committee architecture, and to [mod-106](../mod-106-compensation-architecture-and-total-rewards/) for the US-side compensation-architecture layer. Country-specific equity-plan structuring is specialist tax / legal advisor territory — retain local counsel and, in most cases, a global-mobility / equity-comp advisor for the international overlay.

## Country-appropriate health, pension, and retirement

The base compensation stack outside the US typically decomposes into: **statutory social-insurance contributions**, **statutory pension enrolment**, **market-standard private-benefit top-ups**, and **statutory or market-standard paid leave**. The mix varies by country.

### United Kingdom

- **Statutory pension — auto-enrolment.** Every UK employer must automatically enrol eligible workers in a workplace pension scheme under the Pensions Act 2008. Minimum total contribution: **8% of qualifying earnings**, with employer contribution **≥ 3%** and employee contribution making up the balance. Common market practice: **5–10% employer contribution**, employee at a matching or comparable rate; some employers offer salary-sacrifice arrangements for NIC savings.
- **NHS + private health top-up.** UK residents access the National Health Service (NHS) as of right; private-medical-insurance top-ups (Bupa, Vitality, AXA Health) are commonly offered as a taxable benefit-in-kind. Not a statutory requirement; a market-standard offering.
- **Statutory sick pay (SSP).** Employer-paid statutory sick pay under the Social Security Contributions and Benefits Act 1992; most employers offer enhanced company sick pay above the SSP floor.
- **National Insurance.** Employer NIC ~13.8% (Class 1 secondary) on earnings above the secondary threshold; employee NIC 8% (main rate) above the primary threshold, 2% above the upper earnings limit. Rates and thresholds change annually. <!-- needs-research: verify current UK NIC rates and thresholds for 2025–2026. -->

### Germany

- **Statutory health insurance (Gesetzliche Krankenversicherung).** ~14.6% of gross earnings up to the contribution ceiling (Beitragsbemessungsgrenze), split 50/50 between employer and employee, plus a fund-specific supplemental rate (Zusatzbeitrag, currently averaging ~1.7%). Employees above the annual compulsory-insurance threshold (Versicherungspflichtgrenze) may opt into private health insurance (Private Krankenversicherung); the employer contributes up to the equivalent statutory-share.
- **Statutory pension (gesetzliche Rentenversicherung).** 18.6% of earnings up to the pension-contribution ceiling, split 50/50.
- **Statutory unemployment insurance.** 2.6%, split 50/50.
- **Long-term-care insurance (Pflegeversicherung).** ~3.4% of earnings, roughly split 50/50 (employer share slightly lower; childless employees pay a supplement).
- **Statutory continued-pay-during-sickness.** 6 weeks at 100% employer-paid; thereafter, statutory Krankengeld from health insurance. Employers frequently offer supplemental cover.
- **Occupational pension (betriebliche Altersvorsorge).** Not statutorily required for the employer but the employee has a statutory right to salary-sacrifice into an occupational pension scheme (Betriebsrentengesetz § 1a). Frequently offered as an employer-supported programme.

<!-- needs-research: verify current German statutory contribution rates and the Beitragsbemessungsgrenze / Versicherungspflichtgrenze thresholds for 2025–2026 (they change annually). -->

### France

- **Sécurité sociale.** Statutory social-insurance contributions cover health, maternity, disability, old-age retirement, family allowances, workplace injury, and unemployment; total employer-side charges (charges patronales) typically range **40–45% of gross salary** with rates varying by earning tier; employee-side charges typically 20–23% of gross salary. Charges are calculated on a bracketed basis with different rates by ceiling tier (plafond de la sécurité sociale, tranches A, B, C). This is one of the highest employer-side statutory burdens in the OECD.
- **Complementary retirement (AGIRC-ARRCO).** Mandatory complementary retirement schemes on top of the sécurité sociale retirement pension; employer and employee contribute at defined rates.
- **Mutuelle (complementary health insurance).** Employers must provide a complementary health insurance scheme (mutuelle) covering costs beyond the statutory sécurité sociale reimbursement (Loi n° 2013-504); employer contributes at least 50%.
- **Ticket-restaurant / meal vouchers.** Common market-standard benefit; employer contributes at defined rate.
- **Paid annual leave** — 5 weeks statutory (see [chapter 05](./05-international-employment-law-variance.md)) plus RTT (réduction du temps de travail) days for employees on 35-hour equivalents working effective longer hours.

### Netherlands

- **Statutory social-insurance contributions.** Employer contributes to WW (unemployment), WIA (disability), and Zvw (health-insurance income-dependent contribution); employees contribute to national insurance (AOW, ANW) via wage-tax withholding.
- **Private health insurance (Zorgverzekering).** All residents must hold private (regulated) health insurance individually; employer plays limited direct role.
- **Occupational pension.** Sector-wide pension funds are common (via sector-specific mandatory participation); if not sector-mandated, employers typically offer a company pension scheme.
- **Vacation allowance (vakantiegeld).** 8% of annual salary, statutorily paid in May/June of each year (in addition to base salary and paid vacation).

### Ireland

- **PRSI (Pay Related Social Insurance).** Employer and employee contributions to the Social Insurance Fund; employer PRSI ~11.05% (Class A1); employee PRSI 4%.
- **Auto-enrolment retirement savings.** Ireland's Automatic Enrolment Retirement Savings System is being introduced in phased rollout beginning in 2025 (implementing the Automatic Enrolment Retirement Savings System Act 2024). <!-- needs-research: verify current status and effective date of Irish auto-enrolment as of 2025–2026. -->
- **HSA / private-health-insurance top-up.** Not statutorily required; commonly offered.

### Canada

- **CPP / QPP contributions.** Canada Pension Plan (CPP) or Quebec Pension Plan (QPP) — mandatory employer and employee contributions on pensionable earnings.
- **EI contributions.** Employment Insurance — employer and employee contributions.
- **Provincial health.** Provincial medicare covers most medical services; employer-sponsored **extended health benefits** (dental, vision, prescription-drug top-up) are market-standard.
- **RRSP / group RRSP.** Voluntary; commonly offered as a group RRSP with employer matching.

### Australia

- **Superannuation Guarantee.** 11.5% (rising to 12% July 1, 2025) of ordinary time earnings, employer-paid into a complying super fund.
- **Medicare Levy.** Government Medicare; separately, employer-sponsored private health insurance may be offered as a benefit.

### Singapore

- **Central Provident Fund (CPF).** Mandatory retirement / housing / medical savings scheme for Singapore citizens and permanent residents; employer contribution up to 17% and employee contribution up to 20% depending on age band and wage ceiling. Foreign workers on Employment Pass do not participate in CPF.
- **Private medical insurance.** Not statutorily required for private-sector employers; market-standard offering.

### India

- **Employees' Provident Fund (EPF).** Statutory retirement scheme; employer and employee each contribute 12% of basic salary + dearness allowance (subject to statutory wage ceiling, though many employers voluntarily contribute above the ceiling).
- **Gratuity.** Payment of Gratuity Act 1972 — employer pays 15 days' salary per year of service on termination after 5+ years of service.
- **Group health insurance.** Not statutorily required in most sectors; strongly market-expected.

### Israel

- **Pension Fund / Manager's Insurance (Bituach Menahalim).** Mandatory pension enrolment under Extension Order 2008; employer contributions ~6.5%–7.5% and employee contributions ~6.0% (rates and split subject to variance).
- **Severance component (Pitzuim).** Additional statutory contribution to the pension fund covering severance-pay obligations — 8.33% of salary paid into a Section 14 fund.
- **Study fund (Keren Hishtalmut).** Common tax-preferred savings vehicle; employer contribution ~7.5% up to ceiling, employee 2.5%.

## Country-specific equity-compensation regimes

Global equity-compensation planning is one of the highest-value benefits-design exercises the group runs. Country-specific tax-preferred regimes exist in several markets; using them requires plan-level structuring, pre-grant filings, and administrative discipline. Missing them typically means the employee receives an option that is taxed as ordinary income (wage tax + social contributions) at exercise on the spread — a materially worse outcome than the US ISO / NSO baseline.

### United Kingdom — EMI (Enterprise Management Incentives)

**Enterprise Management Incentives (EMI)** under the Income Tax (Earnings and Pensions) Act 2003 (ITEPA 2003) Schedule 5. A tax-advantaged option scheme for qualifying UK companies.

**Company qualifications:**
- **Independent** (not a 51%-subsidiary).
- **Gross assets ≤ £30M** at grant.
- **Fewer than 250 full-time-equivalent employees** at grant.
- **Trading company** engaged in a qualifying trade (excluded activities — banking, property development, farming, and others — disqualify).
- The **US-parent structure requires careful analysis.** A UK Ltd subsidiary of a US parent may qualify as an EMI-issuing company for its own equity, but grants over the US parent's stock to UK employees typically do not qualify for EMI. The workaround (grant over US-parent stock outside EMI, with local tax-planning support) is common but forfeits EMI benefits.

**Individual qualifications:**
- **Full-time employee** (≥ 25 hours/week or 75% of working time) of the granting company.
- No **≥ 30% material interest** in the company before or after grant.
- **£250,000** limit on unexercised EMI options per individual across all EMI-qualifying grants.

**Tax treatment:**
- **No income tax or NIC on grant** or at exercise (if exercise price ≥ market value at grant).
- **Capital gains tax on sale** of the shares — with **Business Asset Disposal Relief (BADR)** (formerly Entrepreneurs' Relief) potentially applying, taxing the gain at **10%** (up to a lifetime limit of £1M) if held for 24 months from grant.
- No employer NIC.

**Administrative requirements:**
- Options must be **notified to HMRC within 92 days of grant** (via the ERS Online service). Missed notification disqualifies the grant.
- Annual reporting to HMRC via the ERS annual return.

**Practical implication:** For qualifying UK companies (many early-stage UK startups; **US-parent structures generally do not qualify** on the US-parent stock), EMI is the workhorse UK employee-equity vehicle. US-parented groups hiring UK employees typically grant over US-parent stock with awareness that EMI is not available and the tax treatment defaults to standard UK employee-share-option treatment (income tax + NIC on exercise-spread).

### United Kingdom — non-EMI grants over US-parent stock

For US-parent grants to UK employees (the common case):

- **Income tax and NIC on exercise-spread** as employment income. Employer NIC ~13.8% attaches; employer often shifts employer-NIC exposure to the employee via a joint-election (ITEPA 2003 s. 431 election combined with a s. 222 arrangement for the NIC).
- **CGT on subsequent sale gain** measured from the exercise price.
- **Section 431 election** — an employer / employee joint election at acquisition to be taxed on the unrestricted market value at acquisition (rather than at each restriction-lifting event). Standard practice for RSU-and-restricted-share grants.

Structural options:
- **UK CSOP (Company Share Option Plan)** — a separate tax-advantaged UK plan (ITEPA 2003 Schedule 4) permitting up to **£60,000** of options per employee with favourable treatment if held ≥ 3 years. Broader company-eligibility than EMI; can work for US-parent stock. Notification and HMRC-approval requirements apply.
- **SIP (Share Incentive Plan)** and **SAYE (Save As You Earn)** — separate all-employee tax-advantaged plans; less common in venture-backed structures.

### France — BSPCE (Bons de Souscription de Parts de Créateur d'Entreprise)

**BSPCE** under Code général des impôts article 163 bis G. A tax-advantaged warrant / option scheme for qualifying French companies.

**Company qualifications:**
- **Corporate form** — SA, SAS, SCA, SARL, or equivalent.
- **French tax resident** or established in an EU/EEA member state.
- **Less than 15 years old** at grant.
- **Not listed** or listed on a market with capitalisation < €150M.
- **Majority-owned** by natural persons or by companies themselves majority-owned by natural persons (subject to specific exemptions).
- **US-parent structure requires structuring.** A French SAS subsidiary of a US parent typically does not qualify for BSPCE on the US-parent stock; but a French SAS itself can issue BSPCE on its own equity to French employees. For a US-parented startup, this means BSPCE is not available for grants over US-parent stock — a structural limitation.

**Individual qualifications:**
- **Employee or director** of the issuing company.

**Tax treatment:**
- **No taxable event on grant or exercise** (subject to conditions).
- **On sale** of the shares:
  - **Preferential capital-gains rate** if employee has 3+ years of service at exercise (12.8% flat rate + 17.2% social contributions = 30% aggregate — the *prélèvement forfaitaire unique*).
  - **Higher rate** (30% for gain up to €150,000 + higher social contributions and marginal rate above) if employee has < 3 years of service.
  - Losses limited in offset.

**Practical implication:** Where BSPCE is available (French entity issuing on its own equity), it is the workhorse French employee-equity vehicle. For US-parent grants, BSPCE is not available and the default French tax treatment (income tax + social contributions on exercise-spread) applies.

### Germany — dual-employer stock-option treatment

Germany does not offer a UK-EMI-equivalent tax-advantaged employee-option scheme. The default treatment of US-parent stock options granted to German employees is:

- **Income tax on the exercise-spread** as employment income (wage tax withholding via the German employer's payroll).
- **Social-insurance contributions** on the exercise-spread up to the contribution ceiling.
- **Trade tax (Gewerbesteuer)** implications for the German employer entity.

**§ 19a EStG (Zukunftsfinanzierungsgesetz reform).** The 2023 Zukunftsfinanzierungsgesetz (Future Financing Act) introduced an expanded **§ 19a EStG** deferral mechanism for employee-equity grants by qualifying employers — allowing deferral of income tax on exercise-spread until sale, change of employer, or a 15-year outer limit. Qualifying employer criteria (SME thresholds, age of company) apply. This is a meaningful improvement for early-stage grants but requires careful structuring and cooperation from the German employer entity. <!-- needs-research: confirm the current § 19a EStG criteria and thresholds as amended by the Zukunftsfinanzierungsgesetz and any successor legislation as of 2025–2026. -->

**Practical implication:** German employee equity is one of the least-favourable regimes for standard US-parent option grants. Careful structuring — potentially including § 19a EStG deferral where the employer qualifies — is required to avoid the pattern of dry tax at exercise on illiquid stock.

### Israel — § 102 tracks

**Section 102 of the Israeli Income Tax Ordinance** — a tax-advantaged option regime for grants to Israeli employees via a **trustee**.

Two tracks:

- **Section 102 Capital Gains Track (with trustee).** Options granted to a trustee, held for a mandatory holding period of **24 months from grant**. On sale, gain taxed as capital gain at 25% (with any employer-side benefit-in-kind classification specifics), except for the portion of the gain equal to the exercise-price-vs-30-day-average-market-price at grant, which is taxed as ordinary employment income.
- **Section 102 Ordinary-Income Track (with trustee).** Options taxed as employment income on exercise; less common.
- **Section 3(i) — no trustee.** Options taxed as employment income on exercise, without deferral; used only when § 102 conditions cannot be met.

**Structural requirements:**
- Options must be granted **to a trustee** (a licensed § 102 trustee — e.g., Altshuler Shaham, IBI Trust).
- Plan must be **filed with the Israeli Tax Authority (ITA)** at least **30 days** before the first grant under the plan.
- Employer must elect the track (Capital Gains vs. Ordinary Income) and stay consistent for all grants under the plan for the year.

**Practical implication:** § 102 Capital Gains Track (with trustee) is the workhorse for Israeli employee equity. The 30-day pre-grant plan filing is a hard requirement; missed filing forfeits § 102 treatment and defaults grants to § 3(i) ordinary-income treatment. Retain an Israeli employment / tax counsel and a licensed trustee at the earliest sign of Israeli hiring.

### Other jurisdictions — Canada, Australia, Netherlands, Singapore, India

- **Canada.** Employee stock options taxed as employment income on exercise-spread, with a **50% stock-option deduction** available for CCPC-issued qualifying options (Income Tax Act s. 110(1)(d)) or, for non-CCPC options, subject to a $200,000 annual vesting cap on the deduction (2020 amendments effective 2021). US-parent options to Canadian employees typically do not qualify for the CCPC-favourable treatment.
- **Australia.** Employee Share Scheme (ESS) rules under Division 83A ITAA 1997; the 2022 reforms (removing "cessation of employment" as a taxing point for start-up-concessional ESS interests) improved the regime. **Start-up concession** available for grants by qualifying start-ups (unlisted, aggregated turnover < AUD 50M, incorporated < 10 years). Where the concession applies, options taxed on sale rather than exercise; discount / spread at grant not immediately taxable.
- **Netherlands.** Employee stock options taxable on **exercise** (post-2023 rules; previously on vesting) as employment income, with employer wage-tax withholding. RSUs taxable on vesting.
- **Singapore.** Options taxable on exercise as employment income; **Not Ordinarily Resident (NOR)** and **Employee Equity-Based Remuneration (EEBR) scheme** provide relief in specific cases. <!-- needs-research: verify current Singapore ESOP tax framework and any scheme replacements. -->
- **India.** Employee stock options taxable on exercise as employment income (perquisite tax); on sale, capital-gains tax on gain over exercise-value. **ESOP taxation deferral** for eligible start-ups (DIPP-recognised) — deferral until earliest of sale, cessation of employment, or 4/5 years from exercise. Structural specifics via a licensed Indian tax advisor.

## The global equity-plan administration overlay

Beyond the country-specific plan design, several operational patterns apply globally:

- **Global plan structure.** Most US-parented groups issue employee equity from a single US-parent equity plan (issued in US-parent stock). Local country subsidiary employees receive grants under the US plan. Local **country addenda** or **sub-plans** to the US plan (for UK CSOP, French BSPCE where possible, Israeli § 102, etc.) implement the country-specific tax-preferred regimes.
- **Trustee arrangements.** Israeli § 102 requires a trustee; some other jurisdictions permit / require trustee structures for tax-advantaged treatment.
- **Payroll withholding.** Employer wage-tax withholding on option-exercise-spread applies in most jurisdictions (UK PAYE, German Lohnsteuer, French charges sociales, Dutch wage tax, etc.). Payroll integration is a real operational lift — the equity-administration platform (Carta, Pulley, Shareworks, Global Shares) must integrate with each country's payroll to withhold correctly.
- **Mobility and cross-border grants.** Employees who move between countries during the vesting or exercise period create allocation questions — the option's underlying earning period is apportioned between the countries under either tax treaty or OECD Model Commentary principles, with each jurisdiction claiming its share of the tax base. Global-mobility advisors (Deloitte GES, KPMG GMS, PwC GES, EY People Advisory) handle the specifics.
- **Grant approvals.** Some jurisdictions require regulatory filings for cross-border equity grants (e.g., Brazil, China). Local counsel advises on any pre-grant filings.

## FX, tax-residency, and social-security totalisation

Three cross-cutting practicalities:

### FX and currency

Employees are typically paid in the currency of the country where they are employed. Executive-comp packages, retention bonuses, and equity-strike-prices are usually denominated in the currency of the granting entity (typically USD for US-parent grants). The employee bears the FX exposure between grant-currency and pay-currency; the group bears the FX exposure between local-currency cost and USD reporting-currency P&L. Common approaches:

- **Grant-currency USD, exercise-currency USD, paid via local payroll at spot on exercise date.**
- **Local-currency reference amount for cash-comp** (e.g., total-cash comp expressed in GBP for UK employees) with USD reporting on the group side.
- **FX hedging for material employer-side exposure** (typically a treasury / CFO decision, not an HR decision).

### Tax residency

An employee's tax residency drives which country's tax regime applies to their worldwide income. Rules vary by country (day-counts, permanent-home test, centre-of-vital-interests test); common tie-breaker: **OECD Model Tax Convention Article 4**. Practical operator implications:

- **Digital-nomad / remote-first patterns risk multiple tax residencies.** An employee employed by a UK subsidiary but resident in Spain half the year may create Spanish tax and social-security obligations for the employer.
- **Return-to-employer moves** (e.g., a UK-employed employee moving to work at the US parent for 6 months) create split-year tax and potentially PE risk. Coordinate with tax / immigration counsel.
- **Formal remote-work-anywhere policies** need a country whitelist / blacklist based on the group's ability to comply with local employer obligations in each candidate country. Do not simply enable remote-anywhere without an operator-side risk map.

### Social-security totalisation

**Totalisation agreements** — bilateral agreements between two countries that eliminate double social-security contributions for temporarily-assigned workers. The US has totalisation agreements with roughly 30 countries (Australia, Austria, Belgium, Brazil, Canada, Chile, Czech Republic, Denmark, Finland, France, Germany, Greece, Hungary, Iceland, Ireland, Italy, Japan, Luxembourg, Netherlands, Norway, Poland, Portugal, Slovakia, Slovenia, South Korea, Spain, Sweden, Switzerland, United Kingdom, Uruguay). <!-- needs-research: verify current US totalisation-agreement country list — the SSA maintains it and adds occasionally. -->

For a covered employee on a qualifying assignment, the worker (and employer) continues to pay social security to the sending country only, subject to a **certificate of coverage** (SSA Form USA/DE 101 for Germany, etc.) evidencing exemption from the host country. This is a real employer-side cost saving on international assignments; retain global-mobility counsel to structure and file the certificates.

Analogous EU-level regime: **EU Regulation 883/2004** on social-security coordination — a single member-state's social-security system applies to a worker at any one time, with defined tie-breakers.

## Concrete example — offer-package construction for a Berlin ML researcher

A representative offer-package construction for a senior ML researcher joining a US Series-B startup's newly-formed German GmbH subsidiary:

- **Base salary (Berlin market, senior ML).** €130,000 gross annually (paid monthly + 13th-month or vacation-allowance typical in some collective-agreement contexts; confirm inclusion or exclusion structure).
- **Statutory social insurance.** Employer-side ~20% (pension 9.3% + unemployment 1.3% + health 7.3% + long-term care 1.7% + accident insurance ~1%) on earnings up to contribution ceilings.
- **Occupational-pension eligibility.** Employer opens salary-sacrifice pathway per BetrAVG § 1a; commonly, employer matches up to 4% of BBG-A ceiling.
- **Statutory annual leave.** 25 days (above 20-day BUrlG minimum, aligned with German market).
- **Continued sick pay.** 6 weeks statutorily at 100%, per employer standard.
- **Health insurance.** Standard GKV (statutory health) for salaries below the Versicherungspflichtgrenze; for high-earners above, choice of PKV (private).
- **Equity grant.** 5,000 US-parent NSOs, 4-year vesting, 1-year cliff, US-parent standard plan. **German tax note:** exercise-spread taxable as wage income at ordinary rates + solidarity surcharge; social-insurance contributions apply up to contribution ceilings. **§ 19a EStG deferral** evaluated based on German GmbH's employer-qualification status; if applicable, income-tax deferred until liquidity event or 15-year outer limit. Explicit written note to candidate that they should consult a German tax advisor on personal exercise strategy.
- **Employee-invention regime.** ArbnErfG applies; any invention created in the course of employment must be notified to employer under statutory process; employer decides on claim within 4 months; statutory compensation entitlement flows if employer claims the invention.
- **Employment contract.** German-language contract (with English translation) drafted by German counsel; indefinite-term (unbefristet); 4-week statutory notice per BGB § 622 baseline extending under contract to 3 months mutual for a senior role; ArbnErfG acknowledgement; IP-assignment addendum reinforcing US-parent ownership via ICSA.

The offer's German-specific complexity is prosaic once mapped; the mapping is what the incoming operator has to do at the point of decision.

## Anti-patterns

- **Porting the US equity plan without a country addendum.** Grants issued under US-plan defaults with no country-addendum treatment for UK EMI, French BSPCE, Israeli § 102, or German § 19a — leaving material employee-tax and employer-side compliance value on the table.
- **Missing the 30-day Israeli § 102 pre-grant filing.** Grants forfeited to § 3(i) ordinary-income treatment; no fix retroactively.
- **Missing the 92-day EMI notification.** UK EMI grants disqualified permanently; falls back to standard employee-share-option treatment.
- **Ignoring statutory contribution ceilings and mandatory benefits when budgeting international headcount.** German employer-side statutory burden approaches 20% of gross salary; French charges patronales approach 40–45%; a US-native budget of "salary + 20% loaded overhead" underestimates the true cost by 20–30%.
- **Assuming EOR platforms handle equity correctly.** Some EOR platforms cannot administer local statutory equity schemes (EMI, BSPCE, § 102). Confirm before hiring.
- **No global-mobility advisor.** International equity plans, tax residency, and totalisation are specialist territory; running them internally without advisor support is a false-economy risk.

## Summary

- **Base benefits (health, pension, retirement) vary by country** in ways that materially change the total-cost-per-employee. Employer-side statutory burden ranges from ~10% (Singapore, Ireland) to ~45% (France) of gross salary.
- **Country-specific tax-preferred equity regimes** exist in several markets: UK EMI (with limited US-parent applicability); UK CSOP (broader applicability); French BSPCE (limited US-parent applicability); Israeli § 102 (with mandatory trustee and 30-day pre-grant filing); German § 19a EStG (with qualifying employer criteria); Australian ESS start-up concession; Indian ESOP deferral for DIPP-recognised start-ups.
- **Country addenda / sub-plans** are the standard mechanism for implementing country-specific treatment under a single US-parent equity plan.
- **FX, tax residency, and social-security totalisation** are cross-cutting practicalities — grant-currency and pay-currency conventions, tax-residency rules that drive worldwide-income exposure, totalisation agreements that eliminate double social-security on qualifying assignments.
- **Global-mobility and equity-comp advisors** (Big-4 GES / Global Mobility Services practices, boutique global-equity administrators) are specialist territory; retain them for international-plan structuring, cross-border-mobility administration, and grant-jurisdiction analysis.
- **This chapter frames the benefits and equity-comp overlay.** The US-side comp architecture sits in [mod-106](../mod-106-compensation-architecture-and-total-rewards/); the underlying US equity plan and comp-committee mechanics sit in [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/).
