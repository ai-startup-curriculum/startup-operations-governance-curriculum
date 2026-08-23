# 2. The first international entity setup

> Country selection is a design decision that ripples for a decade — talent, tax credits, IP holding jurisdiction, exit-optionality. The wrong first-country choice is expensive to undo; the right one compounds.

## Motivation

The moment [chapter 01](./01-eor-vs-peo-vs-direct-entity-decision-framework.md) tips a country from EOR to direct entity, the operating question changes shape. It is no longer "how do we employ this person?" but "what entity, in what country, with what statutory form, with what local directors, on what bank, on what payroll, under what group-holding position?" These decisions are load-bearing. The country becomes the group's centre of gravity for R&D or GTM or IP holding for years; the statutory form defines the ongoing governance and audit lift; the local-director choice defines the personal-liability exposure of individual officers.

This chapter is the design playbook. It stops short of the intercompany / transfer-pricing structuring — [chapter 03](./03-intercompany-and-transfer-pricing-structure.md) — and the country-specific employment-law layer — [chapter 05](./05-international-employment-law-variance.md). It also stops well short of the specialist tax structuring that Big-Four and boutique international tax counsel own end-to-end; the goal here is to make the incoming operator conversant enough to run the decision responsibly with those advisors.

## The four country-selection drivers

Country selection is driven by one or more of four business reasons. Every deliberate first-country choice can be traced to at least one of them; a country chosen for none of these reasons is usually a country chosen by accident.

### Driver 1 — engineering talent availability

The most common early-stage international-expansion driver. Pick a country because a specific technical talent pool is dense there and the group needs to build in it.

Representative geographies:

- **United Kingdom.** Deep AI / ML and research-engineering talent (Oxford, Cambridge, UCL, ICL; DeepMind, Isomorphic, Wayve, Stability alumni network). English-language operations. Common-law legal system familiar to US counsel. Time-zone overlap with US East Coast.
- **Ireland.** Growing AI / engineering hub; tax and IP-holding-jurisdiction advantages (see driver 3 and driver 4). English-language operations. Substantial US-tech-employer presence has built a bench of experienced engineers.
- **Poland.** Deep general-engineering talent at a favourable cost basis; strong C++ / systems / infrastructure and increasing ML depth. EU-member state, so EU-wide free-movement of workers and consistent GDPR regime.
- **Portugal.** Rapidly growing tech hub (Lisbon, Porto); attractive to European engineering talent; Non-Habitual Resident (NHR) tax regime attracted a wave of tech workers (regime has been narrowed since 2024 — verify current terms before recruiting on it). <!-- needs-research: confirm status of Portuguese NHR successor regime IFICI / RNH 2.0 as of 2026 and its practical application to inbound tech workers. -->
- **Spain.** Deep engineering talent, EU-member state; Ley Beckham inbound-expat tax regime attractive for high-earning inbound hires.
- **Romania.** Historically the largest strong-engineering-with-favourable-cost-basis geography in the EU; strong C / C++ and increasingly ML.
- **India.** Deep engineering and ML operations talent at scale; large delivery centres viable; time-zone offset requires deliberate operating-model design. STPI / SEZ tax structuring available (specialist advisor territory).

**Selection principle:** pick the country where the group's specific talent gap can be filled fastest and highest-quality. Engineering-talent expansion is a hire-driven decision; the country's tax and IP posture is secondary but should still be run through drivers 3 and 4 before the entity form is finalised.

### Driver 2 — sales / GTM presence

Sales and go-to-market expansion drives the second wave of international-entity decisions. Enterprise customers frequently prefer or require a local counterparty; local revenue recognition frequently benefits from local invoicing; local sales cycles frequently require local currency, local support hours, and local language.

Representative geographies:

- **United Kingdom.** European sales hub for most US SaaS; English-language operations; time-zone bridge between US and EU markets.
- **Germany.** Largest EU economy; enterprise and industrial-customer buying preferences frequently require local counterparty and German-language sales / support; frequently the second EU market after the UK.
- **Netherlands.** Popular EU-headquarter jurisdiction (see driver 4); English-fluent business environment; Amsterdam as a European sales hub.
- **Ireland.** EU-headquarter jurisdiction; sales-team clustering common due to US-tech-employer presence.
- **Singapore.** APAC sales / operations hub; English-language, stable common-law regime, tax-treaty network into APAC; Pte Ltd is a fast and administratively light corporate form.
- **Australia.** APAC enterprise-sales market; English-language; time-zone bridge for west-coast US teams.
- **Japan.** Japanese enterprise buying frequently requires a local counterparty (Kabushiki Kaisha or Godo Kaisha), local-language sales and support, and often a Japanese national in a senior sales role. High-friction entry but strategically important market.

**Selection principle:** follow the customer. The sales-driven entity is justified by pipeline, not by convenience. Sales-driven entities also carry the highest **permanent-establishment (PE)** risk — a salesperson with authority to conclude contracts creates PE in-country regardless of whether they are directly employed or EOR-employed, which converts a portion of the US parent's operating income into locally-taxable income. Address the PE analysis with a tax advisor before opening a sales presence, not after ([chapter 03](./03-intercompany-and-transfer-pricing-structure.md)).

### Driver 3 — research tax-credit optimisation

Several countries operate R&D tax-credit regimes that generate meaningful cash-back or tax-offset value when qualifying R&D expenditure sits in a local corporate taxpayer. These regimes reward the country selection with real cash — sometimes materially — but require that the local entity conducts and pays for the qualifying R&D.

Named regimes to know:

- **United Kingdom — R&D tax credit.** Historically two schemes: **SME R&D relief** for smaller companies (up to a ~200% super-deduction of qualifying expenditure) and **RDEC** (R&D Expenditure Credit) for larger companies and grant-funded R&D. HMRC merged the two into a single scheme with effect from accounting periods beginning on or after April 1, 2024. Rates and thresholds have moved several times since 2020; confirm the current effective rate before making structural decisions. <!-- needs-research: cite the current single-scheme UK R&D credit effective rate and the R&D-intensive SME enhanced rate as of the 2025–2026 tax year. -->
- **Canada — Scientific Research and Experimental Development (SR&ED) tax credit.** Federal investment tax credit for R&D expenditure incurred by a Canadian resident corporation; refundable portion for CCPCs (Canadian-Controlled Private Corporations) up to specified expenditure ceilings, non-refundable for others; several provinces add supplementary credits (Ontario ORDTC, Quebec R&D credit, British Columbia, others). A US-parent group typically does not qualify as a CCPC, so plan for the non-refundable rate; run the specifics with a Canadian tax advisor.
- **France — Crédit d'impôt recherche (CIR).** French R&D tax credit of 30% of qualifying R&D expenditure up to €100M and 5% above; historically one of the most generous R&D regimes in the OECD. Requires substantiation and can be challenged; the French tax administration is a serious auditor. Pair with a French tax advisor and a rigorous R&D-substantiation programme.
- **Ireland — R&D tax credit.** 30% (as of 2024) refundable credit against corporation tax on qualifying R&D expenditure by an Irish tax resident company; historically an important element of Ireland's inbound-investment offering. <!-- needs-research: confirm the current Irish R&D tax-credit headline rate for 2025–2026. -->
- **Australia — R&D tax incentive.** Refundable / non-refundable offset scheme depending on the entity's aggregated turnover. Administered jointly by AusIndustry and the ATO.

**Selection principle:** if the group's engineering spend is large enough that the credit is materially cash-positive, and the country's talent supply supports the hiring plan, the R&D-credit country becomes a genuine candidate for the first-entity choice. The credit is not free — it requires meticulous substantiation, project-time-tracking, and an annual claim exercise — but it is real. Do not, however, choose a country *only* for the credit if talent supply is thin; the credit does not help if the roles cannot be filled.

### Driver 4 — IP holding jurisdiction

Holding jurisdiction choices for the group's intellectual property have historically driven a family of tax structures where a low-tax IP-holding entity licenses to operating subsidiaries. Two families of jurisdictions dominate the historical playbook:

- **Netherlands and Ireland — EU IP holding.** Both jurisdictions have historically offered favourable regimes for IP-holding entities licensing IP to affiliated operating companies across the EU. Ireland's 12.5% corporation-tax rate (with a 15% top-up rate for large groups under BEPS 2.0 Pillar 2 — see below), a well-established patent-box-adjacent knowledge-development-box (KDB) regime, and extensive tax-treaty network have made it the workhorse EU IP-holding jurisdiction for US-parented groups. The Netherlands offers the innovation-box regime, an extensive tax-treaty network, and a well-known BV corporate form.
- **Singapore — APAC IP holding.** Singapore's 17% headline corporate-tax rate, tax-treaty network in APAC, IP Development Incentive (IDI), and stable regulatory environment make it the common APAC IP-holding jurisdiction.

**BEPS 2.0 Pillar 2 caveat — read before designing.** The OECD's Base Erosion and Profit Shifting 2.0 project introduced a **15% global-minimum effective-tax-rate (GloBE) floor** for **multinational enterprise (MNE) groups with consolidated revenue of €750M or more**, implemented by countries through their local versions of the GloBE Model Rules (the Income Inclusion Rule, the Undertaxed Profits Rule, and Qualified Domestic Minimum Top-up Taxes). Effective dates vary by jurisdiction; the majority of implementing jurisdictions applied the rules to accounting periods beginning in 2024 (IIR / QDMTT) with UTPR from 2025 onward. <!-- needs-research: verify current implementation status of the EU Pillar 2 directive, the UK Multinational Top-up Tax and Domestic Top-up Tax, Ireland's Pillar 2 implementation, and the US treatment of QDMTT and IIR as of the 2025–2026 period. -->

The practical implication for a startup:

- **Below the €750M consolidated-revenue threshold, Pillar 2 does not directly apply.** Most venture-backed startups are well below the threshold and can structure with legacy considerations.
- **Above the threshold, the arbitrage between a low-tax IP-holding jurisdiction and the group's overall effective tax rate compresses to the 15% floor.** IP-holding structures designed for a pre-Pillar-2 regime need reassessment.
- **Design with graduation in mind.** A structure that is optimal at $50M revenue but requires unwind at $750M is a structure that will be unwound at a bad moment. Prefer structures that scale through Pillar 2 rather than collapse into it.

**Startup-appropriate default:** at Series A / Series B, most groups hold all IP in the US parent, license to operating subsidiaries through cost-plus intercompany services or a limited royalty structure ([chapter 03](./03-intercompany-and-transfer-pricing-structure.md)), and defer IP-holding-jurisdiction restructuring to a later stage (typically post-Series C, when revenue and geographic distribution justify the structuring cost). Do not stand up an Irish or Netherlands IP-holding entity in the first year of international expansion unless a specialist tax advisor has produced a written recommendation with a clear payback analysis.

## The country-and-entity-form map

Once the country is selected, the statutory form of the local entity is the next decision. Every country has multiple corporate forms; typically one is the workhorse for wholly-owned subsidiaries of foreign parents. A representative starter map:

| Country | Default form | Notes |
|---|---|---|
| **United Kingdom** | **Ltd** (private company limited by shares) — Companies Act 2006 | Register at Companies House; PSC (People with Significant Control) register required; annual accounts and confirmation statement filings. |
| **Ireland** | **DAC** (Designated Activity Company) or **Ltd** — Companies Act 2014 | DAC is the traditional form; the post-2015 **Ltd** simpler form is also common. Requires at least one EEA-resident director or the § 137 bond; annual return and financial statements to the Companies Registration Office (CRO). |
| **Canada** | **Federal corporation (CBCA)** + provincial extra-provincial registration, or **provincial corporation** in the operating province | Ontario, British Columbia, Alberta each have their own corporate statutes. Federal incorporation is common; extra-provincial registration is per-province where the entity operates. Director-residency requirements vary by province (Ontario removed its requirement in 2021; British Columbia has no requirement; some provinces still require Canadian-resident directors). |
| **Australia** | **Pty Ltd** (proprietary limited) — Corporations Act 2001 | Register with ASIC; at least one Australian-resident director; audit thresholds trigger by size. |
| **Singapore** | **Pte Ltd** — Companies Act 1967 | ACRA registration; at least one Singapore-resident director (citizen, PR, or EntrePass / EP holder). Nominee-director services are commonly used by inbound US groups. |
| **Germany** | **GmbH** (Gesellschaft mit beschränkter Haftung) — GmbHG | €25,000 minimum share capital (€12,500 payable at formation). Notarial deed required for formation. Managing director (**Geschäftsführer**) — no residency requirement, but must be identifiable and legally competent. Statutory audit for medium-sized entities. |
| **Netherlands** | **BV** (Besloten Vennootschap) — Book 2 Dutch Civil Code | Notarial deed required; no minimum share capital since 2012; UBO register at the Chamber of Commerce (KvK). |
| **France** | **SAS** (Société par actions simplifiée) — Code de commerce | The default form for foreign-parent operating subs in France due to its flexibility and lack of works-council trigger below thresholds; **SARL** (limited-liability) is an alternative for very small operations. President (personne morale ou physique) required. |
| **India** | **Private Limited Company (Pvt Ltd)** — Companies Act 2013 | At least two directors, one of whom must be an Indian resident (present in India ≥182 days). Registered office in India; DIN and DSC required for directors; PAN / TAN for tax; GST registration if turnover threshold crossed. |
| **Japan** | **KK** (Kabushiki Kaisha) or **GK** (Godo Kaisha) — Companies Act | KK is the traditional form with higher formality; GK is the Japanese equivalent of a US LLC, lighter and increasingly common for foreign-parent subs. |
| **Israel** | **Ltd** — Companies Law, 5759-1999 | Registrar of Companies filing; local counsel typically required to file. |

The entity-form choice interacts with local employment law (works-council thresholds, audit-triggering thresholds), local statutory-audit rules, and local governance formalities. Confirm with local counsel before filing.

## Local director, secretary, and statutory-agent requirements

Countries vary widely on the residency and identity requirements for directors, corporate secretaries, and statutory agents. A representative summary:

- **UK Ltd.** No director residency requirement. At least one natural-person director. Company secretary is optional for private companies (removed as a mandatory requirement in the Companies Act 2006). PSC (People with Significant Control) register is mandatory.
- **Ireland DAC / Ltd.** At least one **EEA-resident director** required, or the company must post a § 137 bond (currently €25,000 for two years). Company secretary required. UBO filing at the Central Register of Beneficial Ownership (RBO).
- **Canada.** Historically, most provinces required a majority of Canadian-resident directors; a wave of reforms has removed this requirement in Ontario (2021), Alberta, and British Columbia. Federal CBCA requires that at least 25% of directors be Canadian-resident (Section 105(3)), with some exceptions. **Verify the current requirement in the specific incorporating jurisdiction.**
- **Australia Pty Ltd.** At least one **Australian-resident director** (Corporations Act § 201A(1)). Nominee-director services widely available if the group has no Australian resident. Company secretary required if the sole director is not Australian-resident.
- **Singapore Pte Ltd.** At least one **Singapore-resident director**. A **corporate secretary** (Singapore-resident) is required within 6 months of incorporation. Nominee-director services widely available.
- **Germany GmbH.** No residency requirement for the managing director (**Geschäftsführer**); the Geschäftsführer must be capable of acting for the company in Germany (bank signatures, tax filings), which practically requires either German residency or frequent presence.
- **Netherlands BV.** No director residency requirement. At least one director required. **Substance requirements** for entities claiming Dutch tax residency (real activity in NL) are separate and should be evaluated with a Dutch tax advisor.
- **France SAS.** No president-residency requirement; the president can be a corporate entity or an individual.
- **India Pvt Ltd.** At least two directors; **at least one director must be an Indian resident** (present in India for at least 182 days in the previous financial year — Section 149(3) Companies Act 2013).
- **Japan KK / GK.** No director-residency requirement since 2015 (repealed the prior requirement that at least one director be Japan-resident); however, a Japanese-resident representative or a Japanese address is a practical necessity for tax and bank interaction.
- **Israel Ltd.** No director-residency requirement; local counsel practically required for filing and interaction with the Registrar.

**Nominee directors.** A common practice in Singapore, Ireland, Australia, and other jurisdictions with local-director requirements is to use a professional **nominee director** service — a local individual who serves as a director in name to satisfy statutory requirements, with the operating direction managed by the parent-appointed directors. Nominee directors carry personal statutory liability under local law; ensure the arrangement includes appropriate indemnification (through the local subsidiary and via the D&O policy — see [mod-112 chapter 02](../mod-112-enterprise-risk-insurance-and-compliance/02-startup-insurance-stack-by-stage.md)).

## Local bank accounts and local payroll

**Local bank account.** Nearly every country requires a local bank account for statutory obligations — payroll, tax remittance, social contributions, employer-obligation payments. Opening a local corporate bank account for a foreign-parent subsidiary is one of the slowest steps in the setup timeline; expect **4–12 weeks** and multiple KYC / beneficial-ownership document iterations. Options that shorten the timeline include specialist neobanks (Wise Business, Airwallex, Mercury for the US layer, Revolut Business in-EU); each has its own account-opening constraints and beneficial-ownership thresholds.

**Local payroll.** Local payroll is typically outsourced to a country-specialist provider. Global payroll aggregators (Deel Global Payroll, Rippling Global Payroll, Papaya Global, SD Worx, ADP Streamline) run country-specialist local providers under the hood. Direct engagement with a country-specialist provider is also common (e.g., Sage / IRIS / MHR in the UK, DATEV in Germany, SVEA / Nordea in the Nordics, Ramco / Zoho Payroll in India). Local payroll integrates with local social-insurance filings, statutory pension schemes, and country-specific reporting (real-time PAYE reporting in the UK, DEUV in Germany, DSN in France, Single Touch Payroll in Australia).

## The formation-and-onboarding timeline

A representative 90-to-180-day timeline for a first-country direct-entity setup:

- **Day 0–14: Country and structure decision.** Country selected against drivers 1–4. Entity form confirmed with local counsel. Local counsel and local accountant engaged. Tax advisor engaged for transfer-pricing scoping ([chapter 03](./03-intercompany-and-transfer-pricing-structure.md)).
- **Day 14–45: Formation.** Local counsel prepares constitutional documents; notary appointments (Germany, Netherlands) scheduled; corporate registrations filed. Directors, secretary (where required), UBO / PSC register filings completed.
- **Day 45–90: Registrations.** Tax authority registration (corporate tax, VAT / GST as required, employer-social-insurance-payer registration). Statutory pension / health-insurance registrations (Germany, Netherlands, others). Bank-account application filed and iterating through KYC.
- **Day 60–120: Operational setup.** Local payroll provider onboarded; HRIS integration (Rippling, BambooHR, Deel, others) confirmed; local employment contracts drafted against local law and reviewed by local counsel; local benefits packages (health top-up, statutory pension, statutory leave policies) confirmed; local employee handbook / policy pack (or local addenda to the group handbook) drafted.
- **Day 90–180: First hire onboarded direct.** First direct-employed worker starts; EOR-employed workers (if any) migrated to direct employment through the EOR-run transition or directly (with worker consent). Intercompany services agreement between US parent and new subsidiary signed and effective from the entity's first operating day ([chapter 03](./03-intercompany-and-transfer-pricing-structure.md)).

Timelines slip. Germany GmbH formation with notarial deed and share-capital deposit routinely takes 6–8 weeks; India Pvt Ltd formation takes 2–4 weeks but tax and GST registration take another 4–6 weeks; Singapore Pte Ltd can be incorporated in days but bank-account opening is the bottleneck. Plan for the country-specific slow steps.

## Concrete example — a UK subsidiary for a US Series-B AI startup

A representative first-entity setup for a Series-B US AI-infrastructure startup opening its first UK operations:

- **Country selection.** UK chosen for engineering talent (drivers 1) and EU / European enterprise-sales presence (driver 2). R&D-credit generation (driver 3) is a secondary benefit. IP holding remains in the US parent (driver 4 not triggered at this stage; Pillar 2 not yet applicable at group revenue < €750M).
- **Entity form.** UK **private company limited by shares (Ltd)** under the Companies Act 2006.
- **Directors.** Two directors — the US CFO and the US COO / GC. No UK-resident-director requirement. PSC register lists the US parent as the person with significant control (single 100% shareholder).
- **Local counsel.** UK counsel engaged for formation, employment-contract templates, PIIA / IP-assignment addenda, and the confirmation-statement / annual-accounts cadence.
- **Bank.** Application to a UK high-street bank (e.g., HSBC, Barclays) in parallel with a UK-friendly neobank (e.g., Wise Business) as the operating-day-one bridge.
- **Tax registrations.** HMRC corporation-tax registration (automatic on Companies House incorporation); VAT registration triggered once the £90,000 turnover threshold is crossed (or voluntarily earlier to reclaim input VAT); PAYE / NIC employer registration prior to first UK payroll date. <!-- needs-research: verify current UK VAT registration threshold as of 2025–2026. -->
- **Payroll.** Deel Global Payroll or a UK-specialist provider (e.g., MHR, Sage, IRIS) engaged; real-time PAYE reporting to HMRC via the payroll provider.
- **Employment contracts.** UK employment contracts (indefinite-term, statutory notice, UK-appropriate leave, workplace pension enrolment under the Pensions Act 2008 auto-enrolment regime) drafted by UK counsel and adopted as the UK-employee template. Optional UK EMI stock-option scheme evaluated separately ([chapter 06](./06-international-benefits-and-equity-comp.md)).
- **Intercompany agreement.** US parent and UK Ltd sign a cost-plus intercompany services agreement (typically cost + 8–12% markup for R&D / administrative services — see [chapter 03](./03-intercompany-and-transfer-pricing-structure.md)) effective from the UK Ltd's first operating day.
- **R&D credit.** UK R&D-tax-credit programme designed with UK accountant / tax advisor; project time-tracking, R&D-substantiation documentation, and annual claim cadence stood up as part of the finance calendar.

Timeline: 45 days for the entity, 90 days to first direct UK hire, 6 months to a running UK operation with 5 engineers.

## Summary

- **Four drivers** guide the country-selection decision: engineering-talent supply, GTM presence, research-tax-credit optimisation, and IP-holding-jurisdiction structuring. Every deliberate first-country choice traces to at least one of them.
- **The statutory form** per country is the second decision — UK Ltd, Ireland DAC / Ltd, Canada Federal + provincial, Australia Pty Ltd, Singapore Pte Ltd, Germany GmbH, Netherlands BV, France SAS, India Pvt Ltd, Japan KK / GK, Israel Ltd — each with its own formation, notarial, and share-capital mechanics.
- **Local director, secretary, and statutory-agent requirements** vary sharply — Australian and Singaporean resident-director rules, Indian resident-director rule, Irish EEA-resident-or-bond rule — and drive the practical structuring around nominee arrangements.
- **BEPS 2.0 Pillar 2 (15% global-minimum tax)** does not directly affect a below-€750M startup but should be understood so the structure scales rather than collapses at the threshold.
- **Timeline discipline.** A first-country direct-entity setup takes 90 to 180 days end-to-end; bank-account opening and country-specific formation notarisation are the recurring bottlenecks.
- **This chapter owns the mechanics of standing up the first entity.** [Chapter 03](./03-intercompany-and-transfer-pricing-structure.md) picks up the intercompany-and-transfer-pricing overlay. [Chapter 05](./05-international-employment-law-variance.md) picks up the country-specific employment-law layer.
