# Exercise 04 — IP protection strategy decision drill

> Estimated time: **~10 hours** · Related chapter: [04 — IP protection strategy: patents, trademarks, copyrights, and trade secrets](../04-ip-protection-strategy.md)

## Problem statement

Halyard Flow is a Series-A Delaware C-corp selling an AI-assisted supply-chain optimisation product into mid-market manufacturers (roughly 55 FTE, nine months past a $7.5M Series A). The lead growth-stage investor on the Series A has flagged "IP hygiene" as a diligence lever on the next round, and the general counsel (eleven weeks in-seat) has twelve weeks to walk into the next board meeting with a defensible IP programme that will survive Series-B diligence.

Four forcing functions sit on the GC's desk simultaneously.

First, the CTO has routed three **invention disclosures** into the engineering shared folder over the last four months, each from a different engineer, with no triage process in place:

- (i) A novel reinforcement-learning scheduling algorithm that is the product's primary technical differentiator. The CTO believes a sophisticated competitor could reverse-engineer the behaviour from latency signatures observable at the public API — i.e., detectability-of-infringement is non-trivially above zero. No public disclosure to date.
- (ii) A UI/UX workflow for a scenario-comparison modal that product-and-design believe is unique to the product. The modal has been shown to roughly a dozen design-partner customers under NDA; the public marketing site shows a screenshot. The product team's view is that a competitor could visually copy the pattern within a quarter.
- (iii) A proprietary prompt-engineering template plus a training-data curation methodology that produce a measurable quality edge on a specific industry benchmark. The template and curation steps are embedded in server-side code that is never shipped to customers; the quality edge is visible in benchmark publications the corporation has itself posted on its engineering blog.

Second, the head of brand has been pushing for weeks to lock down the corporation's company mark and the hero product mark on the USPTO Principal Register, has filed nothing to date, and is planning a product launch into **Canada, the UK, and Australia** inside the next twelve months. The company mark is suggestive-bordering-on-descriptive; the hero product mark is fanciful. No formal clearance search has been run on either.

Third, the CTO has observed that of the 48 engineers hired to date, only **34 have an executed PIIA** on file. The 14-engineer gap is concentrated in the 2021 contractor cohort — engineers brought in through an outsourced staffing arrangement who were later converted to FTE without a re-papering step. Several of these engineers authored material contributions to the current production codebase, including portions of the scheduling-algorithm module in disclosure (i).

Fourth, the lead growth-stage investor's partner has asked, informally, what the IP schedule will look like at Series-B diligence. The GC has interpreted this as a request to produce the schedule now, in advance of the formal request, so that the Series-B diligence workstream opens with the IP package already clean rather than with a defect list.

Author the twelve-week IP programme. The three invention disclosures must each receive a specific disposition decision (patent / trade-secret / defensive publication) with the rationale explicit on the statutory frame; the trademark portfolio must be sequenced across the twelve-month international launch window; the PIIA gap must be remediated to a diligence-ready state; the trade-secret programme must be stood up to the DTSA "reasonable measures" bar; and the IP schedule that goes to Series-B diligence must be authored in draft form.

## Requirements

### Part A — Invention-disclosure programme

Author the standing programme the CTO and GC will run from week one onward, so that the three current disclosures and every future disclosure flow through a defined process rather than accumulating in a shared folder.

1. **Intake template.** The fields the submission form captures: title; named inventors (with contribution shares); conception date; reduction-to-practice date (if applicable); first disclosure outside the corporation (date, audience, confidentiality basis); enabled written description (the § 112 question); prior art known to inventors; whether the invention has been publicly used, sold, offered for sale, or demonstrated to a non-NDA audience (the § 102(b)(1) question); the inventors' recommended disposition. Author the template as operative fields, not a summary.
2. **Triage rhythm.** The named roles that review disclosures (CTO, outside IP counsel, head of product), the cadence (weekly? monthly?), the SLA from submission to disposition decision, and the escalation path when the triage committee is split.
3. **Retention and confidentiality discipline.** Where disclosure records are stored, the access-control posture, the retention duration, and the marking standard that flows from Part E's trade-secret programme.
4. **Stage-appropriate posture.** The chapter 04 discipline — Series-A corporations do not file every disclosure. Name the explicit filter criteria the triage committee applies before any filing-fee is spent.

### Part B — Patent / trade-secret / defensive-publication decision per disclosure

Walk each of the three current disclosures through the chapter 04 statutory frame and arrive at a specific disposition. For each disclosure, author:

1. **Subject-matter eligibility (35 U.S.C. § 101).** Where the claim would land under the *Alice* / *Mayo* / *Bilski* framework. For software-implemented inventions, is there a specific technical improvement in the *Enfish* / *McRO* sense, or does the claim read as an abstract idea on generic hardware?
2. **Novelty and the on-sale / public-disclosure bars (35 U.S.C. § 102(b)(1)).** Any prior disclosure, demonstration, offer-for-sale, or public use that triggers the twelve-month clock. For disclosure (ii), the design-partner NDA posture and the marketing-site screenshot; for disclosure (iii), the engineering-blog benchmark publication. Name the clock-start date (if any) and the filing deadline that follows.
3. **Non-obviousness (35 U.S.C. § 103) and enablement (35 U.S.C. § 112).** The practitioner view on obviousness exposure under *KSR* and the enablement adequacy of the current invention disclosure.
4. **First-inventor-to-file posture.** The AIA priority discipline — whether the corporation should file ahead of further public disclosure.
5. **Detectability-of-infringement test.** Whether infringement would be detectable from the product's public surface, from reverse-engineering a shipped artefact, or only through an inside witness. Chapter 04's canon — if the invention is not detectable, trade-secret is often the better choice.
6. **Cost curve.** The practitioner-canon cost envelope for provisional vs. non-provisional vs. provisional-then-utility, deferring specific fee figures to `<!-- needs-research: ... -->`.
7. **Disposition.** A specific recommendation per disclosure — file provisional, file utility, provisional-then-utility within twelve months, trade-secret only, defensive publication (arXiv / IP.com / Research Disclosure / company blog with timestamp) — with the rationale tied explicitly to the frame above. Do not duck; "it depends" is not a disposition.

The exercise does not pre-decide which disclosure is a patent and which is a trade secret. The author must reach a defensible per-disclosure answer and be able to defend it against the frame.

### Part C — Trademark portfolio design

Author the twelve-month trademark portfolio across the US launch and the Canada / UK / Australia expansion.

1. **US filings.** The company mark and the hero product mark on the USPTO Principal Register. The § 1051(a) use-in-commerce vs. § 1051(b) intent-to-use basis for each. The Nice classes (Class 9, Class 42, and any others the chapter 04 discussion names) and the discipline against over-filing. TEAS Plus vs. TEAS Standard per filing.
2. **Clearance posture.** The knockout search (USPTO TESS, state registers, common-law web, domain registrations) that runs first, and the full clearance search (Corsearch / Compumark / Thomson CompuMark with counsel opinion) that gates intent-to-use filing and public launch. Flag the company-mark descriptiveness exposure under § 1052(e).
3. **International posture.** The Madrid Protocol vs. direct-filing decision for Canada (CIPO), the UK (UKIPO), and Australia (IP Australia). Name the central-attack trade-off against the aggregate-filing-cost delta. Specify which route the corporation adopts and why.
4. **Twelve-month filing calendar.** A month-indexed sequence covering clearance → US intent-to-use filings → international filing route → statement-of-use / use-in-commerce evidence → launch. Align the international filings to the twelve-month convention-priority window from the earliest US filing date.
5. **Budget envelope.** The programme's twelve-month budget as a line-item sketch (US filing fees, clearance search cost, international filing fees, counsel time, watch-service subscription). Defer specific fee schedules to `<!-- needs-research: ... -->`; do not invent figures.
6. **Domain and social-handle acquisition.** The parallel workstream chapter 04 names — .com, .io, .ai, .co, country-code TLDs, and primary social-handle acquisition before public launch.

### Part D — Copyright registration posture

Chapter 04 treats copyright as the least-intentional of the four regimes but names the registration posture that preserves pre-infringement statutory damages and attorney fees. Author the registration slate.

1. **Scope.** Which works go through registration — product documentation, the published API specification, flagship whitepapers, marketing collateral, published open-source projects, source code (and the first-25 / last-25 pages redaction posture if adopted). Which works deliberately stay unregistered.
2. **Statutory frame.** The § 408 permissive registration posture, the § 411(a) prerequisite-to-suit mechanics clarified by *Fourth Estate*, and the § 412 statutory-damages-and-attorney-fees discipline — register before infringement, and within three months of publication for published works, to preserve enhanced remedies.
3. **Work-made-for-hire discipline.** The employee-authorship posture under § 201(b) and the belt-and-suspenders assignment posture for contractors who do not fit the nine-category test. Defer the full PIIA architecture to [mod-103](../../mod-103-employment-law-and-contract-design/) and the contractor-SOW drafting to [chapter 03](../03-vendor-contract-suite-and-onboarding-workflow.md); name the cross-reference, do not re-author.
4. **DMCA § 512 safe-harbour posture.** If any part of the Service hosts user-uploaded content, the safe-harbour prerequisites — designated agent registration with the Copyright Office, published takedown procedure, repeat-infringer policy — that the GC will stand up alongside the registration slate. Name whether Halyard Flow's Service in fact hosts user content and whether safe-harbour applies.

### Part E — DTSA / UTSA-compliant trade-secret programme

The "reasonable measures" element under 18 U.S.C. § 1839(3) is the operational bar. Author the programme that will satisfy it.

1. **Identification register.** The written data-classification policy — Public / Internal / Confidential / Trade Secret-Restricted — and the specific items that land in Trade Secret-Restricted (source code, unpublished algorithms, the Part B disclosures that disposition as trade-secret, customer-specific pricing, unfiled training-data curation methodology, M&A pipeline). The register itself as a maintained artefact.
2. **Access control.** Least-privilege, role-based access, MFA for Confidential-and-above, quarterly access reviews, hardware-key second-factor posture for production-code and model-repository access.
3. **Marking standard.** The footer / watermark / header-comment / data-catalogue-label convention and the discipline that marks are applied consistently so that mishandling is detectable.
4. **Personnel controls.** The PIIA with the 18 U.S.C. § 1833(b)(3) whistleblower-notice carried per [mod-103](../../mod-103-employment-law-and-contract-design/); the NDA / SOW with equivalent obligations and notice carried per [chapter 03](../03-vendor-contract-suite-and-onboarding-workflow.md). Name the cross-reference; do not re-author the PIIA architecture or the state-law variance (defer to [mod-102](../../mod-102-founding-team-legal-architecture/) and [mod-103](../../mod-103-employment-law-and-contract-design/)).
5. **Exit interview and IP-return protocol.** The checklist run at departure — continuing-confidentiality reminder, device-and-materials return, retained-information certification, outstanding invention / work-product questions. The evidentiary posture this creates in later DTSA / UTSA enforcement.
6. **Audit trail.** Logging of access to trade-secret repositories, retention duration, and the records-retention policy cross-reference to [mod-101](../../mod-101-legal-entity-formation-and-corporate-structure/).

### Part F — Chain-of-title remediation (the 14-engineer PIIA gap)

Author the remediation plan for the 14 engineers currently without an executed PIIA, with specific attention to the 2021 contractor cohort whose contributions land in the production codebase (including portions of the Part B(i) scheduling-algorithm module).

1. **Population inventory.** The named-headcount-level breakdown: how many are current FTEs, how many are former (now departed), how many authored contributions to code that is live in production, how many authored contributions to code that disposition-to-patent under Part B.
2. **Nunc pro tunc assignment posture.** The retroactive-assignment-plus-present-assignment drafting pattern the GC will use for current FTEs. The cross-reference to [mod-103](../../mod-103-employment-law-and-contract-design/) for the PIIA mechanics; the chapter 04 ownership is the chain-of-title artefact.
3. **Incremental-consideration mechanic.** The consideration that supports the retroactive assignment — nominal cash payment, a one-off RSU grant tied to the signature, or the continued-employment-and-access framing — with the practitioner-canon discipline that *some* fresh consideration is prudent to defeat a later consideration challenge.
4. **Former-engineer outreach.** The outreach letter, the named-GC-signature posture, the economic incentive (if any), and the diligence-ready documentation of the attempt even where signature is not obtained. Name the risk this creates on the Part B(i) disposition.
5. **Diligence-ready schedule.** The chain-of-title manifest the GC will produce — one row per material contributor, name, employment / contractor status, PIIA-executed date (or the nunc pro tunc date), the modules authored, and the open-items flag where signature could not be obtained.

### Part G — Series-B diligence IP schedule

Author the schedule the GC will produce in advance of the Series-B diligence request, so that the diligence workstream opens with the IP package clean.

1. **Patent register.** Filed applications, provisionals in-flight, abandoned applications, and the Part B disposition decisions. Format as a table.
2. **Trademark register.** US and international marks, their § 1051 basis, their Nice classes, their filing / registration / renewal dates, and the clearance opinion of record.
3. **Copyright register.** Works registered, registration numbers, effective dates, and the Part D works that are deliberately unregistered with the rationale.
4. **Trade-secret identification register.** The output of Part E — the maintained register of items the corporation treats as trade-secret, with the "reasonable measures" evidence pack cross-indexed.
5. **Chain-of-title manifest.** The output of Part F.
6. **Open-source inventory.** Cross-reference to [chapter 05](../05-open-source-hygiene-and-sbom-programme.md) — the SBOM / OSS-licence inventory, including copyleft exposure. Do not re-author the OSS programme; cite the chapter 05 artefact.
7. **Open-items log.** The honest list of defects that remain at week twelve — PIIA signatures still outstanding, pending clearance opinions, pending non-provisional conversions, pending international-filing decisions. Diligence counsel reads an honest open-items log more favourably than a schedule that pretends everything is clean.

## Starter guidance

- Chapter 04 is the primary reference. Part A is the invention-disclosure programme the chapter opens on; Part B walks each disclosure through the statutory frame the chapter sets out (§§ 101 / 102 / 103 / 112, *Alice* / *Mayo* / *Bilski*, the on-sale bar, detectability-of-infringement); Part C is the trademark discipline the chapter describes; Part D is the copyright-registration slate the chapter frames around § 408 / § 411 / § 412; Part E is the DTSA-reasonable-measures programme; Parts F and G are the chain-of-title and diligence artefacts the chapter opens on as the Series-A → Series-B justification for the whole programme.
- Chapter 04 is explicit that the Series-A posture is **selective**, not exhaustive. Resist the pattern of filing provisional on every disclosure. Each Part B disposition should carry a defensible "why this disposition and not the alternatives" paragraph.
- Chapter 04 is also explicit that **detectability-of-infringement** is the pivot test on the patent-vs-trade-secret question. Reach a specific answer per disclosure; "it depends" is not a disposition.
- Do not pre-decide which of the three invention disclosures is a patent and which is a trade secret. Reach the answer through the frame.
- Defer the PIIA architecture to [mod-103](../../mod-103-employment-law-and-contract-design/) and the founder-era pre-formation IP posture to [mod-102](../../mod-102-founding-team-legal-architecture/); defer the contractor-SOW IP-assignment drafting to [chapter 03](../03-vendor-contract-suite-and-onboarding-workflow.md); defer the OSS / SBOM inventory to [chapter 05](../05-open-source-hygiene-and-sbom-programme.md); defer the records-retention policy to [mod-101](../../mod-101-legal-entity-formation-and-corporate-structure/); defer the privacy overlay on personal-data trade secrets to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/). Reference the cross-modules; do not re-author.
- Any specific fee figure — USPTO filing fees, utility-patent prosecution cost, full-clearance-search cost, Copyright Office eCO fee, LOT Network membership tier, IP.com defensive-publication fee, international-filing fees in Canada / UK / Australia — gets `<!-- needs-research: ... -->`. Do not invent dollar amounts. The chapter 04 fee ranges that are quoted with `<!-- needs-research: ... -->` discipline propagate into the exercise draft the same way.
- Any specific benchmark figure — the quality-edge delta on the Part B(iii) industry benchmark, the latency-signature observability on Part B(i), the design-partner count — may be named in operating terms but any quantitative claim should carry `<!-- needs-research: ... -->` if it is not grounded in the problem statement.
- No real-company names (no "Wilson Sonsini drafted this", no "Cooley reviewed this"). Chapter 04 names outside counsel firms as examples of diligence-side counsel; the exercise narrative does not retain any as the corporation's named adviser.
- Nothing in this exercise is a legal opinion. The Part B dispositions are operating recommendations the GC takes to outside IP counsel for the formal filing decision; the Part C clearance opinion is counsel-produced; the Part F nunc pro tunc assignments go through counsel. Flag the counsel sign-off step in each part.

## Deliverables

- `invention-disclosure-programme.md` — Part A.
- `patent-trade-secret-decisions.md` — Part B.
- `trademark-portfolio.md` — Part C.
- `copyright-registration-posture.md` — Part D.
- `trade-secret-programme.md` — Part E.
- `piia-remediation-plan.md` — Part F.
- `diligence-ip-schedule.md` — Part G.

## Acceptance criteria

The package is acceptable if:

1. Part A's invention-disclosure programme specifies the intake template as operative fields (title, named inventors with contribution shares, conception date, first disclosure outside, § 112 enabled description, prior art known, § 102(b)(1) public-use / on-sale status, recommended disposition), the named triage roles and cadence, and the stage-appropriate filter criteria the triage committee applies before any filing-fee is spent.
2. Part B reaches a specific disposition for each of the three disclosures — file provisional, file utility, provisional-then-utility, trade-secret only, or defensive publication — with the rationale explicit on §§ 101 / 102 / 103 / 112, the *Alice* / *Mayo* / *Bilski* subject-matter frame, the on-sale and public-disclosure bars under § 102(b)(1), the first-inventor-to-file posture under AIA, and the detectability-of-infringement test. "It depends" dispositions are unacceptable.
3. Part B names the clock-start date (if any) for each disclosure under § 102(b)(1), with specific attention to disclosure (ii)'s design-partner NDA posture and marketing-site screenshot, and disclosure (iii)'s engineering-blog benchmark publication.
4. Part C specifies the § 1051(a) use-in-commerce vs. § 1051(b) intent-to-use basis for each US filing, the Nice classes (Class 9, Class 42, others as applicable), the TEAS Plus / TEAS Standard decision, the clearance posture (knockout + full clearance) with counsel opinion gating public launch, the Madrid Protocol vs. direct-filing decision for Canada / UK / Australia with the central-attack trade-off addressed, a month-indexed twelve-month filing calendar, and a budget envelope that defers specific fees to `<!-- needs-research: ... -->`.
5. Part C flags the company-mark descriptiveness exposure under § 1052(e) explicitly and names the domain / social-handle acquisition workstream to run in parallel with the filings.
6. Part D names the works that go through registration, the works that deliberately stay unregistered with the rationale, the § 411(a) / *Fourth Estate* prerequisite-to-suit mechanics, the § 412 three-month-post-publication window for preserving statutory damages and attorney fees, and the DMCA § 512 safe-harbour posture (including whether safe-harbour in fact applies to Halyard Flow's Service).
7. Part E's trade-secret programme covers identification-and-classification, access control, marking, personnel controls (with the 18 U.S.C. § 1833(b)(3) notice cross-referenced to the [mod-103](../../mod-103-employment-law-and-contract-design/) PIIA), exit-interview protocol, and audit-trail logging — all tied to the 18 U.S.C. § 1839(3) "reasonable measures" standard.
8. Part F names the 14-engineer population, breaks it down by current / former status and by material-contribution-to-production-code, specifies the nunc pro tunc assignment posture, specifies the incremental-consideration mechanic (nominal cash, RSU grant, or continued-employment framing) with the practitioner-canon discipline that fresh consideration is prudent, specifies the former-engineer outreach plan, and produces the diligence-ready chain-of-title manifest.
9. Part F names the risk the chain-of-title gap creates on the Part B(i) scheduling-algorithm disposition — the module authored in part by 2021-contractor-cohort engineers whose assignment is not clean — and specifies how the Part B(i) disposition addresses that risk (file over cleaner assignments only, defer the filing until signatures are obtained, or document the open-item for diligence).
10. Part G produces the Series-B diligence IP schedule as a set of named registers — patent register, trademark register, copyright register, trade-secret identification register, chain-of-title manifest, OSS inventory (cross-referenced to [chapter 05](../05-open-source-hygiene-and-sbom-programme.md)) — and an honest open-items log naming the defects that remain at week twelve rather than pretending the schedule is clean.
11. Deferrals to sibling modules and chapters are named explicitly: [mod-101](../../mod-101-legal-entity-formation-and-corporate-structure/) for records-retention, [mod-102](../../mod-102-founding-team-legal-architecture/) for founder-era pre-formation IP, [mod-103](../../mod-103-employment-law-and-contract-design/) for the PIIA architecture and DTSA whistleblower notice, [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/) for the privacy / personal-data overlay, [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md) for the outbound IP indemnity the IP programme underwrites, [chapter 03](../03-vendor-contract-suite-and-onboarding-workflow.md) for contractor-SOW IP assignment, and [chapter 05](../05-open-source-hygiene-and-sbom-programme.md) for the OSS / SBOM inventory. Mechanics owned by those references are not re-authored in the deliverable.
12. Any specific fee or benchmark figure not grounded in chapter 04 or the problem statement is flagged with `<!-- needs-research: ... -->`. No real-company names are invented as the corporation's named adviser. Nothing is left as `[TBD]` or `[FILL IN]`.
