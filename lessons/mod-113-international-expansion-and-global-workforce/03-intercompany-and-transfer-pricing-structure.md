# 3. Intercompany and transfer-pricing structure

> Every dollar that moves between the US parent and an international subsidiary is a transfer-pricing event, whether it is documented as one or not. The design decision is not whether to have a transfer-pricing structure — it is whether the structure will be legible under audit or be reconstructed by an auditor with the benefit of hindsight.

## Motivation

The moment an international subsidiary exists, three things become true. First, the US parent and the subsidiary are **related parties** for tax purposes in both jurisdictions. Second, every transaction between them — a services fee, an IP royalty, a cost reimbursement, a cash transfer, a management-fee allocation, a loan — must be priced as if the parties were dealing at arm's length (IRC § 482 in the US; the OECD Transfer Pricing Guidelines and each country's local implementation abroad). Third, both jurisdictions will eventually ask to see the documentation supporting the pricing — and the burden of proof is on the taxpayer.

For a startup, this is one of the areas where the substance is highest and the pattern is most standardised. The startup does not need to invent a novel intercompany structure; it needs to implement a well-understood cost-plus-services pattern, document it properly, and run it on a repeatable annual cadence. This chapter frames the structure so the incoming COO / GC / CFO can direct the specialist tax advisors and read the resulting agreements with informed judgment.

**Ownership boundary before we begin:** this chapter frames the intercompany-and-transfer-pricing programme at the level a startup operator needs to understand. Detailed structuring — country-by-country transfer-pricing documentation packages, comparable-company analyses, advance-pricing agreements (APAs), cost-sharing arrangements under Treas. Reg. § 1.482-7, IP-migration structures, and the tax-effective corporate structure of an eventual pre-IPO group — is **specialist advisor territory**. The names commonly retained in this practice area are **Big 4 tax practices** (Deloitte, EY, KPMG, PwC), **Baker McKenzie**, **Fenwick & West**, **DLA Piper**, and **specialist transfer-pricing boutiques**. This module trains the operator to run the relationship; it does not replace the advisor.

## Why arm's-length pricing exists

Related parties can, in principle, transact at any price. If the US parent charges its Irish subsidiary a $1 fee for services worth $10, the effect is to shift $9 of pre-tax profit from the US to Ireland; at differential tax rates, this converts economic profit into tax savings. Every tax jurisdiction operates transfer-pricing rules to prevent that arbitrage.

The controlling principle globally is the **arm's-length standard**: related parties must transact on the terms and prices that unrelated parties would agree to in comparable circumstances. The principle is codified in **IRC § 482** and the extensive regulations at **Treas. Reg. §§ 1.482-1 through 1.482-9**, and mirrored in the **OECD Transfer Pricing Guidelines for Multinational Enterprises and Tax Administrations** (2022 edition) that most non-US jurisdictions have adopted directly or by reference.

The consequence for a startup: intercompany prices must be defensible against the arm's-length standard, and documentation must show the analysis that supports the chosen price.

## The startup-default intercompany structure

For an early-stage US-parented group with international subsidiaries that primarily conduct **routine functions** (R&D services, sales / marketing support, administrative services), the standard structure has three moving parts.

### Part 1 — cost-plus services agreement

The international subsidiary is characterised as a **routine service provider** to the US parent. It performs functions (engineering, sales support, administration) on behalf of the group at the parent's direction, and is compensated on a **cost-plus** basis — the subsidiary's operating costs plus a markup.

Typical markup ranges:

- **R&D services (engineering, ML research, product development):** cost + **8% to 12%** is the historical benchmark range for early-stage groups. The exact markup should be supported by a comparable-company analysis (benchmarking against unrelated companies performing similar routine R&D services), typically produced by the tax advisor. Cost + 10% is the frequently-used mid-point in the absence of company-specific benchmarks.
- **Administrative services (finance, HR, IT support):** cost + **5% to 10%** is the historical benchmark range. Slightly lower than R&D services because the risk profile of the service provider is lower.
- **Sales and marketing support (lead generation, sales-support, business-development without contract-signing authority):** cost + **5% to 8%** is a historical benchmark, with wider variance depending on the exact activities. If the international entity signs revenue contracts and books local revenue, the structure shifts from cost-plus-services to a **buy-sell distributor** or **commissionaire** structure with different transfer-pricing characterisation — a specialist call.

<!-- needs-research: verify the current OECD-benchmark markup ranges for cost-plus R&D and administrative services against the latest OECD Transfer Pricing Guidelines and current published comparable-company benchmark studies. The 8–12% R&D range is the historical practitioner benchmark but should be reconfirmed against current comparables. -->

**What "cost" means.** The cost base is the subsidiary's fully-loaded operating cost — direct labour (salaries, bonuses, employer social contributions, benefits), directly-attributable overhead (rent, IT, local depreciation), and a reasonable allocation of indirect overhead. Cost typically **excludes** stock-based compensation for arm's-length pricing purposes (though this is a jurisdictional judgment call; the US Tax Court's *Altera Corp. v. Commissioner*, 926 F.3d 1061 (9th Cir. 2019), addressed the treatment of SBC in cost-sharing arrangements — with a different but related answer).

**Practical mechanics.** The US parent invoices the international subsidiary monthly (or the subsidiary invoices the US parent, depending on the direction of services). Amounts are settled via intercompany cash transfers on a documented cadence — monthly, quarterly, or annually with a running intercompany balance. The intercompany balance is trued-up annually against the actual cost-plus calculation.

### Part 2 — intercompany services agreement (ICSA)

The cost-plus arrangement is memorialised in a **written intercompany services agreement (ICSA)** signed between the US parent and each international subsidiary. The agreement:

- Identifies the parties and their affiliation.
- Defines the services provided (routine R&D, administrative, sales-support — as applicable).
- Specifies the compensation methodology (cost + N% markup on a defined cost base).
- Documents payment terms and settlement cadence.
- Includes standard commercial terms: term and termination, confidentiality, IP-assignment (see part 3), governing law, dispute resolution.
- Confirms that the services are performed **on behalf of the parent as the principal risk-taker** — an important characterisation point for the cost-plus treatment.

A signed ICSA effective from the subsidiary's first operating day is a baseline diligence expectation. Absence of an ICSA (or a backdated ICSA drafted retroactively for diligence) is a common finding on early-stage-startup diligence checklists and creates unnecessary friction at every subsequent financing.

### Part 3 — IP ownership and licensing

For a group whose IP is held by the US parent — the startup-default — the international subsidiaries do **not** own IP. IP created by international subsidiary employees is **assigned** to the US parent through:

- **Employment-contract IP assignment** in the local employment contract (drafted by local counsel with the specific IP-assignment language required to be enforceable under local employment / IP law). This is one of the practical reasons the local employment contract is not the EOR platform's default template but a local-counsel-reviewed template.
- **Present-assignment language** analogous to the US employee PIIA ([mod-103 chapter 04](../mod-103-employment-law-and-contract-design/04-employee-piia.md)), adjusted to the local IP-law regime (UK Copyright, Designs and Patents Act 1988 s. 11(2) for employer ownership of employee-created IP; German ArbnErfG for employee-invention entitlement; French Code du travail L. 611-7 for employee inventions; each has its own default rules that require deliberate override or supplementation).
- **Intercompany IP-assignment agreement** between the subsidiary and the US parent covering IP created by the subsidiary's operations. The agreement flows created IP up to the parent; the parent grants back a limited licence to the subsidiary as necessary for the subsidiary to perform its cost-plus services.

**Where the group does implement a formal IP-licence or royalty structure** (post-Series-C IP-holding jurisdiction; specific product line held in a separate IP-holding entity), the structure requires its own transfer-pricing analysis (the royalty rate must be arm's-length), its own agreements, and its own documentation. This is specialist-advisor territory; the operator's job is to ensure the arrangement is documented, signed, and effective from the first day the underlying transactions occur.

### The employee-invention regime by country — a very quick tour

- **United Kingdom.** Under the Copyright, Designs and Patents Act 1988 s. 11(2), copyright in a literary, dramatic, musical, or artistic work created by an employee in the course of employment vests in the **employer** by default. Under the Patents Act 1977 s. 39, patentable inventions made by an employee "in the course of the normal duties" belong to the employer, with a compensation entitlement for the employee where the invention is of "outstanding benefit" (s. 40).
- **Germany.** The **Arbeitnehmererfindungsgesetz (ArbnErfG)** requires the employee to notify the employer of a service invention (Diensterfindung); the employer must claim the invention within four months of notification, upon which title transfers to the employer. If the employer claims the invention, the employee is entitled to **statutorily-calculated compensation** (Vergütungsrichtlinien) — a real, ongoing obligation that must be tracked.
- **France.** Under the Code du travail L. 611-7 and Code de la propriété intellectuelle L. 611-1, inventions made by an employee in the course of an employment contract with an inventive mission belong to the employer, subject to statutorily-required "additional remuneration" (rémunération supplémentaire) — again, a real obligation.
- **Netherlands.** Article 12 of the Netherlands Patent Act 1995 vests inventor rights in the employee unless the employer has been "assigned" the invention by nature of the employment relationship; in practice, employment contracts contain explicit invention-assignment provisions.
- **Israel.** Section 132 of the Patents Law, 5727-1967, provides that inventions made by an employee in the course of employment belong to the employer, but Israeli law recognises a distinct **employee-invention compensation** entitlement, made prominent by the Supreme Court decision in *Barazani v. Israel* (Committee for Compensation and Royalties, 2014); careful contract drafting is required to manage the exposure.

The practical implication: **do not rely on US-default assumptions about employer ownership of employee inventions in international subsidiaries.** Local counsel must draft the local employment-contract IP-assignment language to be effective under local law, and country-specific inventor-compensation entitlements (Germany, France, Israel) must be understood and either satisfied on the compensation stack or contractually addressed.

## Documentation — what needs to exist, and where

Transfer-pricing documentation is a global compliance obligation with a jurisdiction-specific overlay.

- **Master File and Local File.** The OECD's BEPS Action 13 introduced the standardised **Master File** (high-level information about the group's global operations, transfer-pricing policies, and financial allocations) and **Local File** (transactional analysis for the specific country) framework. Adopted by most jurisdictions with implementing rules. Thresholds and formats vary — typically triggered by group or local-entity revenue exceeding a country-specific threshold. <!-- needs-research: verify the OECD Model Master File / Local File thresholds and jurisdiction-by-jurisdiction implementation status as of 2025–2026. -->
- **US Section 6662(e) transfer-pricing documentation.** Contemporaneous transfer-pricing documentation prepared by the return-due-date can protect against **§ 6662(e) transfer-pricing penalties** (up to 40% for substantial or gross valuation misstatements). Document types recognised under the regulations at Treas. Reg. § 1.6662-6(d). A US-parented group with international subsidiaries should prepare US-side transfer-pricing documentation annually.
- **Country-by-Country Reporting (CbCR).** BEPS Action 13 also introduced **Country-by-Country Reporting** for MNE groups with consolidated revenue of **€750M or more**. Groups above the threshold file the CbCR (annual, per-country breakdown of revenue, profit, tax paid, employees, tangible assets) with their home tax authority, which exchanges the report with other participating jurisdictions. Below the threshold, CbCR does not directly apply — but the reporting infrastructure typically becomes necessary as a group approaches the threshold.
- **Local country documentation.** Individual countries have their own transfer-pricing documentation and disclosure rules that layer on top of the OECD framework. Germany's Ordnungsmäßigkeit rules, France's declaration 2257-SD, Australia's IDS (International Dealings Schedule), and India's Form 3CEB are examples. Local advisors track the country-specific requirements.

**Practical cadence for a startup:**

- **Annually**, produce or refresh the transfer-pricing documentation for each subsidiary (US Section 6662(e) documentation, OECD Local File equivalent where required). The tax advisor typically drives this; the finance team provides the underlying cost data.
- **On material changes** (new intercompany services, new subsidiary, new IP-holding arrangement, change in functional profile), refresh the documentation contemporaneously with the change.
- **On approach to CbCR-threshold**, plan the CbCR infrastructure at least 12 months before the year in which the group is expected to cross €750M — the reporting is retrospective and requires clean per-country data.

## Permanent-establishment (PE) risk

**Permanent establishment (PE)** is the tax concept that says a foreign company doing business in a country in a sufficiently substantial way is treated as having a taxable presence there — with income attributable to the PE taxable in the source country. Every income-tax treaty and every non-treaty country has a version of the PE concept; the OECD Model Tax Convention Article 5 is the reference.

The exposure for a US company hiring internationally:

- **A fixed place of business** in the country (a leased office, a warehouse, a factory, a permanent home-office presence with a defined role) generally creates PE.
- **A dependent agent with authority to conclude contracts** on behalf of the US company generally creates PE, regardless of whether a fixed place of business exists. A sales employee — direct or EOR-employed — with authority to sign or negotiate to signature contracts on behalf of the US parent creates PE risk in the country of residence.
- **Independent agents** operating in the ordinary course of their business do not create PE — but a "sales consultant" whose only client is the US parent and who negotiates deals on the parent's behalf is unlikely to qualify as an independent agent under scrutiny.
- **Home-office-only R&D workers** without customer-facing authority and without contract-signing authority typically do not create PE — but the analysis is jurisdictional. The **BEPS Action 7** revisions to the OECD Model tightened the definition and reduced some historical exemptions.

The practical implications:

- **Before the first sales hire in a country, run the PE analysis.** The tax advisor evaluates the role, the authority structure, the compensation model, and the customer-contract mechanics.
- **Structure the local entity's role deliberately.** A direct international subsidiary that is a cost-plus service provider does not itself trigger US-parent PE in the country — the subsidiary is the local taxable entity, and the parent's income is protected by the subsidiary interposing itself. This is one of the practical reasons to move from EOR to direct subsidiary as sales operations expand: the direct entity's local-tax residency contains the PE exposure.
- **Document the position.** The tax advisor's PE analysis for each new market is a durable record. It supports the group's position under a subsequent local audit and informs any future APA (advance pricing agreement) discussion.

## BEPS 2.0 Pillar 1 and Pillar 2 — the compressing frame

The OECD's BEPS 2.0 project has two pillars that reshape the tax structuring landscape and that startups should understand at the level of "when will these apply to us."

- **Pillar 1 — Amount A.** Reallocates a portion of the largest MNEs' residual profit to market jurisdictions based on where sales are made, independent of physical presence. Applies to MNE groups with global revenue **above €20 billion** and profit margins above 10%. **Not relevant for startups** for the foreseeable future.
- **Pillar 2 — Global Minimum Tax (15%).** Imposes a **15% effective-tax-rate (ETR) floor** on MNE groups with consolidated revenue of **€750M or more**, implemented country-by-country through the **Income Inclusion Rule (IIR)**, the **Undertaxed Profits Rule (UTPR)**, and **Qualified Domestic Minimum Top-up Taxes (QDMTT)**. Effective dates vary by implementing jurisdiction; most of the EU applies IIR / QDMTT to fiscal years starting on or after December 31, 2023, and UTPR one year later. <!-- needs-research: verify current implementation status of EU Pillar 2 Directive, UK Multinational Top-up Tax / Domestic Top-up Tax, Ireland's Pillar 2 implementation, and the US treatment of QDMTT credits and IIR interaction with GILTI as of the current period. -->

**Practical implications for a below-€750M startup:**

- **Pillar 2 does not directly apply.** Existing low-tax-jurisdiction structures continue to function under legacy rules.
- **Design with graduation in mind.** Structures whose value depends on effective tax rates below 15% will lose that value once the group crosses the threshold. If the group's expected growth trajectory points at €750M consolidated revenue within a foreseeable planning horizon (say, three-to-five years), IP-holding-jurisdiction and low-tax-hub restructuring at Series C / Series D should assume a Pillar-2 outcome.
- **Reporting infrastructure.** Groups approaching the threshold need CbCR-quality data infrastructure (per-country revenue, profit, tax paid, employees, tangible assets) 12–24 months before crossing.
- **Model the Pillar 2 outcome** as part of any structuring analysis. A specialist tax advisor should include the Pillar-2 outcome in every recommendation from Series B onwards, even if the group is currently below threshold.

## Concrete example — a US-parent / UK-sub cost-plus structure

A representative first-year intercompany structure for a Series-B US AI-infrastructure startup with a newly-formed UK Ltd subsidiary of 5 engineers:

- **Characterisation.** UK Ltd is a routine R&D services provider to the US parent.
- **Pricing.** Cost + **10% markup** (mid-point of the 8–12% benchmark range, supported by a UK-focused comparable-company benchmark prepared by the tax advisor).
- **Cost base.** UK Ltd's fully-loaded UK operating cost — engineer salaries + employer NIC + auto-enrolment pension contributions + benefits + directly-attributable overhead (UK office rent, UK IT, UK legal/accounting).
- **Intercompany services agreement.** Signed between US parent and UK Ltd effective from UK Ltd's first operating day; specifies the services (routine R&D), the pricing (cost + 10%), settlement terms (monthly invoicing, quarterly cash settlement), and IP-assignment (UK Ltd assigns all IP to US parent through the ICSA and reinforced in the local employment contracts).
- **IP.** UK Ltd employees' invention-assignment addressed in the local employment contract drafted by UK counsel, reinforced in the ICSA with a group-wide assignment from UK Ltd to US parent. US parent grants UK Ltd a limited operating licence to use the group's IP as necessary to perform the routine R&D services.
- **Documentation.** US-side Section 6662(e) transfer-pricing documentation prepared annually by the tax advisor; UK-side documentation prepared to HMRC's requirements; comparable-company benchmark refreshed on a rolling three-year cadence.
- **PE analysis.** No sales-signing employees in the UK; UK Ltd is the local taxable entity; US-parent PE risk in the UK is minimal.
- **R&D credit.** UK R&D-tax-credit claim run annually against qualifying UK Ltd R&D expenditure. Project time-tracking and R&D-substantiation infrastructure operated by the UK finance / operations team with support from the UK accountant.
- **Pillar 2.** Not applicable at current group revenue; deferred to a future planning cycle.

The structure is prosaic, well-understood, and inspectable. It is exactly what the tax advisor recommends and what Series-C diligence will expect to find.

## Anti-patterns

- **Undocumented intercompany balances.** Cash moves from parent to subsidiary "as needed" without invoices, without an ICSA, without transfer-pricing documentation. Every dollar is a transfer-pricing exposure and none of it is defensible.
- **Backdated agreements.** Documents drafted retroactively — an ICSA "effective January 1" but signed the following December — invite audit questions and create diligence discomfort. Sign agreements contemporaneously with the underlying activity.
- **US-parent-only-thinking on employee IP.** Assuming the US "work for hire" doctrine (or the US-style PIIA) applies globally. It does not. Local IP-assignment law drives the local contract language.
- **Ignoring inventor-compensation entitlements** (Germany ArbnErfG, France, Israel). A German employee-inventor claim can attach years after the invention; the group's exposure needs to be surfaced when the invention is created, not litigated years later.
- **"We're too small for transfer pricing."** Every intercompany transaction is a transfer-pricing event. Small groups can use simple documentation; they cannot skip documentation entirely.
- **Aggressive structuring without advisor support.** IP-migration structures, cost-sharing arrangements, and low-tax-hub structures are specialist-tax territory. A startup that self-serves an aggressive structure without advisor support buys the audit risk without the audit-defence support.

## Summary

- **Every intercompany transaction is a transfer-pricing event** priced under the arm's-length standard (IRC § 482 in the US, OECD Guidelines globally).
- **The startup default** is a cost-plus intercompany services structure — the subsidiary performs routine R&D or administrative services for the US parent at cost + markup (typical benchmark 8–12% for R&D services, 5–10% for administrative services).
- **The intercompany services agreement (ICSA)** is the load-bearing document; sign it contemporaneously with the subsidiary's first operating day.
- **IP flows to the US parent** through local employment-contract IP-assignment (drafted for local IP-law effectiveness) reinforced by intercompany IP-assignment; know the country-specific employee-invention-compensation regimes (Germany ArbnErfG, France, Israel).
- **Documentation cadence:** US Section 6662(e) documentation annually; OECD Master File / Local File where thresholds triggered; Country-by-Country Reporting at €750M+ consolidated revenue.
- **Permanent-establishment risk** attaches primarily to sales-with-authority roles; direct international subsidiaries contain PE exposure by acting as the local taxable entity.
- **BEPS 2.0 Pillar 2 (15% global-minimum tax)** applies at €750M+ consolidated revenue; design structures to scale through the threshold rather than collapse into it.
- **Defer detailed structuring to specialist tax advisors** (Big 4 tax, Baker McKenzie, Fenwick, DLA Piper, transfer-pricing boutiques). The operator's job is to run the relationship, sign the agreements, and maintain the documentation cadence.
