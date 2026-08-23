# 1. EOR vs. PEO vs. direct-entity — the international-hiring decision framework

> The first international hire does not require an international entity. The tenth one probably does. The decision framework in between is what separates a working global-workforce programme from an accumulating pile of tax and employment-law exposure.

## Motivation

An early-stage US startup rarely plans to be an international employer. It becomes one the day the CEO signs a candidate the recruiter met at a conference in London, or the day the CTO recommends a former colleague in Warsaw, or the day the head of sales opens a Toronto pipeline that needs a local closer. The question the incoming COO / GC / Head of People inherits at that moment is not "should we go international?" — the question is "how do we legally employ this specific person, starting Monday?"

There are three doors: **Employer of Record (EOR)**, **Professional Employer Organization (PEO)**, and **direct international entity**. Each door opens onto a different tax posture, a different employment-law footprint, a different intellectual-property assignment problem, a different data-privacy exposure, and a different unwind cost. The choice is not fixed at first hire — a country typically starts on the EOR door, and the company moves to a direct entity only when the country-specific headcount, IP, tax, or operational trade-off flips.

This chapter is the decision framework. It defers the specifics of first-entity setup ([chapter 02](./02-first-international-entity-setup.md)), transfer-pricing ([chapter 03](./03-intercompany-and-transfer-pricing-structure.md)), immigration ([chapter 04](./04-us-immigration-programme.md)), employment-law variance ([chapter 05](./05-international-employment-law-variance.md)), and the workforce-reduction playbook ([chapter 08](./08-international-workforce-reduction-playbook.md)) to their respective chapters.

## The three doors

### Door 1 — Employer of Record (EOR)

An **Employer of Record** is a third-party company that is the **legal employer of record** for the worker in the worker's country of residence, on your behalf. The EOR:

- Has (or contracts with) a local legal entity in the worker's country.
- Runs the local employment contract, in the local language, under the local employment-law regime, with all statutory notice / severance / holiday / social-insurance provisions.
- Runs the local payroll, withholds and remits local income tax and social contributions to the local tax authority, and issues the local statutory pay statement.
- Administers or gates local benefits (statutory pension, private health top-up, statutory leave).
- Handles the immigration / work-permit paperwork where the worker is a foreign national in the country of residence.

The client company (you) enters into a **client services agreement** with the EOR under which you pay the EOR (a) the gross local salary, (b) the local employer-side social contributions and mandatory benefits, plus (c) a platform fee. Typical EOR platform fees sit at **US$400–800 per employee per month** — Remote, Deel, Oyster, Rippling EOR, Papaya Global, Velocity Global, Multiplier, and Globalization Partners (G-P) are the widely used platforms; the market is competitive on fees and consolidates regularly. <!-- needs-research: verify current EOR platform-fee benchmarks per employee per month across Remote, Deel, Oyster, Rippling, Papaya, Velocity Global, Multiplier, and G-P — the $400–800 range is the historical benchmark but pricing tiers and country-specific surcharges vary. -->

The client directs the worker's day-to-day work — assignments, priorities, reviews, promotions, compensation changes. The EOR handles the *employment relationship* around that work.

**Where EORs shine:**

- **First-1-to-5-hire countries.** The break-even is entirely against the fixed cost of a direct entity — formation, ongoing local counsel, local accountant, local statutory audit if triggered, local director requirements. For most countries, an EOR is cheaper than a direct entity below roughly 5–10 headcount; the crossover is country-specific ([chapter 02](./02-first-international-entity-setup.md)).
- **Optionality.** An EOR relationship is unwound in weeks; a direct entity takes months to a year to liquidate.
- **Compliance load transfer.** The EOR is on the hook for local employment-law compliance under the client-services contract. The client still has practical exposure — the EOR's contract terms usually let it pass through statutory penalties and give it the right to terminate if the client directs an unlawful action — but the operating burden of tracking every statutory change is transferred.

**Where EORs get expensive or wrong:**

- **Scale.** At 10 headcount in one country, EOR platform fees run US$48k–96k/year on top of gross payroll and employer contributions. A direct entity's fixed operating cost (formation, local accountant, statutory audit) is frequently comparable or lower.
- **IP ownership friction.** The worker is legally employed by the EOR. IP the worker creates for you must be assigned from the EOR (or the worker) to your US parent — this is handled contractually in the EOR client services agreement and the local employment contract, but the arrangement is inspected in Series-A and later diligence and in any subsequent asset acquisition. Some EOR platforms handle IP assignment cleanly; some do not. Read the IP clauses of any EOR agreement before signing.
- **Country-specific limitations.** Some countries limit or prohibit EOR arrangements for certain roles or durations. Germany's Arbeitnehmerüberlassungsgesetz (AÜG) treats EOR-like leased-labour relationships as regulated staffing and imposes duration limits and licensing requirements — an unaware client can find that a long-tenured German worker on an EOR platform has statutorily converted into a direct employee of the EOR, with all that implies. France's requirements around portage salarial and Spain's around empresas de trabajo temporal have similar edges. Confirm the EOR's licence and structural approach country by country.
- **Executive / equity / regulated roles.** Some EOR platforms will not employ officers, directors, or workers with signing authority; some cannot administer local statutory equity-scheme benefits (UK EMI, French BSPCE, Israeli § 102 tracks — see [chapter 06](./06-international-benefits-and-equity-comp.md)). Confirm before hiring.
- **Permanent-establishment risk.** An EOR-employed worker in-country is *usually* not a permanent establishment (PE) of the US parent for tax purposes, but the "usually" turns on the worker's role and authority. A sales worker with signing authority creates PE risk regardless of whether they are direct or EOR-employed; an engineering worker without customer-facing authority typically does not. This is a tax-advisor call ([chapter 03](./03-intercompany-and-transfer-pricing-structure.md)).

### Door 2 — Professional Employer Organization (PEO)

A **PEO** is a US-market construct. Under a **co-employment** arrangement, the client remains the employer of the worker for most legal purposes, but the PEO becomes the co-employer for payroll, tax withholding, and benefits administration. The PEO's aggregated employee base gives the client small-employer access to enterprise-grade benefits pricing (medical, dental, 401(k), workers-comp), plus multi-state payroll and HRIS in a bundled platform.

TriNet, Justworks, Rippling PEO, Sequoia One, Insperity, and ADP TotalSource are the market names. PEO relationships are governed by IRS Certified Professional Employer Organization (CPEO) rules where applicable (Rev. Proc. 2016-33 and successors) and state-by-state PEO licensing statutes.

**PEO is US-only.** A common early-stage error is to treat PEO and EOR as the same product because both platforms bundle payroll and benefits — they are not the same product. PEO is co-employment inside the US market; EOR is sole-employer-of-record in international markets. Many vendors sell both under one brand (Rippling has a PEO and an EOR product; Deel has a US EOR and a global EOR); the products are structurally different.

For the purposes of this module, **PEO is out of scope** — the US-employment layer (worker classification, offer letters, FLSA exempt / non-exempt, state-law variance) is [mod-103](../mod-103-employment-law-and-contract-design/) and the US HR-operations layer (payroll, HRIS, benefits) is [mod-104](../mod-104-hiring-onboarding-and-hr-operations/). PEO is a *tool* those modules recommend for a US company operating across many US states without an in-house benefits team. This module notes only that a PEO does not solve the international-hire problem, and that a company on a US PEO still needs to make the EOR-vs-direct-entity decision the first time it hires outside the US.

### Door 3 — Direct international entity

The client stands up a wholly-owned subsidiary in the country of hire (or in a nearby country that is the group's regional hub). The subsidiary:

- Registers as an employer with the local tax authority and social-insurance bodies.
- Signs the local employment contract with the worker directly.
- Runs its own local payroll (typically outsourced to a local payroll provider — ADP, Ceridian Dayforce, SD Worx, Paychex international, or a country-specific specialist).
- Files local corporate income tax returns, VAT / GST returns, statutory-audit returns where triggered, and any employer-side social-insurance filings.
- Opens local bank accounts, holds the local employment contracts and IP assignments in its own name, and is the counterparty to any local vendor contracts.
- Requires at least the country-mandated local directors / statutory-agent presence (varies by country — see [chapter 02](./02-first-international-entity-setup.md)).

The direct entity is the endpoint every scale-up eventually reaches in every country where it maintains meaningful headcount. It is the correct answer once (a) the headcount justifies the fixed operating cost, (b) IP or tax structuring demands local entity ownership, (c) the country's EOR regime is unfavourable, or (d) the operational profile (customer contracting, regulated activity, ownership of local assets) requires it.

## The decision framework

For each country in which the company will have workers, answer the following questions in order:

### Question 1 — how many workers, on what horizon?

- **1–5 workers, no plan to exceed 5 in 12 months:** **EOR by default.** The direct-entity fixed cost is not yet earned.
- **5–10 workers, growing:** **EOR still viable; start planning the entity.** Break-even math is country-specific; run it explicitly. Include in the direct-entity cost side the local formation fees, ongoing local accountant, local statutory audit (if triggered by size), local counsel retainer, and the transfer-pricing documentation lift ([chapter 03](./03-intercompany-and-transfer-pricing-structure.md)). Include on the EOR side the fully-loaded platform fees at projected headcount.
- **10+ workers, or clear line-of-sight to 10+:** **Direct entity is almost always the right answer.** Continue existing EOR relationships if operationally convenient, but stand up the entity and migrate new hires directly.
- **Any single officer, director, or country-general-manager hire:** **Direct entity, regardless of headcount.** EORs generally will not employ officers, and the country GM's authority to bind the group is easier to structure through a direct subsidiary.

### Question 2 — does the country's regulatory regime disfavour EOR?

Four country patterns tip the answer toward direct entity earlier than headcount alone would suggest:

- **Germany — the AÜG limit.** Germany's Arbeitnehmerüberlassungsgesetz treats leased labour as a regulated construct and imposes an **18-month maximum** on a single worker's assignment to a client via a licensed staffing arrangement (with limited collective-agreement variance). Long-tenured German workers on EOR platforms carry statutory-conversion risk; some EORs address this via alternate structures, but the compliance path is fragile. Plan for a German subsidiary when the intent is more than a short-term hire.
- **Germany — the Betriebsrat trigger.** German operations with **5 or more permanent employees** are entitled to elect a **works council (Betriebsrat)** under the Betriebsverfassungsgesetz (BetrVG). Once a works council exists, its co-determination rights over working time, hiring, dismissal, and social matters are legally binding on the employer. If the target German operations will exceed 5 employees, plan the direct entity — an EOR arrangement does not eliminate the Betriebsrat right if the workers' community-of-interest test is met, and the compliance friction is easier to manage as the direct employer. See [chapter 05](./05-international-employment-law-variance.md).
- **France — CDI vs. CDD.** France's default employment contract is the **CDI (contrat à durée indéterminée)** — indefinite-term, with statutory notice and severance on termination. **CDD (contrat à durée déterminée)** — fixed-term — is available only in enumerated cases and carries a 10% end-of-contract precarity indemnity. EORs default to CDI for the worker's benefit; the client should confirm the contract type and the reason for any CDD. France also imposes a **portage salarial** regulatory regime for umbrella-employment structures that some EORs use; confirm the EOR's structural approach.
- **UK — IR35 and the off-payroll working rules.** For workers engaged as *contractors* through their own personal-service company (PSC) — a "Ltd" — HMRC's off-payroll working rules (Chapter 10, Part 2, ITEPA 2003, as amended) shift the tax-status determination and, in the medium-to-large-client case, the withholding obligation to the client. A US company engaging a UK contractor through their own Ltd must run an IR35 status determination and, if the engagement is deemed inside IR35, deduct PAYE and NICs as though the contractor were an employee. IR35 exposure is one of the recurring "we thought this was a contractor" surprises for US companies operating in the UK — the direct-EOR / employee route is cleaner where the working pattern looks employment-like.
- **Canada — provincial variance.** Canadian employment law is **provincial**, not federal (except for federally-regulated sectors — banking, telecom, interprovincial transport, some others). An Ontario employee is governed by the Ontario Employment Standards Act, 2000; a Quebec employee by the Act respecting labour standards (LSA); a British Columbia employee by the Employment Standards Act. Each province has its own notice / severance / statutory holiday regime, and Quebec adds a distinct language-of-work regime under the Charter of the French Language (Loi 96 as amended). Direct-entity registration in Canada is typically per-province in addition to the federal incorporation.

### Question 3 — is there an IP, tax, or regulatory reason to hold the local relationship directly?

- **IP ownership.** IP created by an EOR-employed worker must flow up to the US parent contractually. The chain — worker → EOR → client US parent — is inspected at diligence. For workers in senior technical roles or roles creating patentable inventions, a direct subsidiary employment relationship is cleaner.
- **Local R&D tax-credit generation.** The UK R&D tax credit (RDEC / SME schemes), Canada's SR&ED, France's CIR, and Ireland's R&D credit generally require that qualifying R&D expenditure sit in a local corporate taxpayer. EOR-employed workers do not generate qualifying R&D expenditure for the US parent under most local regimes. If the country is being chosen partly for its research-tax-credit regime, plan the direct entity from day one ([chapter 02](./02-first-international-entity-setup.md) and [chapter 03](./03-intercompany-and-transfer-pricing-structure.md)).
- **Local customer contracting.** If the group needs to sign revenue contracts in the local jurisdiction (public sector customers frequently require it; regulated industries frequently require it; some enterprise customers demand it), a direct local entity is required.
- **Regulated activity.** A regulated licence (financial services, medical devices, data-processing under a national data-protection authority, telecoms) is held by a licensed entity in the jurisdiction — not by an EOR.

### Question 4 — what is the exit cost?

- **EOR exit.** Termination of the client-services agreement plus wind-down of the local employment relationships through the EOR — the EOR runs the local statutory notice / severance and the worker is either terminated, transferred to a new EOR / direct entity, or converted to a direct employee. Weeks-to-months, driven by the local statutory notice.
- **Direct-entity exit.** Terminate the employees under local employment law (which is much harsher than at-will in most jurisdictions — see [chapter 05](./05-international-employment-law-variance.md) and [chapter 08](./08-international-workforce-reduction-playbook.md)); close the local tax registrations; file the final corporate-tax return; publish any statutorily-required creditor notices; liquidate the entity through local statutory dissolution. Months-to-years. A German GmbH liquidation, for example, is not a same-year exercise. Plan the entity assuming a multi-year commitment.

## The country-first-hire playbook

The default operating playbook for the first hire in a new country:

1. **Confirm the role, the country of residence, and the expected 12-month headcount trajectory.** The trajectory drives everything downstream.
2. **Run the four framework questions** with the CFO, the GC / Head of People, and the founder sponsor of the hire. Document the reasoning in a one-page decision memo, filed to the corporate record.
3. **If EOR: select the EOR platform.** Existing platform if you already have one; a comparison exercise if not. Confirm the platform's country coverage, IP-assignment clause, executive / equity-plan handling, and any country-specific structural notes (Germany AÜG, France portage salarial, UK IR35).
4. **Draft the client-services agreement additions.** Confirm the platform's default IP-assignment language is defensible; add supplemental IP-assignment or restrictive-covenant language to the local employment contract if the platform allows it (some do, some do not).
5. **Coordinate with the US-side employment layer** ([mod-103](../mod-103-employment-law-and-contract-design/) and [mod-104](../mod-104-hiring-onboarding-and-hr-operations/)) so the international worker is set up in the HRIS, gets equipment provisioning, security onboarding, and the standard offer-communication treatment consistent with the US workforce.
6. **Screen the individual against sanctions and export-control lists** — [mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md). International hires increase FCPA and sanctions exposure; the screening is not optional.
7. **Set a review checkpoint.** Ninety days into the relationship, reconfirm the EOR platform is working; ninety days before hitting the country's break-even headcount, begin the direct-entity planning.

## Concrete example — a Series-B AI-infrastructure startup goes international

A representative trajectory for a Series-B US AI-infrastructure company hiring outside the US for the first time:

| Country | Trigger | Door | Rationale |
|---|---|---|---|
| Canada (Ontario) | Two senior ML engineers, referrals from a founder | **EOR** initially, **direct entity within 6 months** | Trajectory to 5+ engineers is credible; SR&ED tax-credit generation is meaningful; direct Ontario employment law is manageable. |
| UK | One enterprise-sales lead based in London | **EOR** | Single hire; UK EMI equity plan not required at this stage; direct-entity planning if the sales function grows to 3+. |
| Germany | One senior ML researcher relocated from a US university | **Direct entity (GmbH)** planned; **EOR bridge** during formation | AÜG duration limit disfavours long-tenure EOR; researcher's IP contribution is central; German subsidiary is planned for the R&D team. |
| India | Six-person offshore engineering team | **Direct entity (Pvt Ltd)** | Headcount is well past EOR break-even from day one; India transfer-pricing and STPI / SEZ structuring benefits from direct entity. |
| Poland | One senior engineer, first in the country | **EOR** | Single hire; direct-entity trigger deferred. |
| Israel | One founder-referral AI researcher | **EOR (with § 102 equity-plan compatibility)** or **Direct entity** | Trigger the direct-entity conversation if the § 102 track is central to the offer package ([chapter 06](./06-international-benefits-and-equity-comp.md)). |

The decision is not one framework applied once. It is applied per country, revisited annually, and re-run whenever a country crosses a headcount, tax, or operational trigger.

## Summary

- **Three doors.** EOR (third-party employer of record in the worker's country); PEO (US-only co-employment); direct international entity (wholly-owned subsidiary in country). PEO does not solve the international-hire problem.
- **EOR is the default for the first 1–5 hires** in any new country, subject to country-specific regulatory disqualifiers (Germany AÜG, France portage, UK IR35 for contractor engagements).
- **Direct entity becomes right** as headcount grows past the country-specific break-even (typically 5–10), when IP / R&D-credit / regulated-activity / local-contracting reasons require it, or when a country-GM or officer role forces a direct employment relationship.
- **The framework is four questions:** headcount trajectory, regulatory regime, IP / tax / regulatory posture, and exit cost. Answer them country-by-country, revisit annually, and document the reasoning at the moment the decision is made.
- **This chapter owns the decision.** [Chapter 02](./02-first-international-entity-setup.md) owns the mechanics of standing up the first direct entity; [chapter 03](./03-intercompany-and-transfer-pricing-structure.md) owns the intercompany-and-transfer-pricing overlay; [chapter 05](./05-international-employment-law-variance.md) owns the employment-law variance that shapes every step.
