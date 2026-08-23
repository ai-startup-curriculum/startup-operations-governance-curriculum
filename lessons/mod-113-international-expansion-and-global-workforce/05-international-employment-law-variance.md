# 5. International employment-law variance

> The single most important thing to know about international employment law is that **US at-will employment is a rare exception globally**. In most of the world, terminating an employee requires cause or severance or both, on a statutory notice period the employer does not get to shorten by contract.

## Motivation

A US-native operator's default assumptions about the employment relationship — at-will, terminable with no cause on no notice, few statutorily-mandated benefits, minimal termination formalities — do not translate outside of the US. Every country outside the US operates on some version of a **cause-required-or-severance-required-or-both** default; most operate a statutory notice period; most operate a statutory paid-leave floor; many operate a works-council or employee-representative overlay that inserts a co-decision-maker into termination and workforce-change decisions.

The consequence is that international employment relationships are structurally more expensive to end than to begin. A US layoff at a US company happens in a day; a French layoff at a French subsidiary happens over months, requires a *plan de sauvegarde de l'emploi (PSE)* if it exceeds a threshold, and produces statutorily-calculated severance and re-employment obligations. The exec-team compensation package a US-only company can offer to a US executive would be non-compliant if offered to a German executive under German law.

This chapter surveys the employment-law variance the incoming COO / GC / Head of People must operate against, focused on the five markets most likely to be the first international footprint: **United Kingdom, Germany, France, Canada, Australia**. It builds the framework the workforce-reduction playbook ([chapter 08](./08-international-workforce-reduction-playbook.md)) applies. Non-US countries not covered here (Netherlands, Ireland, Spain, Poland, Israel, India, Japan, Singapore) follow analogous patterns but with their own specifics that require local-counsel review.

**Ownership boundary before we begin:** this chapter owns the **international-employment-law variance layer**. It defers to [mod-103](../mod-103-employment-law-and-contract-design/) for the US-side employment-law layer and to [chapter 08](./08-international-workforce-reduction-playbook.md) for the reductions-playbook operationalisation.

## The at-will spectrum

Employment relationships globally can be ordered on an at-will spectrum from most flexible to most protected. A rough ordering:

- **United States (except Montana).** At-will by default — the employment relationship can be terminated by either party at any time, with or without cause and with or without notice, subject to specific state-law and federal-law exceptions (public-policy, implied-contract, covenant-of-good-faith, WARN Act, discrimination, retaliation). Montana operates under the Wrongful Discharge from Employment Act (MCA § 39-2-901), which requires good cause after a probationary period.
- **Canada.** **Common-law reasonable notice** on top of statutory minimums. No US-style at-will; termination without cause requires notice (or pay in lieu) calculated as the greater of the provincial statutory minimum or the common-law reasonable-notice period (which varies with age, tenure, position, and re-employment prospects — the *Bardal v. Globe & Mail* factors).
- **Australia.** No at-will; **unfair dismissal** framework under the Fair Work Act 2009 protects most employees after a qualifying employment period (6 months for most employers, 12 months for small businesses under the Small Business Fair Dismissal Code).
- **United Kingdom.** No at-will; **unfair dismissal** protection under the Employment Rights Act 1996 after 2 years' continuous employment, with statutorily-required notice and consultation obligations.
- **Germany.** No at-will; **Kündigungsschutzgesetz (KSchG)** protects employees after 6 months' service in businesses with more than 10 employees, requiring one of the enumerated cause grounds — personal, conduct, or operational. **Works-council co-determination** overlays.
- **France.** No at-will; **Code du travail** requires cause and procedural formality; **CDI (indefinite-term)** is the default contract; **PSE (plan de sauvegarde de l'emploi)** and **CSE (comité social et économique)** consultation overlays.

The framework this chapter uses is: for each country, walk (a) **default contract type**, (b) **statutory notice period on termination**, (c) **termination-protection regime**, (d) **works-council / representative obligations**, (e) **statutory paid-leave floor**, and (f) any country-specific quirks the operator must know.

## United Kingdom

**Governing law:** Employment Rights Act 1996; Equality Act 2010; Working Time Regulations 1998; Trade Union and Labour Relations (Consolidation) Act 1992; multiple secondary regulations.

**Default contract type.** Indefinite-term written contract (though a written statement of particulars is the specific statutory requirement — section 1 ERA 1996). Fixed-term contracts permitted; conversion to permanent status after four years of successive fixed-term contracts without objective justification (Fixed-term Employees (Prevention of Less Favourable Treatment) Regulations 2002).

**Statutory notice on termination.** Section 86 ERA 1996:
- Employer to employee: **1 week** notice after 1 month's service, increasing by **1 week per year of service** to a **maximum of 12 weeks** after 12 years.
- Employee to employer: **1 week** notice after 1 month's service.
- Contractual notice periods commonly exceed statutory minimums, particularly for senior roles (typical: **1 month to 6 months** for professional roles; **6 months to 12 months** for executive roles).

**Termination protection.** Unfair dismissal protection after **2 years' continuous employment** (Employment Rights Act 1996 s. 108). Dismissal must be for one of the enumerated potentially-fair reasons — capability, conduct, redundancy, statutory illegality, or "some other substantial reason" — and the employer must follow a fair process (ACAS Code of Practice on Disciplinary and Grievance Procedures). Awards for unfair dismissal include a basic award (calculated on age × service × weekly pay) plus a compensatory award (subject to a statutory cap — currently around £115k). <!-- needs-research: verify current statutory compensatory-award cap under s. 124 ERA 1996 for 2025–2026. -->

**Redundancy specifics.**
- Statutory **redundancy pay** for employees with 2+ years' service: age-and-service-weighted formula capped at a statutory weekly-pay cap.
- **Collective consultation.** Where the employer proposes to dismiss **20 or more employees at one establishment within a 90-day period**, the employer must consult with employee representatives (or a recognised trade union) for a minimum period — **30 days** for 20–99 proposed dismissals, **45 days** for 100+ (TULRCA 1992 s. 188). Failure carries **protective award** liability of up to 90 days' pay per affected employee.
- HR1 filing to the Insolvency Service required for collective redundancies (100+ proposed dismissals require prior notification).

**Statutory paid leave.** **28 days paid annual leave** (including or in addition to public holidays, depending on the contract) under the Working Time Regulations 1998 for full-time workers (5.6 weeks). Statutory public holidays: 8 (England / Wales), 9 (Scotland), 10 (Northern Ireland).

**Statutory pension enrolment.** Automatic enrolment under the Pensions Act 2008 — every UK employer must enrol eligible workers in a workplace pension scheme; minimum contribution 8% of qualifying earnings (5% employee, 3% employer, as of the most recent phased-in rate). The Pensions Regulator oversees.

**IR35 / off-payroll working.** As noted in [chapter 01](./01-eor-vs-peo-vs-direct-entity-decision-framework.md), engagement of UK contractors through personal-service companies (PSCs) requires an IR35 status determination and, for medium-and-large clients, PAYE / NIC withholding if the engagement is deemed inside IR35. HMRC's CEST tool and status-determination-statement mechanics govern.

**TUPE.** The **Transfer of Undertakings (Protection of Employment) Regulations 2006 (TUPE)** — the UK implementation of the EU Acquired Rights Directive — protects employees on the transfer of a business or a service-provision change. Terms and conditions transfer with the employee; changes and dismissals connected to the transfer are void unless justified by an ETO (economic, technical, or organisational) reason.

**Working time and NMW.** Working Time Regulations 1998 cap the average working week at 48 hours (opt-out permitted individually and commonly signed for professional roles); National Minimum Wage / National Living Wage sets floor wages by age band.

## Germany

**Governing law:** Bürgerliches Gesetzbuch (BGB), Book 2 §§ 611–630 (employment contracts); Kündigungsschutzgesetz (KSchG); Betriebsverfassungsgesetz (BetrVG) — works-council regime; Teilzeit- und Befristungsgesetz (TzBfG); Bundesurlaubsgesetz (BUrlG); Allgemeines Gleichbehandlungsgesetz (AGG); Nachweisgesetz; Arbeitnehmerüberlassungsgesetz (AÜG); many sector-specific and collective-bargaining overlays.

**Default contract type.** Indefinite-term (unbefristeter Arbeitsvertrag). Fixed-term contracts (befristeter Arbeitsvertrag) permitted only under enumerated grounds or, for a first-time engagement, without objective grounds for up to 2 years (with limited renewals) under TzBfG § 14.

**Statutory notice on termination.** BGB § 622:
- **4 weeks** to the fifteenth of a calendar month or the end of a calendar month (baseline).
- **Employer-side extended notice by tenure**: 1 month after 2 years; 2 months after 5 years; 3 months after 8 years; 4 months after 10 years; 5 months after 12 years; 6 months after 15 years; **7 months after 20 years**, all to the end of a calendar month.
- Contracts frequently extend the mutual notice period by agreement.

**Termination protection.** **KSchG applies** after **6 months' service** in workplaces with **more than 10 employees** (excluding trainees). Once KSchG applies, dismissal requires one of three enumerated grounds:
- **Personal grounds (personenbedingt)** — inability to perform the role (long-term illness, loss of professional licence).
- **Conduct grounds (verhaltensbedingt)** — breach of duties, generally requiring prior warning (Abmahnung).
- **Operational grounds (betriebsbedingt)** — reduction in operations requiring a workforce reduction, subject to statutory **social selection (Sozialauswahl)** among comparable employees (weighting age, service, dependants, disability).

Special protection applies to specific categories — works-council members, pregnant employees (Mutterschutzgesetz), parents on parental leave, severely disabled employees (SGB IX).

**Works-council co-determination.** The **Betriebsrat (works council)** — elected by the workforce in businesses with **5+ permanent employees** — has co-determination rights over working time, hiring, transfers, dismissals, social matters, workplace changes, and staffing plans (BetrVG §§ 87, 99, 111). The employer must **consult the Betriebsrat before every dismissal** (BetrVG § 102); a dismissal without works-council consultation is void. For workforce reductions above defined thresholds, an **operational-change (Betriebsänderung)** consultation triggers additional obligations, including negotiation of an **interest-balancing agreement (Interessenausgleich)** and a **social plan (Sozialplan)** covering severance and workforce-transition measures (BetrVG §§ 111–113).

**Statutory paid leave.** BUrlG minimum: **20 working days** (based on a 5-day week) or **24 working days** (based on a 6-day week) per year. Common German market practice provides **25–30 days**. Public holidays: state-dependent, typically 9–13 additional days.

**Statutory continued-pay-during-sickness.** **6 weeks** of continued pay by the employer during illness (Entgeltfortzahlungsgesetz § 3); thereafter, statutory sickness pay (Krankengeld) from the statutory health-insurance system for up to 78 weeks.

**Social insurance.** Statutory health insurance (roughly 14.6% + supplemental rate, split 50/50 employee/employer); statutory pension insurance (18.6%, split 50/50 up to income ceiling); unemployment insurance (2.6%, split 50/50); long-term-care insurance (roughly 3.4%, employer share slightly lower). Employer administers all withholdings and remittances through payroll.

**Employee-invention regime.** Arbeitnehmererfindungsgesetz (ArbnErfG) — see [chapter 03](./03-intercompany-and-transfer-pricing-structure.md). Employee-invention compensation is a real, ongoing statutory obligation.

**Data protection.** BDSG-neu (Bundesdatenschutzgesetz — new) implements GDPR in the employment context; § 26 BDSG addresses employee-data processing. See [chapter 07](./07-international-privacy-and-fcpa-overlay.md).

## France

**Governing law:** Code du travail (extensive statutory framework); Code de la sécurité sociale; sector-wide collective bargaining agreements (conventions collectives) that layer on top of the Code and are near-universal in coverage.

**Default contract type.** **CDI (contrat à durée indéterminée)** — indefinite-term — is the default. **CDD (contrat à durée déterminée)** — fixed-term — is available only in enumerated situations (temporary replacement of an absent employee, seasonal work, temporary increase in activity, project-specific work). Maximum CDD duration typically 18 months (with variance by ground); improper CDD converts by operation of law to CDI. A **10% precarity indemnity (prime de précarité)** is due at the end of most CDDs.

**Statutory notice on termination.** Code du travail L. 1234-1: statutory minimum notice varies by tenure — no minimum below 6 months (subject to convention collective); **1 month** for 6 months to 2 years; **2 months** for 2+ years. Applicable convention collective typically extends notice, particularly for senior / executive roles.

**Termination protection.** Dismissal requires **cause réelle et sérieuse (real and serious cause)** — personal (performance / conduct) or economic. Procedural requirements are extensive: pre-dismissal interview (entretien préalable) with formal notification and an opportunity for the employee to be assisted; written notification of dismissal specifying the reasons; observance of the notice period. Wrongful-dismissal awards (indemnité de licenciement sans cause réelle et sérieuse) are set within a **Barème Macron** grid keyed to tenure and workforce size (Ordonnance n° 2017-1387; article L. 1235-3 Code du travail).

**Severance.** Statutory **indemnité légale de licenciement** for employees with 8+ months' service: **1/4 month's salary per year of service** for the first 10 years; **1/3 month's salary per year** for years thereafter (article R. 1234-2). Convention collective typically enhances.

**Economic redundancy (licenciement pour motif économique).** Additional procedural formality — priority reclassification obligation (obligation de reclassement), consultation with the CSE, priority re-hiring rights (priorité de réembauche).

**PSE — plan de sauvegarde de l'emploi.** For employers with **50+ employees** proposing to dismiss **10+ employees for economic reasons within a 30-day period**, the employer must adopt a **PSE** — a comprehensive social plan covering redeployment measures, training, external placement support, severance, and consultation with the CSE. The PSE is validated or homologated by the DREETS (regional labour administration) before dismissals can be effected. This is one of the most procedurally demanding termination regimes in the OECD; expect **3–6 months minimum** from PSE launch to effected dismissals.

**CSE (comité social et économique).** Employers with **11+ employees** must have a **CSE** — elected employee representation — with attributions varying by workforce size (economic and social attributions expand at 50+ employees under Ordonnance n° 2017-1386). CSE consultation is required on significant organisational changes; dismissal of employee representatives requires labour-inspectorate authorisation.

**Statutory paid leave.** **5 weeks (30 working days on a 6-day week / 25 on a 5-day week)** paid annual leave (Code du travail L. 3141-3). Public holidays: 11 statutory (variable observance).

**35-hour week.** The statutory working week is **35 hours (durée légale du travail)** — hours above 35 are overtime unless a **forfait jours** (day-count) arrangement applies for eligible cadre / executive employees.

**Ruptures conventionnelles.** A negotiated mutual-termination mechanism (article L. 1237-11 et seq.) enabling employer and employee to end a CDI by mutual agreement with a specific negotiated severance, subject to a reflection period and administrative homologation. Widely used in practice as an alternative to dismissal.

## Canada

**Governing law:** Provincial employment-standards statutes (Ontario Employment Standards Act, 2000; Quebec Loi sur les normes du travail; British Columbia Employment Standards Act; Alberta Employment Standards Code; and equivalents in other provinces); provincial human-rights codes; Canada Labour Code for federally-regulated sectors (banking, telecom, interprovincial transport, some others); provincial pay-equity, occupational-health-and-safety, and workers-compensation regimes.

**Federal vs. provincial jurisdiction.** Provincial law governs most private-sector employment. The Canada Labour Code governs federally-regulated employers (10% of the workforce). Confirm jurisdiction before applying rules.

**Default contract type.** Written employment contract common; verbal contracts enforceable but not recommended. Fixed-term contracts permitted; conversion or common-law renewal-of-employment analysis applies on repeated renewal.

**Statutory notice on termination.** Provincial statutory minimums per employment-standards statute. Ontario ESA § 57: 1 week for 3 months–1 year; 2 weeks for 1–3 years; 3 weeks for 3–4 years; and increasing to 8 weeks after 8 years, plus **severance pay** for employers with a $2.5M+ Ontario payroll (or 50+ terminations within 6 months) at 1 week per year of service up to 26 weeks (ESA § 64). Other provinces have similar tables.

**Common-law reasonable notice.** In the absence of a specifically enforceable termination clause in the employment contract, **common-law reasonable notice** applies **on top of the statutory minimum**. The *Bardal v. Globe & Mail* factors — character of employment, length of service, age, availability of similar employment — drive the calculation; awards routinely range from **1 to 24 months** of notice or pay in lieu. Enforceable contractual termination clauses can limit termination pay to the statutory minimum; unenforceable clauses (frequently invalidated for failure to satisfy the entire ESA at all times of tenure, per *Waksdale v. Swegon North America Inc.*, 2020 ONCA 391) revive common-law entitlement.

**Termination-clause drafting is a specific expertise.** A defensible Ontario termination clause requires meticulous drafting; boilerplate clauses are routinely struck down. Retain Canadian employment counsel for the local employment-contract template.

**Constructive dismissal.** A unilateral, fundamental change to the terms of employment (compensation cut, demotion, forced relocation) can constitute constructive dismissal — treated as termination with the associated notice / severance liability.

**Statutory paid leave.** Provincial. Ontario ESA: **2 weeks** after 1 year, **3 weeks** after 5 years of service. Quebec: 3 weeks after 3 years. Federal: 2 weeks initial, 3 weeks after 5 years. Public holidays: 9 (federal) / 9–12 (provincial).

**Quebec-specific.** Language-of-work regime under the Charter of the French Language (Loi 96 as amended by the *Act respecting French, the official and common language of Québec*, in force from 2022 with staged effective dates) — French must be the language of internal communication; French-language proficiency requirements imposed on hires above certain thresholds; French versions of employment contracts and workplace policies required.

**Workers' compensation.** Provincial no-fault workers-comp regime; mandatory registration and premium payment.

## Australia

**Governing law:** Fair Work Act 2009 (federal); modern awards; enterprise agreements; National Employment Standards (NES); state-level long-service-leave, workers-compensation, and occupational-health-and-safety overlays.

**Default contract type.** Written employment contract. Fixed-term contracts subject to the December 2023 Fair Work amendments limiting fixed-term contracts to a maximum of 2 years (with limited exceptions) and prohibiting consecutive fixed-term contracts. Casual employment framework separately regulated with a defined pathway to permanent conversion.

**Statutory notice on termination.** Fair Work Act s. 117: employer minimum notice **1 week** for up to 1 year of service; **2 weeks** for 1–3 years; **3 weeks** for 3–5 years; **4 weeks** for 5+ years; **plus 1 additional week if the employee is 45+ and has 2+ years of service**. Modern award or enterprise agreement may extend.

**Unfair dismissal.** Fair Work Act Part 3-2. Available after a minimum employment period of **6 months** (12 months for small business), subject to eligibility. Remedies: reinstatement, compensation (capped at 6 months' pay). Dismissal must not be "harsh, unjust or unreasonable" — evaluated against the Small Business Fair Dismissal Code (for small businesses) or the general test (for other employers).

**General protections.** Fair Work Act Part 3-1 protects employees from adverse action taken for a workplace right, industrial activity, discrimination on protected attributes, or a range of other prohibited reasons. Reverse onus of proof on the employer once the employee raises a prima facie claim. Awards uncapped.

**Redundancy.** Genuine-redundancy defence to unfair dismissal (Fair Work Act s. 389). Statutory **redundancy pay** (s. 119): scales from 4 weeks (1–2 years' service) to a maximum of 16 weeks (9–10 years' service) and then reduces slightly at longer tenures. Small-business employer (fewer than 15 employees) is exempt from statutory redundancy pay.

**Modern awards / enterprise agreements.** Most Australian employees are covered by a modern award or enterprise agreement that sets minimum wages, working hours, allowances, penalty rates, and other conditions specific to the industry / occupation. Award coverage is a specific analysis for each role.

**Statutory paid leave.** NES: **4 weeks (20 days)** paid annual leave per year (5 weeks for shift workers). **10 days** personal / carer's leave. **12 months** unpaid parental leave (with statutory paid-parental-leave scheme in parallel). Long-service-leave: state-level entitlement (typically after 7–10 years of service with the same employer).

**Superannuation.** Superannuation Guarantee — currently **11.5%** of ordinary time earnings paid by the employer to a complying superannuation fund on behalf of the employee (rising to 12% on July 1, 2025, per Superannuation Guarantee (Administration) Act 1992). Employer must offer a choice-of-fund at hire.

## Cross-cutting patterns

Beyond the country-by-country specifics, several patterns recur across most non-US jurisdictions and worth internalising:

- **Notice periods are floors, not ceilings.** Contractual notice periods commonly extend statutory minimums, especially for senior roles. Executive contracts routinely include **6–12 months** of contractual notice; the "garden leave" mechanism (paid non-working notice) is a routine drafting element.
- **Severance is real.** Statutory severance obligations attach in most non-US jurisdictions on redundancy / non-cause termination. The exec-team compensation package must be designed with the severance regime of each executive's country of employment in mind.
- **Consultation obligations bite.** Collective consultation (UK 20+/30-day and 100+/45-day), German Betriebsrat, French CSE and PSE — the consultation windows push planned workforce actions out by weeks or months. Announcements cannot precede consultation.
- **Employee-representative bodies have real veto or delay power.** German works councils, French CSE, Nordic country tillitsvalgt / union representatives, Netherlands works councils — the operator must engage the representative body, not around it.
- **Local counsel is non-negotiable.** No US employment attorney can competently draft a French employment contract or advise on a German dismissal. Retain local counsel for each country of operation.

## Practical implications

**Exec-team severance design.** Executive compensation packages designed for US at-will terminations do not survive scrutiny in most other jurisdictions. Where an executive is employed by an international subsidiary:

- The local employment contract must comply with local law (notice, severance, cause requirements).
- Change-of-control acceleration provisions in equity grants remain governed by the equity plan (US plan) but interact with the local severance obligations.
- Retention agreements, cash-severance letters, and separation agreements must be drafted for local enforceability — including specific language required in some jurisdictions (release-of-claims mechanics vary; some jurisdictions require signed post-termination release; some require negotiated mutual-termination like the French *rupture conventionnelle*).

**Global workforce reductions.** [Chapter 08](./08-international-workforce-reduction-playbook.md) operationalises the country-specific reductions playbook — the consultation windows, the immigration implications, the EOR unwind, and the interaction with the US-side layoff playbook in [mod-107](../mod-107-performance-promotion-and-offboarding/).

**Handbook and policy design.** Global-policy design frequently defaults to a "highest-common-denominator" approach — the group adopts the strictest applicable rule (e.g., 30-day statutory notice) across markets. This simplifies the policy stack but overpays in the more-flexible markets. The alternative — per-market policy addenda — respects local law and market practice at the cost of policy-stack complexity. Neither is inherently correct; the choice is a deliberate operating-model decision.

**M&A implications.** Acquiring a company with international workforce inherits the country-specific employment-law regimes; TUPE-like acquired-rights transfers apply in the EU / UK; consultation obligations attach to the transaction. Diligence and integration planning must include local employment-counsel input in every country of operation.

## Concrete example — first-country employment-law posture

A representative posture for a Series-B US AI-infrastructure startup opening a UK subsidiary and considering Germany, France, and Canada:

- **UK.** Employment contract template drafted by UK counsel; indefinite-term; 1-month mutual notice at entry, extending to 3 months for senior individual contributors and 6 months for VP-level and above; 28 days paid annual leave inclusive of statutory bank holidays; workplace pension via auto-enrolment. Termination-planning assumes 2-year unfair-dismissal vesting; consultation obligations tracked from first UK hire onwards.
- **Germany.** Direct subsidiary contemplated once headcount passes 5 (works-council trigger). Employment contract template drafted by German counsel using KSchG-compliant boilerplate; 25 days paid annual leave (market standard); mutual notice per BGB § 622 tenure schedule. Terminations require KSchG cause + Betriebsrat consultation from the day the works council exists.
- **France.** CDI-only for direct hires; EOR arrangement used for the first 1–2 hires before entity is stood up; French counsel drafts local CDI template with convention collective referenced; termination planning assumes formal *entretien préalable* + written cause + convention-collective severance schedule. Any group reduction ≥ 10 employees within 30 days triggers PSE — a decision requiring 3–6 months' runway.
- **Canada (Ontario).** ESA-compliant employment contract drafted by Ontario counsel with a termination clause satisfying the ESA at all times of tenure (per *Waksdale*). Common-law reasonable notice contained by an enforceable termination clause where possible; SR&ED programme requires Canadian corporate taxpayer status ([chapter 02](./02-first-international-entity-setup.md)).

## Summary

- **US at-will is a global exception.** Every non-US jurisdiction of interest to a US startup operates on some version of cause-required-or-severance-required-or-both.
- **Statutory notice periods** — UK 1–12 weeks (tenure-based); Germany BGB § 622 tenure schedule up to 7 months; France 1–2 months (convention collective extends); Canada provincial statutory minimums + common-law reasonable notice; Australia 1–4 weeks + tenure add-on.
- **Termination-protection regimes** — UK unfair dismissal (2-year vesting); Germany KSchG (6-month vesting, 10+ employees); France cause réelle et sérieuse + Barème Macron; Canada common-law reasonable notice; Australia Fair Work unfair dismissal + general protections.
- **Works-council / representative obligations** — Germany Betriebsrat (5+ employees); France CSE (11+ employees) + PSE (50+ employees, 10+ economic dismissals in 30 days); UK collective consultation (20+ / 30 days, 100+ / 45 days).
- **Statutory paid-leave floors** — UK 28 days; Germany 20/24 days (BUrlG) with 25–30 market standard; France 5 weeks; Canada provincial 2–3 weeks; Australia 4 weeks NES; US 0 days statutory.
- **Local counsel is non-negotiable.** No US employment attorney can competently draft or advise on non-US employment matters.
- **Exec-team severance and global reductions** must be designed with country-specific severance, consultation, and procedural regimes in mind — [chapter 08](./08-international-workforce-reduction-playbook.md) operationalises the pattern.
