# 7. The HRIS / PEO / payroll stack and the graduation path

> The PEO makes seed-stage payroll and benefits work with almost no operating investment. It also becomes the constraint at Series-B — and the migration off it is a full-quarter project.

## Motivation

Every W-2 employee (see [mod-103 chapter 01](../mod-103-employment-law-and-contract-design/01-w2-vs-1099-worker-classification.md)) creates a set of operating obligations the corporation cannot skip:

- **Payroll processing** — running the payroll cycle, calculating gross-to-net, remitting payroll taxes to the IRS and every state where the corporation employs someone, generating pay stubs, delivering direct deposits, and preparing year-end W-2s.
- **Payroll-tax registration** — the corporation must register as an employer with the state tax authority and, in most states, with the state unemployment-insurance and workers'-compensation systems, in every state where it has an employee. Registration is per-state, per-tax, and takes weeks.
- **Workers' compensation** — every state requires the corporation to carry workers'-comp coverage for its employees (with a narrow set of exceptions). The insurance is placed through a broker; the premiums vary by state, class code (job type), and payroll volume.
- **Benefits administration** — health, dental, vision, 401(k), FSA / HSA, commuter, life / disability, and ESPP where applicable. Benefits require a broker (for health / dental / vision / life / disability), a plan administrator (for 401(k)), and open-enrollment, life-event, COBRA, and ACA-reporting operational cadences.
- **HR system-of-record** — every employee has a record: name, address, tax withholding, direct-deposit info, comp history, title / department / manager, PTO balance, benefits selections, work-authorisation status, performance history.
- **Compliance overlay** — I-9 / E-Verify, ACA Form 1095-C reporting (for Applicable Large Employers), state pay-transparency logging, EEO-1 reporting (for employers of 100+), OFCCP (for federal contractors), plus the state-specific labour-law posters, wage-theft-prevention notices, and paid-sick-leave accruals.

At two W-2 employees, all of that is a founder-time drag. At twenty employees across four states, it is a full-time function. At two hundred employees across ten states and two countries, it is a full department with a system of record, a benefits broker, a payroll operations lead, and a compliance calendar.

The corporation gets from two to two hundred through a stack that graduates in a predictable sequence: **PEO** at seed (bundled) → **HRIS** at Series-A / B (unbundled, self-administered) → **HCM** at growth (integrated enterprise suite). Each transition is deliberate; each has a trigger; each has cost, control, and benefits-access trade-offs that this chapter names.

## The bundled-vs-unbundled axis

The single most useful mental model for this chapter is **bundled vs. unbundled**:

- **Bundled (the PEO model).** The Professional Employer Organization is the "co-employer" of the corporation's employees for a defined set of purposes — payroll, employment taxes, workers'-comp, benefits — under a Client Service Agreement (CSA). The PEO uses its own EIN for payroll tax filings, sponsors master benefits plans that the corporation's employees participate in, carries workers'-comp coverage under a PEO-master policy, and provides an integrated HR platform.
  - **Pro.** Access to large-group benefits pricing the corporation could not get on its own at 20 employees. Compliance overhead handled by the PEO. Time-to-set-up measured in days, not weeks. Single vendor to work with.
  - **Con.** Cost is a % of payroll (typically <!-- needs-research: confirm typical PEO administrative-fee ranges; commonly quoted PEO admin fees are 2–12% of payroll or $50–$200 per employee per month, but the range is wide and depends on services included, benefits pass-through, geography, and employer size. -->). Corporate identity submerged in PEO's tax filings (the corporation is not the direct employer of record with SSA for many purposes). Benefits switching cost is high — leaving the PEO means a full benefits re-open. Migration off the PEO is a project.

- **Unbundled (the HRIS + broker + payroll model).** The corporation is the employer of record. Payroll is processed through an HRIS with a payroll engine (Rippling, Gusto, Deel, or a payroll-native product like ADP Run or Paychex Flex). Benefits are placed through a benefits broker (Newfront, Woodruff Sawyer, Aon, One Digital, Mercer, or a startup-focused broker like Newfront's One Medical partnership offerings, Sequoia Consulting Group's post-Justworks-graduation service, or Rippling's own benefits brokerage). Workers'-comp is placed through a broker. Compliance is the corporation's own.
  - **Pro.** Direct control over benefits design and broker selection. Full corporate-identity presence with SSA and every state tax authority. Costs scale less steeply than PEO percentage. Path to full HCM is cleaner.
  - **Con.** Corporation is directly responsible for compliance — payroll-tax registration in every state, workers'-comp placement, benefits open enrollment and administration, ACA reporting, COBRA administration, etc. Requires the operating capacity (a payroll operations lead at 50+ headcount, a benefits and compliance function at 100+).

The graduation from bundled to unbundled is the largest single operating transition covered in this chapter.

## Stage 1 — PEO at seed (headcount ~1–50)

### The PEO landscape

The PEO landscape in the US venture-backed ecosystem is dominated by a small set of providers:

- **Justworks** — startup-focused PEO with a modern platform and predictable per-employee-per-month pricing. Frequent seed-stage default. Also offers a non-PEO (payroll-only) product for corporations that graduate off the PEO but want to stay on the same platform.
- **TriNet** — larger PEO with an established benefits book and specific vertical offerings (technology, life sciences). Common at seed and Series-A.
- **Sequoia One** — the PEO arm of Sequoia Consulting Group, popular with venture-backed technology companies and known for a strong benefits book. Sequoia Consulting Group also offers a post-PEO consulting / brokerage service ("Sequoia Enterprise Solutions" and related offerings) that some corporations use during graduation.
- **Insperity, Paychex PEO, ADP TotalSource** — larger national PEOs with a broader but less-startup-focused book.

<!-- needs-research: confirm current PEO market positioning, pricing, and benefits book for Justworks, TriNet, Sequoia One, Insperity, Paychex PEO, and ADP TotalSource; the PEO market has consolidated in specific ways since 2020 and current-state should be checked before publishing a specific recommendation. -->

Any of the above will work at seed. The specific choice usually turns on (a) benefits book fit for the corporation's employee geography and demographics, (b) platform ergonomics, and (c) the corporation's PEO / non-PEO path (some PEOs, notably Justworks, offer a non-PEO product that reduces migration friction later).

### Why the PEO is right at seed

At seed the corporation has 3–20 employees, is opening in two or three states, and does not have a head of people or a payroll operations lead. It has a founder-CEO who does not want to research state unemployment-insurance registration in Colorado, an operator who does not want to negotiate a health-insurance renewal with a broker at 8 lives, and a burn rate that would rather pay a per-employee-per-month fee than build the operating machinery in-house.

The PEO absorbs all of it. In practice a seed-stage PEO onboarding takes 2–6 weeks and produces:

- A payroll cadence (usually semi-monthly or biweekly) running from day one.
- Health, dental, vision, and often life / disability benefits accessible on day one (or within the plan's waiting period).
- 401(k) plan (in some PEO's offerings; in others, the corporation adopts its own plan through a separate provider).
- Workers'-comp coverage in every state where the corporation has an employee.
- Payroll-tax registrations handled by the PEO under its own EIN.
- An HR platform for employee self-service, PTO tracking, and document storage.

### The PEO's blind spots

The PEO's benefits are structural, not universal:

- **Benefits are the PEO's benefits.** The corporation cannot easily customise; the benefits plan-designs on offer are what the PEO's master policies offer. If the corporation wants a specific carrier network, a specific plan design, or a specific 401(k) match that the PEO does not offer, the PEO cannot accommodate.
- **HRIS features may lag standalone HRIS products.** The PEO platform is good at what it does; it is often less feature-rich than a standalone HRIS on things like modern onboarding workflows, performance management, headcount planning, or granular reporting.
- **State-registration is under the PEO's EIN.** The corporation does not build its own state-level payroll-tax registration muscle. When the corporation eventually leaves the PEO (see graduation, below), it will need to register in every state from scratch — a multi-week project per state.
- **Percentage-of-payroll fee grows with the corporation.** A 5% PEO fee on a $200k payroll is $10k/year — cheap. On a $10M payroll (100 employees at $100k avg) it is $500k/year — visible. On a $30M payroll it is $1.5M/year and materially larger than the operating cost of an in-house payroll + brokerage + compliance function.
- **Concentration risk.** All of the corporation's HR data, payroll, and benefits are with one vendor. A PEO outage or a PEO business event is disproportionately consequential.

## Stage 2 — HRIS at Series-A / B (headcount ~50–200)

### The graduation trigger

The trigger to graduate off the PEO is typically a combination of:

- **Cost.** The percentage-of-payroll fee has crossed the point where a self-administered stack is materially cheaper.
- **Benefits design.** The corporation wants benefits customisation, a specific carrier, a specific 401(k) match design, or better executive-benefits offerings that the PEO cannot deliver.
- **Operating maturity.** The corporation has hired (or is about to hire) a Head of People and can hire a Payroll Operations lead and a Benefits & Compliance lead within the next 12 months.
- **Feature gap.** The HRIS features (headcount planning, performance management, engagement surveys, onboarding workflow, reporting) the corporation now needs are ahead of the PEO's platform.
- **Diligence.** Series-B / Series-C diligence is easier when the corporation is the direct employer of record with visibility into its own compliance posture, rather than routed through a PEO's aggregate.

Typical trigger headcount is 50–100, sometimes earlier if the trigger is benefits design or later if the corporation is deliberately conservative.

### The HRIS landscape

The dominant startup-market HRIS products at Series-A / B:

- **Rippling** — modern HRIS + IT (identity / device / SaaS provisioning) + Finance (spend management) platform. Strong integrated payroll, benefits administration, onboarding, and compliance. Very strong integration story across IT and HR.
- **Gusto** — SMB-focused HRIS with strong payroll, benefits administration, contractor payments, and time tracking. Increasingly credible at Series-A / B; historically stronger at seed / SMB.
- **Deel HR** — international-first HRIS with strong contractor and EOR capabilities; growing US-employee capabilities. Common where the corporation has international operations from early on.
- **BambooHR** — HRIS with strong core HR features (employee record, onboarding, performance) — payroll varies by geography and integration.
- **Namely** — HR + payroll + benefits platform focused on mid-market. <!-- needs-research: confirm Namely's current positioning and market share. -->

<!-- needs-research: confirm current pricing tiers and feature sets for Rippling, Gusto, Deel HR, BambooHR, Namely; the HRIS market has moved substantially since 2022. -->

### The unbundled operating stack

Post-PEO, the corporation operates a stack:

- **HRIS + payroll.** Rippling, Gusto, Deel, or a specialised payroll product (ADP Run, Paychex Flex — historically strong at broader SMB, though the market has moved to modern HRIS-native payroll for tech).
- **Benefits broker.** The corporation selects a broker (see below) who places health / dental / vision / life / disability. The broker is the corporation's *ongoing* partner — renewals, plan design, employee education, open enrollment.
- **401(k) provider.** A separate 401(k) provider (Guideline, Human Interest, ForUsAll, Betterment 401(k), Fidelity, Vanguard, Empower) with plan design (safe-harbour, match structure, vesting). Integrated to the HRIS for contribution / withholding.
- **Workers' comp.** Placed through the corporation's broker (may be the same broker as health, or a separate P&C broker). State-by-state, with an audit at renewal.
- **HRIS-integrated adjacent tools.** Performance management (Lattice, 15Five, Culture Amp), LMS (Learn.com, TalentLMS, WorkRamp, Trainual), engagement surveys, and expense management (Ramp, Brex, Airbase — with HRIS integrations).

### The benefits-broker selection

The broker is the corporation's *ongoing* partner. Selection factors:

- **Book of business.** Does the broker have a book of business in the corporation's geographies and size range that gives it real market leverage?
- **Startup-native.** Does the broker understand the venture-backed startup lifecycle — mid-year headcount growth, geo expansion, executive-benefits considerations, ESPP integration?
- **Service model.** Is the corporation's day-to-day contact a licensed benefits consultant, or a service desk? How responsive are they? What is the SLA on employee-question resolution?
- **Technology integration.** Does the broker integrate with the corporation's HRIS for enrollment, terminations, and life events? Modern brokers (Newfront, Sequoia Consulting Group, One Digital, Aon, Woodruff Sawyer) all offer some form of HRIS integration; the depth varies.

Common startup-focused brokers: **Newfront**, **Sequoia Consulting Group** (the same Sequoia — a common post-Sequoia-One-PEO continuation), **Woodruff Sawyer**, **Aon**, **One Digital**, **Marsh & McLennan Agency**, and the HRIS-native brokerages (e.g., **Rippling's own brokerage arm**, **Gusto's benefits marketplace**).

<!-- needs-research: confirm current broker landscape, service tiers, and typical broker-of-record fee structures for startup-focused benefits brokerages. -->

The corporation should interview 2–3 brokers before making the selection — this is a multi-year relationship and the fit matters.

### The migration project

Moving from a PEO to an unbundled HRIS + broker stack is a 3–6 month project. Common milestones:

1. **Decision and vendor selection (month 0).** Board / CEO decision to migrate. HRIS selection. Benefits broker selection. 401(k) provider selection. Workers'-comp broker selection (may be same as benefits).
2. **State-tax registrations (months 1–3).** The corporation registers as an employer with SSA (for FUTA), the IRS (SS-4 EIN — already in place from formation, but confirm), every state's tax authority (state income tax withholding, state unemployment insurance), and every state's workers'-comp authority. Registrations take 2–8 weeks per state and are dependency-blocking for payroll cutover.
3. **Benefits plan design and quote (months 1–3).** Broker quotes health / dental / vision / life / disability with the corporation's employee census. Plan design decisions. Contribution strategy (employer contribution %, HDHP + HSA vs. PPO tiers, family-plan strategy, dependent-care FSA vs. HSA).
4. **401(k) plan setup (months 1–3).** 401(k) plan document, safe-harbour vs. non-safe-harbour, match design, vesting, eligibility, entry dates.
5. **HRIS setup and data migration (months 2–4).** Employee data migration from the PEO to the HRIS. Historical payroll data reconciliation for W-2 continuity.
6. **Open enrollment window (month 3–4).** Employees enroll in the new benefits plans. Typically a 2–3 week enrollment window with clear communication and support.
7. **Parallel run (month 4).** One or two payroll cycles run in parallel between the PEO and the HRIS to validate calculations before cutover.
8. **Cutover (month 4–5).** The PEO's last payroll runs. The HRIS's first payroll runs. Employees experience continuity of benefits and pay.
9. **PEO exit and W-2 reconciliation (months 5–6).** The PEO issues W-2s for the portion of the year under its EIN; the corporation issues W-2s for the portion under its EIN. Employees receive two W-2s for the transition year.

The migration is not casual. Failure modes:
- Missed state registration → payroll runs but tax remittance fails; the corporation gets late-payment penalties from a state tax authority.
- Failed W-2 reconciliation → employees get incorrect year-end tax documents and file amended returns.
- Broken benefits transition → employees experience a gap in coverage during transition.

A defensible migration has a dedicated project lead (typically the Head of People or a Payroll Operations lead), a written project plan with owners and deadlines, external counsel review on any employment-law questions surfaced by the transition, and weekly executive updates until cutover is confirmed successful.

## Stage 3 — Full HCM at growth (headcount ~500–1,000+)

### The graduation trigger

At scale — 500+ employees, multiple countries, an in-house benefits function, an HR business-partner org, a talent-management function — the mid-market HRIS starts to constrain. Common triggers:

- **Global payroll.** The HRIS's global-payroll story does not cover every country; the corporation is running a patchwork of country-specific providers (see [mod-113](../mod-113-international-expansion-and-global-workforce/)).
- **Enterprise controls.** SOC 2, ISO 27001, and enterprise-customer security-review requirements need controls the mid-market HRIS does not natively provide at the enterprise level.
- **Talent-management depth.** The corporation needs deep succession planning, complex performance-management workflows, learning-management integration, and enterprise headcount planning.
- **Finance integration.** Corporate finance wants the HRIS integrated with the ERP (NetSuite, SAP, Oracle) at a depth the mid-market HRIS does not support natively.

The graduation is to a full **Human Capital Management (HCM)** suite:

- **Workday HCM** — dominant enterprise HCM. Common at post-IPO / growth-stage tech.
- **Dayforce (formerly Ceridian)** — HCM with strong payroll and workforce management.
- **SAP SuccessFactors** — enterprise HCM common at larger and international corporations.
- **Oracle HCM Cloud** — enterprise HCM common at Oracle-heavy shops.
- **UKG Pro / UKG Ready** — HCM common in specific verticals.

<!-- needs-research: confirm current market positioning and pricing of the enterprise HCM suites; this is a growth-stage decision and the market has evolved. -->

### The HCM migration

Migration from a mid-market HRIS to an HCM is a multi-quarter, cross-functional project — typically ~9–18 months from selection to full go-live. It touches every people-ops process, every finance integration, every IT provisioning workflow, and every manager's UI. This is properly a growth-stage / pre-IPO decision, and this module flags the transition rather than walking it in depth — the depth belongs in a growth-stage people-ops module.

## Multi-state and multi-country payroll complexity

Every state where the corporation has an employee adds:

- **State income-tax withholding.** Correct withholding based on the employee's state of residence and, in some cases, the state where the work is performed. Reciprocity agreements between neighbouring states (e.g., PA-NJ, VA-DC-MD) reduce some complexity.
- **State unemployment insurance.** Corporation must register, pay quarterly contributions, and update as employees are hired / terminated.
- **Workers' comp.** State-specific coverage requirements and class codes.
- **State-specific paid-leave.** California PDL / CFRA, New York PFL, Washington PFML, Massachusetts PFML, Colorado FAMLI, Oregon Paid Leave, Connecticut PFMLA — and more, added regularly. Each has employer contribution / employee contribution / leave-request administration workflow.
- **State-specific pay-transparency, wage-theft-prevention notice, and pay-stub requirements.** See [mod-103 chapter 08](../mod-103-employment-law-and-contract-design/08-state-law-variance.md).
- **State-specific final-pay laws.** California (immediate on termination), several other states (within a specified period after termination). Off-cycle payroll runs required.

The HRIS is what makes this tractable. Every modern HRIS (Rippling, Gusto, Deel) supports multi-state payroll natively; every PEO absorbs it under the PEO's own registrations. The failure pattern is the corporation that hires its first out-of-state employee without registering in that state and runs a payroll cycle without correct withholding — creating an obligation the corporation must clean up retroactively with the state's tax authority.

Multi-country payroll (post-first-international-hire) is the [mod-113](../mod-113-international-expansion-and-global-workforce/) territory. The relevant handoff: an HRIS that handles international well (Deel, Rippling International, Remote, Papaya Global) is preferable to a US-only HRIS paired with country-specific providers, once international headcount is more than 5% of total.

## The SOC 2 audit boundary

The HRIS holds sensitive employee data — SSNs, comp, health-plan selections, disability status, benefits beneficiaries. The corporation's own SOC 2 audit (Type I or Type II) either includes or excludes the HRIS from its boundary — but even if excluded, the SOC 2 audit will require the corporation to have collected the HRIS's own SOC 2 report as a vendor-management artifact.

The HRIS graduation decision therefore has a SOC 2 lens:

- **PEO.** The PEO's SOC 2 report covers the PEO's operating scope. The corporation reviews the report as part of vendor management.
- **HRIS.** The HRIS's SOC 2 report covers the HRIS's operating scope; the corporation is the direct employer of record and its own controls over HRIS data (SSO, MFA, access review, data-classification handling) are in-scope for the corporation's SOC 2 audit.
- **HCM.** The HCM's SOC 2 is enterprise-grade; the corporation's own controls are still in-scope.

Depth on the SOC 2 audit boundary lives in the corporation's compliance / security programme; this module flags the intersection.

## A worked example — a Series-B PEO-to-HRIS graduation decision

The corporation is at 80 employees across 8 states, on Justworks since seed. It has just closed Series-B and is planning to grow to 200 in 18 months, add a first international hire, and build a benefits function.

**The decision.**

Migrate off the PEO to Rippling (HRIS + payroll + benefits admin + IT provisioning), Newfront (benefits broker), and Guideline (401(k) provider). Retain Justworks as the incumbent through cutover; use Justworks's post-PEO payroll product only if the migration slips.

**Rationale.**

- **Cost.** Justworks PEO fee at 80 employees on the corporation's total payroll is materially higher than the projected Rippling + Newfront + Guideline stack once the internal payroll ops lead is in place.
- **Benefits design.** The corporation wants a specific health-carrier network (competitive with the PEO's book but not identical) and an executive-benefits enhancement the PEO does not offer.
- **International.** Rippling's international EOR product provides a cleaner path to the first international hire than Justworks's international offering.
- **HRIS features.** Rippling's integrated IT provisioning (Okta-adjacent identity, MDM integration, SCIM into every SaaS system) replaces two separate tools the corporation currently pays for.
- **Diligence.** Series-C diligence will be easier as the direct employer of record with in-house payroll and benefits records.

**Project plan.**

- Month 0 — Board / CEO decision. Vendor selection. Payroll Ops lead hired (parallel).
- Months 1–3 — State-tax registrations (8 states in parallel). Broker plan design and quotes. 401(k) plan setup.
- Months 2–4 — Rippling data migration from Justworks. Open enrollment window (mid-month 3).
- Month 4 — Parallel payroll run (last Justworks cycle + first Rippling cycle overlap).
- Month 5 — Cutover.
- Months 5–6 — Justworks exit and W-2 reconciliation for the transition year.

**Cost budget.** Migration project cost (internal + external counsel + implementation partners) ~<!-- needs-research: confirm typical PEO-to-HRIS migration cost bands; a defensible range at 80 employees is $50k–$150k in project cost plus internal time. --> plus internal time equivalent to ~0.5 FTE for 6 months.

## Summary

- The HRIS / PEO / payroll stack graduates: PEO at seed → HRIS at Series-A / B → HCM at growth.
- Bundled (PEO) trades cost and control for speed and benefits access. Unbundled (HRIS + broker + payroll) trades operating investment for cost, control, and diligence-readiness. The trade flips somewhere between 50 and 100 employees.
- Seed-stage PEO defaults: Justworks, TriNet, Sequoia One. Series-A / B HRIS defaults: Rippling, Gusto, Deel HR. Growth-stage HCM: Workday, Dayforce, SuccessFactors, Oracle HCM.
- The PEO-to-HRIS migration is a 3–6 month project — state registrations, benefits plan design, 401(k) setup, HRIS data migration, open enrollment, parallel payroll, cutover, W-2 reconciliation. Not casual.
- Multi-state payroll is per-state complexity that the HRIS abstracts but does not remove — registration, withholding, unemployment insurance, workers' comp, state-specific paid leave, state-specific notice requirements, state-specific final-pay laws.
- The benefits broker is a multi-year partner — interview 2–3, select on book, service model, and technology integration.
- The SOC 2 audit boundary intersects the HRIS choice; the corporation's controls over HRIS data are in-scope for its own SOC 2 audit at HRIS stage.
- International expansion of the workforce is [mod-113](../mod-113-international-expansion-and-global-workforce/) territory but is a factor in the HRIS-selection decision at Series-B / growth.
