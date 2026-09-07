# Exercise 01 — W-2 vs. 1099 worker-classification decision matrix

> Estimated time: **~4 hours** · Related chapter: [01 — W-2 employee vs. 1099 independent contractor](../01-w2-vs-1099-worker-classification.md)

## Problem statement

Acme Robotics is a 22-person Delaware C-corp with employees in San Francisco (7), Los Angeles (2), Seattle (3), Austin (4), Boston (3), Chicago (2), and Denver (1). The CEO has just been asked by the incoming COO (you) to run a "contractor-vs-employee cleanup" on the current non-founder workforce and the queued Q4 hiring plan. Historically, engagements were papered as 1099 contractors whenever the person "wasn't full-time," "preferred it," "worked from home," "wanted flexibility," or "was on a three-month trial." The Head of Finance has asked how much exposure the corporation is carrying and what to do about the incoming Q4 requisitions.

You are producing (a) a worker-classification decision matrix that classifies each existing and incoming role under the applicable federal and state tests, (b) a quantified misclassification-exposure memo for the mis-papered subset, and (c) a remediation plan.

## Roster and pipeline

Each row lists the role, the location, the current or intended paper structure, and the operational facts you have.

### Currently engaged (year-to-date at $ annualised rate)

1. **Andre — Senior Software Engineer — San Francisco — 1099 at $220k.** Works 45–55 hours/week on the corporation's core inference product. Uses corporation-issued MacBook and Slack. Attends daily standups. Reports to CTO. No other clients. Engagement letter is a one-page "Consulting Agreement" that references a "Statement of Work" that was never signed. Started 9 months ago, "trial for the first three months then we'll see."
2. **Bea — Product Designer — Los Angeles — 1099 at $140k.** Works 30–35 hours/week, 100% on Acme's product design. Owns her equipment and works from her own studio. Has one other client (a marketing agency) that occupies ~5 hours/week. Attends the Acme weekly design review; her deliverables are tracked in Acme's project-management system. Started 5 months ago.
3. **Chen — Salesforce Administrator — remote (Seattle) — 1099 at $95k.** Works 20 hours/week, on Acme's Salesforce instance only, on Acme-defined tasks. Has been "consulting" for 14 months. Works from home using their own laptop. Invoices monthly via a personal PayPal account.
4. **Dara — Inside Sales Representative — Austin — 1099 at $80k base plus commission.** Uses Acme CRM, is territory-assigned by the VP of Sales, attends weekly sales standup, has an @acmerobotics.com email address, sells only Acme products. Started 8 months ago as an "independent sales agent."
5. **Elena — Fractional CFO — Boston — 1099 at $180/hour, ~40 hours/month.** Runs her own advisory practice (Elena Advisory LLC). Currently serves five other early-stage clients. Sets her own hours, works from her own office, reviews Acme's books monthly, presents to Acme's board quarterly. Uses her own accounting-tools stack.
6. **Frank — Full-Stack Engineer — Chicago — W-2 at $180k, salaried, "exempt."** Works 40–50 hours/week. Reports to CTO. FLSA salary basis is met; the duties-test analysis is deferred to exercise 02.
7. **Gina — Recruiter — Denver — 1099 at $120k retainer + $8k per placement.** Runs her own recruiting practice. Has two other startup clients. Sources exclusively engineering roles for Acme (per her SOW).
8. **Hana — Customer Success Manager — San Francisco — W-2 at $110k.** New hire; joined last month.

### Q4 hiring plan (proposed paper structure)

- **Two Senior Software Engineers (San Francisco, Boston)** — proposed W-2.
- **One Head of Marketing (LA)** — proposed W-2.
- **One "Marketing Ops Consultant" (LA)** — proposed 1099, $110k, 30 hours/week, on Acme's marketing tech stack, exclusive to Acme, "we may convert to W-2 after 6 months."
- **One Video Producer (contract engagement)** — the Q4 recruiting video. Vendor is B Films LLC, delivering a 90-second recruiting video for a flat $18k on a defined SOW; they own their equipment, work from their studio, have five other clients.
- **One EA to CEO (San Francisco)** — proposed W-2.
- **Six "Enterprise Sales Development Representatives" (distributed across all cities except Denver)** — proposed 1099, $60k base + commission, "outbound only, they can work whenever they want, we're not paying benefits, we're calling them contractors so we can flex the team size."

## Requirements

### Part A — Classification matrix

Produce a table with one row per current engagement (1–8) and one row per Q4 proposed hire, with columns for:

1. **Role / name / location.**
2. **Current or proposed paper structure** (W-2 or 1099).
3. **IRS common-law test** — apply the three-category framework (behavioural control, financial control, type of relationship). State the operational facts on each side.
4. **FLSA economic-realities test** — apply the six-factor totality analysis.
5. **State ABC test if applicable** — California (Cal. Lab. Code § 2775), Massachusetts (M.G.L. c. 149 § 148B). Prong-by-prong analysis. Note any statutory exceptions (Cal. Lab. Code § 2776 business-to-business, § 2778 professional services) that might apply.
6. **Correct classification per applicable tests.** W-2 or 1099.
7. **Confidence level.** High / medium / low. Any test that returns different answers across the three federal tests or between federal and state should be low-confidence unless a single test unambiguously governs.
8. **What changes if the answer is W-2** — payroll setup, FICA / FUTA / state UI / workers'-comp, benefits eligibility, PIIA execution (chapter 04), offer-letter reissuance (chapter 03), FLSA exempt-vs-non-exempt classification (deferred to exercise 02).

### Part B — Exposure memo for mis-papered engagements

For each engagement you classify as *currently mis-papered as 1099 when it should be W-2*, produce a quantified exposure entry per chapter 01's "consequences of misclassification, quantified" section:

- **Federal employer FICA back exposure** — 7.65% (with the appropriate Social Security wage-base cap and Additional Medicare threshold applied). Flag current-year Social Security wage base as a `<!-- needs-research -->` item.
- **Federal income-tax withholding assessed at 24% supplemental rate**, with a note on the IRC § 3402(d) / Rev. Proc. 2004-56 partial-mitigation pathway.
- **State unemployment insurance** — state-specific rate assumptions with citation to the applicable state agency, plus penalty and interest posture.
- **Workers'-compensation** — industry-rate assumption with citation, plus state-specific penalty posture (e.g., California stop-work-order and civil-penalty framework).
- **FLSA back overtime + liquidated damages** — for any misclassified worker who is also arguably non-exempt (defer the exempt-vs-non-exempt analysis to exercise 02, but flag which workers require the additional analysis).
- **State wage-and-hour additions** — California daily overtime, meal-and-rest premiums, Cal. Lab. Code § 226 wage-statement penalties, § 203 waiting-time penalties, § 2802 expense reimbursement, PAGA per-pay-period penalties.
- **Benefits catch-up exposure** — brief; note the ERISA / plan-document dependence.
- **IRC § 6672 personal liability** — brief; identify the corporation's "responsible person(s)" (CEO, CFO/Head of Finance, COO) whose personal, non-dischargeable exposure this creates.

Aggregate the per-worker exposure into a total number. Do not manufacture precision — round appropriately and note the ranges. Where a `<!-- needs-research -->` marker is applicable (current-year Social Security wage base, current DOL 29 C.F.R. Part 795 status, current PAGA reform terms), flag it in-line rather than picking a number.

### Part C — Q4 hiring-plan gating

For the six proposed Q4 hires (SDRs), the marketing ops consultant, the video producer, the EA, the SWEs, and the Head of Marketing, produce a go / no-go decision for the proposed paper structure. Where you say "no-go," specify the correct paper structure and any additional preconditions (e.g., "corporation must register as an employer with California EDD before the LA hire can be onboarded," "video producer engagement letter must reflect the SOW-with-milestones structure per chapter 01").

Explicitly reject the "consultant-to-hire" pattern for the marketing ops consultant per chapter 01's "consultant-to-hire transition trap" section. Substitute a compliant alternative (W-2 hire with introductory-period framing).

Address the SDR pool explicitly. The "we're calling them contractors so we can flex the team size" rationale is a fail; explain why per the "why 'the engineer only works 20 hours a week' argument loses" section.

### Part D — Remediation plan for existing mis-papered engagements

For each engagement you classify as currently mis-papered, produce a specific remediation-path recommendation. Choose from and justify:

1. **Convert to W-2 prospectively.** Effective date, communications plan, payroll setup, benefits enrollment, PIIA execution, exposure-mitigation posture (do we self-audit and file amended payroll returns? do we look at the Voluntary Classification Settlement Program per Announcement 2011-64? does the corporation approach the worker to acknowledge the change and preserve continuity of assignment?).
2. **Terminate the engagement.** If the engagement no longer makes economic sense as a W-2 (e.g., the worker's actual weekly hours are too low to justify the W-2 overhead and the corporation cannot restructure the work into a legitimate contractor SOW).
3. **Restructure the engagement.** For any engagement that could genuinely satisfy the applicable tests as a contractor with different operational facts (e.g., limited scope of work, defined deliverables, independent tools, other clients). Note that this is rare in practice.

Address specifically:

- Whether to pursue VCSP (Announcement 2011-64) as the federal-side mitigation strategy. Note the eligibility criteria and the payment computation, and flag the current-year VCSP terms as a `<!-- needs-research -->` item.
- Whether the California engagements (Andre, Bea) require an EDD self-audit disclosure or a Labor Commissioner reporting posture. Advise, and cite chapter 01's enforcement-channel section.
- What the corporation says to each affected worker, and in what order. This is a sensitive communication with legal, tax, and employee-relations dimensions.

### Part E — Design-choices memo

A 2–3 page memo covering:

- The framework you applied and why (chapter 01's decision-framework distillation).
- The three worker-classification decisions you found hardest and how you resolved them. Elena (fractional CFO), Gina (recruiter), and the video producer are candidates; explain what tipped each one.
- The corporation-level policy you recommend going forward: default posture, gating for any proposed 1099 engagement, engagement-letter template (SOW-with-milestones vs. employment agreement), review cadence, and role of counsel.
- The § 530 safe-harbour analysis — whether the corporation has any credible § 530 defense (chapter 01's section on § 530). Almost certainly no, but state the analysis.
- Any `<!-- needs-research -->` items you flagged and how the corporation should resolve them (current DOL 29 C.F.R. Part 795 status, current-year Social Security wage base, current-year VCSP terms, current PAGA reform terms, current state-by-state ABC-test scope).

## Starter guidance

- Chapter 01 is the primary reference. The three-category IRS common-law framework, the six-factor FLSA economic-realities framework, and the three-prong ABC framework are laid out there.
- California's prong (B) — "outside the usual course of business" — is the most disqualifying prong for a software-industry contractor and should be the first prong you apply for any Californian.
- The "consultant-to-hire" trap and the "20 hours a week means contractor" argument are addressed in the chapter — cite the specific sections when you reject the CEO's or the Head of Finance's framing.
- Do not manufacture facts. If a fact is not in the roster, mark it as an open question. E.g., you do not know Bea's LLC status; state that you would want to know before finalising, and note how the answer would change the analysis.
- Do not attempt the FLSA exempt-vs-non-exempt analysis for the W-2 population here — that is exercise 02. Flag the population that requires it.
- The exposure numbers are ranges, not point estimates. The chapter's $60k–$150k per-worker range for a full-time misclassified engineer is a reasonable order-of-magnitude anchor.
- The state-agency and enforcement-channel section of chapter 01 is the reference for who does what — do not assume the IRS is the only worry. The California EDD and Labor Commissioner are the more-likely triggers in California.

## Deliverables

- `classification-matrix.md` — Part A.
- `misclassification-exposure-memo.md` — Part B.
- `q4-hiring-plan-gating.md` — Part C.
- `remediation-plan.md` — Part D.
- `classification-design-choices-memo.md` — Part E.

## Acceptance criteria

The package is acceptable if:

1. Every engagement (current 1–8 and Q4 proposed) is classified under the applicable federal and state tests, with the operational facts marshalled on each side of each test.
2. Andre is classified as W-2 with high confidence; the "consulting for the first three months" rationale is explicitly rejected.
3. Bea's classification identifies California's prong (B) as dispositive and rejects the paper-title label.
4. Chen's classification identifies indefinite-duration + single-client + Acme-defined-tasks as disqualifying for contractor status.
5. Dara's classification identifies behavioural control (CRM, territory, standup, email address) as dispositive.
6. Elena and the video producer are correctly classified as defensible 1099s with the specific factors (independent practice, multiple clients, project scope, own tools) called out. Do not misclassify these as employees.
7. Gina's classification is medium-confidence; the analysis identifies both directions and picks a defensible answer.
8. The Q4 SDR pool is rejected as 1099 with the correct reasoning; the marketing-ops "consultant-to-hire" is rejected with the correct reasoning.
9. Every current mis-papered engagement has an exposure number (with ranges), the identified California engagements carry Cal. Lab. Code § 226 / § 203 / PAGA add-ons, and the § 6672 personal-liability exposure is identified with the specific responsible persons.
10. The remediation plan for each mis-papered engagement is specific (effective date, communications, payroll setup, PIIA execution, benefits enrollment, § 530 / VCSP analysis) and does not paper over the difficulty of the worker communication.
11. Statutory citations (IRS Rev. Rul. 87-41, 29 C.F.R. Part 795 as currently operative, Cal. Lab. Code § 2775, Cal. Lab. Code §§ 2776 and 2778 exceptions, IRC § 6672, IRC § 3402(d), Rev. Proc. 2004-56, VCSP Announcement 2011-64) are correct.
12. Nothing left as `[FILL IN]` or `[TBD]` — every field populated or explicitly flagged with a `<!-- needs-research -->` marker.
