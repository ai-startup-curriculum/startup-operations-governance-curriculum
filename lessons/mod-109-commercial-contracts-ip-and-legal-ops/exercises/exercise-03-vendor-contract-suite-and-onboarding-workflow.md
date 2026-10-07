# Exercise 03 — Vendor contract suite and onboarding workflow

> Estimated time: **~8 hours** · Related chapter: [03 — The vendor contract suite and vendor-onboarding workflow](../03-vendor-contract-suite-and-onboarding-workflow.md)

## Problem statement

Harborlane Analytics is a Series-B Delaware C-corp selling a merchandising-and-replenishment product into mid-market enterprise retail. The corporation is 110 FTE, closed its Series B eleven months ago, and operates out of a hybrid HQ in Boston plus a Toronto engineering pod. The corporation inherited roughly 125 active vendor agreements from the Series-A era as a Google Drive folder (unindexed) plus a stale spreadsheet last touched by a founding-ops lead who departed six weeks ago. Three facts are forcing a vendor-architecture decision now. First, the CFO's quarterly spend review has flagged approximately **$340k of apparent duplicate SaaS spend** across two overlapping observability vendors (one inherited, one introduced by the new VP engineering) and two overlapping product-analytics vendors (one introduced by growth, one by product). Second, the head of security has flagged **two Tier-1 vendors with no executed DPA on file** — one payroll-adjacent, one customer-support — both of which process employee or customer PII today. Third, **two in-flight enterprise sales deals** have been held up in the last six weeks by customer-side vendor-and-subprocessor questionnaires the corporation could not answer in less than ten days, because the subprocessor list is not centrally maintained.

Three live vendor requests sit in-queue as test cases for the architecture you are about to build. (i) **Lumenware AI** — a $65k/yr enterprise AI-inference provider that will process customer-identifiable prompts; engineering wants to onboard this quarter and has already run a 30-day POC under an informal email exchange with no NDA on file. (ii) **PulseFunnel** — a $9k/yr vendor-selected clickthrough-contract product-analytics tool that marketing self-provisioned four weeks ago and is now asking IT for SSO integration and a shared workspace. (iii) **Northfield Data Partners** — a $220k 12-month implementation SOW with a boutique consulting firm to migrate the data warehouse; the vendor has sent its own SOW template and is pushing for a kickoff in three weeks.

The head of legal ops has **eight weeks** to publish the vendor-contract architecture — tier framework, template pack, onboarding workflow, delegation of authority, auto-renewal register — and to walk the three live requests through it as the first-run worked examples. Author the full package.

## Requirements

### Part A — Vendor-tier framework

Draft `vendor-tier-framework.md` covering:

1. **Three named tiers** — Tier-1 (strategic, data-processing, or Tier-1 security surface), Tier-2 (material spend, moderate security surface), Tier-3 (routine SaaS, clickthrough acceptable) — each with a one-paragraph definition in operative language a business-unit requester can read.
2. **Tier-assignment criteria** as an explicit decision matrix. Name the Harborlane-specific thresholds: annual-contract-value bands, data-class matrix (public, internal, confidential, regulated — defer the data-classification schema to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/)), SSO-required flag, DPA-required flag, SIG-required flag, infra-dependency flag. Do not invent industry benchmarks for the ACV bands; propagate `<!-- needs-research: ... -->` for any threshold not in chapter 03 or `resources.md`.
3. **Override and escalation** — the named decision point at which security or legal escalates a vendor to a higher tier than the matrix auto-assigns, and the discipline that the auto-assign is the floor, not the ceiling.
4. **Tier-based treatment table** — what each tier gets by way of legal review depth, security review depth, DPA posture, insurance-certificate requirement, and re-review cadence. Reference [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/) for the vendor-insurance minimums and third-party-risk register; do not re-author that mechanic here.

### Part B — Vendor template pack

Author `vendor-template-pack/` as a set of five scoped template-posture documents (not full redlined contracts — the posture notes a counsel would hand to a drafter). Cover:

1. `vendor-msa-posture.md` — the accept-with-redlined-clauses pattern below the Harborlane ACV threshold; the short list of clauses that get redlined even on accept-vendor-paper deals (auto-renewal opt-out, data ownership, DPA execution, security-addendum reference); the mirror-image redline posture from [chapter 02](../02-contract-playbook-and-fallback-position-matrix.md) for above-threshold deals.
2. `sow-template-posture.md` — fixed-fee vs. T&M mechanics, enumerated-deliverables discipline, objective acceptance criteria, lapse-based acceptance window (name a defensible window), change-order mechanics, the three-layer IP framework from chapter 03, and the SOW-vs-MSA order-of-precedence posture.
3. `contractor-agreement-posture.md` — IP-assignment and work-for-hire language per chapter 03. **Defer the DTSA whistleblower-notice mechanics, the *Stanford v. Roche* "hereby assigns" drafting rule, and the state-law classification overlay (CA AB5, state analogues) to [mod-103](../../mod-103-employment-law-and-contract-design/).** Note the deferrals explicitly in the template header.
4. `mnda-and-unilateral-nda-posture.md` — direction, when the corporation uses mutual vs. unilateral, the gate that the NDA executes before substantive discovery (defer anatomy of the NDA — standard exceptions, DTSA carveout, dispute resolution — to [mod-103](../../mod-103-employment-law-and-contract-design/)).
5. `vendor-dpa-posture.md` — the review checklist chapter 03 names (sub-processor list and change-notice mechanics, data-residency and cross-border transfer basis, data-return-and-destruction, breach-notification timeline, audit or SOC-2 provision, right to instruct); **defer the privacy-regulatory depth (GDPR Art. 28, CCPA/CPRA § 1798.140 service-provider analysis, SCCs, UK IDTA, Data Privacy Framework) to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/)**.

### Part C — End-to-end onboarding workflow

Draft `onboarding-workflow.md` covering:

1. **Intake form fields** — the specific fields a requesting business-unit owner fills in (vendor name, category, business case, expected ACV, data category, urgency, SSO-required, existing-contract-on-file). The intake drives the initial tier auto-assignment from Part A.
2. **Routing decision** — the branching logic from intake to the parallel work streams (legal, security, privacy, procurement, IT). Specify where Tier-3 is a self-serve path against an allow-list and where Tier-1 and Tier-2 enter the full workflow.
3. **Parallel work streams** — DPA execution for Tier-1 and Tier-2; SecReview against SOC 2 Type II or SIG-lite for Tier-1 and Tier-2; procurement approval against the Part D delegation of authority; finance / spend-management handshake; SSO / access provisioning via the corporation's identity provider; CLM filing. **Defer the CLM-tool mechanics (which product, which schema, which obligation-reminder cadence) to [chapter 07](../07-clm-stack-and-legal-ops-graduation.md).**
4. **Visual-friendly step list** — present the end-to-end flow as a numbered-step list or a swim-lane sketch readable by a non-legal audience. Name the dwell-time target for each stage under the Harborlane posture (Tier-1 full workflow 4–8 weeks, Tier-2 2–4 weeks, Tier-3 self-serve 1–2 weeks) and the named gate that no step is skipped above Tier-3.
5. **Exception path** — the named route when a business unit has already signed a vendor without going through onboarding (the "quarter-end rep hands over an order form" pattern from chapter 03). Specify the retroactive-remediation posture, not punishment theatre.

### Part D — Delegated authority matrix

Draft `delegated-authority-matrix.md` covering:

1. **Named signing authority by tier and by ACV band** — who can sign at what tier and up to what spend without executive approval. Build the matrix against named Harborlane roles (manager, director, VP, CFO, CEO, board), not abstract levels. Include the data-class overlay (any regulated-data vendor, regardless of ACV, requires a named officer signature).
2. **Corporate-authority citations** — name the officer-authority instruments that back the delegation. **Defer the officer-authority mechanics (bylaws delegation, board-resolution-based signing authority, incumbency certificate practice) to [mod-101](../../mod-101-legal-entity-formation-and-corporate-structure/).** Reference the mechanic; do not re-author it.
3. **Delegation hygiene** — the discipline that delegations are written, periodically reviewed, revoked on departure, and audited against the CLM record of signed contracts; the specific trigger that forces an authority review (new officer, departed officer, M&A, board-composition change).
4. **Over-authority / unauthorised-signature remediation** — the named path when a non-authorised signer executes a vendor contract. Name the ratification-vs-void posture and the organisational-signaling cost of under- or over-reacting.

### Part E — Auto-renewal opt-out discipline

Draft `auto-renewal-register.md` covering:

1. **The obligations the CLM must track for every vendor** — notice window (named days before term-end), counterparty notice contact (named email / portal / certified mail per the vendor's MSA), pricing-escalator cap and index, change-of-control notice obligation, insurance-certificate renewal date, DPA-re-execution trigger, SOC 2 re-review date.
2. **The notice-window calendar** — the published calendar discipline (calendared reminder at least two weeks before notice deadline per chapter 03) and the escalation path when a reminder goes unactioned.
3. **Kill-switch when a non-renewal window is being missed** — the named role (head of legal ops, with finance and the business owner on-copy) empowered to send the non-renewal notice when the business owner has gone silent for a named number of days before deadline; the carve-out for Tier-1 vendors where renewal-vs-replacement is an executive decision.
4. **Backfill posture for the 125 inherited contracts** — a named triage approach to populate the register from the Google Drive folder plus stale spreadsheet without doing a 125-contract redline-from-scratch exercise. Name the sequence (Tier-1 first, Tier-2 second, Tier-3 batch) and the acceptable completeness bar for the eight-week publication deadline.

### Part F — Three worked onboarding scenarios

Draft `worked-scenarios.md` walking each of the three live vendor requests through the Part A–E architecture. For each scenario, produce:

1. **Tier assignment** — the specific tier from the Part A matrix, with the triggering criteria named.
2. **Redline posture** — which clauses the corporation pushes on and which it accepts under the Part B posture; the specific carve-outs from the chapter 03 mirror-image matrix that matter for this vendor.
3. **DPA / SecReview outcome** — whether a DPA is required (and if so, what the Part B DPA checklist flags), whether SOC 2 Type II or SIG-lite is required, and the specific SecReview conditions that must clear before SSO / access provisioning.
4. **Workflow disposition** — the specific intake-to-filed path, named dwell-time estimates, named approver per stage, and the final go / no-go / go-with-conditions recommendation.
5. **Specific scenario notes:**
   - **Lumenware AI ($65k AI inference, customer-identifiable prompts, 30-day POC already run under no NDA).** Address the retroactive-NDA posture, the AI-vendor-specific DPA depth, and the data-residency question. Defer the AI-specific contract depth (training-data use carve-outs, model-output IP, prompt-logging posture) to [chapter 06](../06-ai-vendor-contracts-and-ai-dpa-pattern.md).
   - **PulseFunnel ($9k clickthrough analytics, self-provisioned by marketing, SSO request in-queue).** Address the retroactive-remediation path from Part C step 5, the tier-assignment question (Tier-3 by ACV, but does the data-class trip it up?), and the vendor-paper-accept posture.
   - **Northfield Data Partners ($220k 12-month SOW, vendor-sent template, three-week kickoff pressure).** Address the vendor-template-vs-corporation-template posture, the three-layer IP framework application, the acceptance-criteria discipline against the warehouse migration deliverable, and the delegation-of-authority question (does the ACV cross the CFO signature threshold?).

## Starter guidance

- Chapter 03 is the primary reference. The vendor-tier framework, the five-document template pack, and the eight-step onboarding workflow all map directly onto Parts A, B, and C. Do not re-author the chapter; author Harborlane-specific posture against it.
- The sell-side mirror in [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md) and the redline matrix in [chapter 02](../02-contract-playbook-and-fallback-position-matrix.md) are load-bearing. The Part B redline posture is the mirror image of the sell-side playbook — reference it, do not re-author it.
- Any ACV threshold, dwell-time target, or industry benchmark not in chapter 03 or `resources.md` gets `<!-- needs-research: ... -->`. The chapter's "typical" numbers (e.g., $25k–$50k accept-vendor-paper threshold) are directional; propagate the research-flag discipline into your Harborlane-specific thresholds.
- Defer the privacy-regulatory depth (GDPR Art. 28, CCPA/CPRA § 1798.140 service-provider analysis, SCCs, UK IDTA, DPF, breach-notification regulatory timelines) to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/). Reference the mechanic; do not re-author it.
- Defer the vendor-insurance minimums (CGL, E&O, cyber-liability floors, additional-insured mechanics) and the enterprise third-party-risk register to [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/). The Part A tier table names *that* an insurance certificate is required; the dollar floors live in mod-112.
- Defer the officer-authority mechanics underpinning the Part D delegation (bylaws delegation, board-resolution signing authority, incumbency certificate practice) to [mod-101](../../mod-101-legal-entity-formation-and-corporate-structure/).
- Defer the DTSA whistleblower-notice mechanics, the *Stanford v. Roche* present-tense "hereby assigns" drafting rule, state-law worker-classification variance, and the employee-side PIIA interaction to [mod-103](../../mod-103-employment-law-and-contract-design/). The Part B contractor-agreement-posture names *that* these mechanics apply; the substantive drafting lives in mod-103.
- Defer the CLM-tool mechanics (product selection, metadata schema, obligation-reminder cadence configuration) to [chapter 07](../07-clm-stack-and-legal-ops-graduation.md). Parts C and E name *what* the CLM must track; chapter 07 owns *how* it tracks.
- Defer the AI-vendor-specific contract depth (training-data use, model-output IP, prompt-logging, model-change notice, hallucination-and-accuracy posture) to [chapter 06](../06-ai-vendor-contracts-and-ai-dpa-pattern.md). The Lumenware AI scenario in Part F invokes chapter 06 posture; it does not re-author it.
- Do not invent real peer company names. Harborlane Analytics, Lumenware AI, PulseFunnel, and Northfield Data Partners are the only named counterparties.
- The CFO-side cost note from chapter 03 is deliberate — a vendor-architecture rollout is a people-cost and tool-cost exercise, not a free one. Name the implementation cost line items (legal-ops headcount, outside-counsel template work, CLM tooling, SIG-lite subscription if elected, SOC 2 report access fees) without inventing dollar figures.

## Deliverables

- `vendor-tier-framework.md` — Part A.
- `vendor-template-pack/` — Part B, containing `vendor-msa-posture.md`, `sow-template-posture.md`, `contractor-agreement-posture.md`, `mnda-and-unilateral-nda-posture.md`, `vendor-dpa-posture.md`.
- `onboarding-workflow.md` — Part C.
- `delegated-authority-matrix.md` — Part D.
- `auto-renewal-register.md` — Part E.
- `worked-scenarios.md` — Part F.

## Acceptance criteria

The package is acceptable if:

1. Part A names three tiers with operative definitions, publishes an explicit tier-assignment matrix with Harborlane-specific ACV bands, data-class criteria, and the SSO / DPA / SIG / infra-dependency flags, and names an override-and-escalation decision point.
2. Part A's tier-based treatment table covers legal review depth, security review depth, DPA posture, insurance-certificate requirement, and re-review cadence per tier, deferring the vendor-insurance dollar floors to [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/).
3. Part B publishes five scoped posture documents under `vendor-template-pack/` covering the vendor MSA (with the accept-with-redlined-clauses pattern and the mirror-image redline posture from [chapter 02](../02-contract-playbook-and-fallback-position-matrix.md)), SOW mechanics (fixed-fee vs. T&M, enumerated deliverables, lapse-based acceptance window, three-layer IP framework, order of precedence), contractor agreement (IP-assignment and work-for-hire posture with explicit deferral of DTSA notice and state-law variance to [mod-103](../../mod-103-employment-law-and-contract-design/)), mutual and unilateral NDA posture, and vendor DPA posture (with explicit deferral of the privacy-regulatory depth to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/)).
4. Part C's onboarding workflow specifies intake form fields, tier-routing decision, parallel work streams (DPA, SecReview against SOC 2 Type II or SIG-lite, procurement, finance, SSO / access provisioning, CLM filing), named dwell-time targets per tier, a visual-friendly step list, and a retroactive-remediation path for vendors already signed outside the workflow — deferring the CLM-tool mechanics to [chapter 07](../07-clm-stack-and-legal-ops-graduation.md).
5. Part D's delegated authority matrix names signing authority by tier and ACV band against Harborlane role titles, applies a data-class overlay for regulated-data vendors, cites the officer-authority instruments backing the delegation, and defers the officer-authority mechanics to [mod-101](../../mod-101-legal-entity-formation-and-corporate-structure/).
6. Part D includes an over-authority / unauthorised-signature remediation posture (ratification vs. void) and a named trigger-set for authority review.
7. Part E's auto-renewal register names the per-vendor obligations the CLM must track (notice window, counterparty contact, pricing escalator cap and index, change-of-control notice, insurance renewal, DPA re-execution, SOC 2 re-review), the notice-window calendar discipline, a named kill-switch role when a non-renewal window is being missed, and a backfill posture for the 125 inherited contracts under the eight-week deadline.
8. Part F walks each of the three live scenarios (Lumenware AI, PulseFunnel, Northfield Data Partners) through tier assignment, redline posture, DPA / SecReview outcome, workflow disposition, and a go / no-go / go-with-conditions recommendation. The Lumenware scenario addresses the retroactive-NDA posture and defers AI-specific contract depth to [chapter 06](../06-ai-vendor-contracts-and-ai-dpa-pattern.md); the PulseFunnel scenario addresses the retroactive-remediation path and the ACV-vs-data-class tier question; the Northfield scenario addresses the vendor-template-vs-corporation-template posture and the three-layer IP framework application.
9. Any ACV band, dwell-time target, insurance floor, or industry benchmark not in chapter 03 or `resources.md` is flagged with `<!-- needs-research: ... -->`. No real peer company names are invented; nothing is left as `[TBD]` or `[FILL IN]`.
10. Deferrals to sibling modules and chapters are named explicitly where the chapter 03 ownership boundary assigns the mechanic elsewhere — [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md) for the customer-side mirror, [chapter 02](../02-contract-playbook-and-fallback-position-matrix.md) for the redline playbook, [chapter 06](../06-ai-vendor-contracts-and-ai-dpa-pattern.md) for AI-vendor contract depth, [chapter 07](../07-clm-stack-and-legal-ops-graduation.md) for CLM filing mechanics, [mod-101](../../mod-101-legal-entity-formation-and-corporate-structure/) for officer-authority mechanics, [mod-103](../../mod-103-employment-law-and-contract-design/) for the DTSA / *Stanford v. Roche* / worker-classification depth, [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/) for the vendor-DPA regulatory depth, and [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/) for the vendor-insurance minimums and third-party-risk register.
11. The Part A tier framework and the Part C onboarding workflow are internally consistent — the tier auto-assignment from intake drives the workflow branching, and the delegated-authority matrix in Part D keys off the same tier-and-ACV axes used in Parts A and C.
12. The package reads as an operating architecture a legal-ops lead could publish and defend to the CFO, head of security, and head of engineering in the eight-week window — not as a legal treatise and not as a template-pack dump.
