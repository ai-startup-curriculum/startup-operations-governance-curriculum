# Exercise 04 — Background check and fair-chance decision drill

> Estimated time: **~5 hours** · Related chapter: [04 — Reference checks and pre-employment background checks](../04-reference-and-background-checks.md)

## Problem statement

Concord Health is a Series-A digital-health startup, 34 employees. It runs on Rippling as its HRIS, Ashby as its ATS, and Checkr for pre-employment background checks. Concord hires in California (San Francisco, Los Angeles), New York (New York City), Illinois (Chicago), Washington (Seattle), and Massachusetts (Boston). Concord is not a federal contractor and does not currently engage with federally regulated health data (its product sits upstream of the covered-entity boundary today), though HIPAA-adjacent conversations with two enterprise customers are on the near horizon.

Six things have happened over the past 60 days:

1. **Compliance flag.** During a routine internal audit, counsel discovered that the corporation's background-check disclosure document includes the corporation's logo, a two-sentence introduction ("Concord Health is committed to a safe workplace, and we conduct background checks on all new hires..."), and a check-box authorising the disclosure of the results to Concord's insurance broker. Counsel flagged this as an FCRA standalone-disclosure risk.
2. **Adverse-action complaint.** A candidate who received a rescinded offer 45 days ago has sent a demand letter through counsel alleging Concord's adverse-action process was defective (specifically: the pre-adverse-action packet did not include the CFPB Summary of Rights, and the corporation acted the same business day it sent the pre-adverse-action letter).
3. **Fair-chance hit — pending offer.** A candidate has just received a conditional offer for a senior operations role in Los Angeles. The background check has come back with a 2019 misdemeanor conviction for a substance-related offense; the candidate disclosed nothing during the interview process (they were not asked, correctly). The hiring manager is asking to rescind. This is Concord's first fair-chance decision.
4. **Reference-call incident.** A hiring manager was overheard on a reference call for a New York City candidate asking "does she have kids?" and "is she planning to stay in the area?" Both questions are protected-category-adjacent.
5. **Back-channel reference concern.** The founder-CEO is proposing to call a friend at a candidate's current employer to "just get the real story" before extending an offer. The candidate has not authorised this.
6. **International hire.** Concord is finalising its first UK hire (a research scientist in London). The Rippling / Checkr package does not automatically extend to the UK; the operations team wants to know how to run a comparable background check.

Produce (a) a corrected FCRA disclosure and end-to-end operating policy, (b) an incident response for the adverse-action complaint, (c) an individualised-assessment memo and decision for the fair-chance hit, (d) a reference-call remediation and revised playbook, (e) a back-channel-reference policy, and (f) a UK background-check operating procedure.

## Requirements

### Part A — FCRA-compliant disclosure and end-to-end operating policy

1. **Draft a corrected disclosure document** that satisfies the standalone-disclosure requirement of 15 U.S.C. § 1681b(b)(2)(A)(i). Remove the logo, the introductory paragraph, and the insurance-broker check-box. Include only the clear-and-conspicuous statement that a consumer report may be obtained for employment purposes, plus the written-authorisation section (permitted on the same document under § 1681b(b)(2)(A)(ii)).
2. **Draft the corrected authorisation** — the candidate's written consent to procure the report. Include the specific data elements the authorisation must capture.
3. **Draft the state-analogue notices** as *separate documents* for California (ICRAA — including the check-box for the candidate to request a copy of the report; CCRAA where applicable), New York (Article 25), Massachusetts, Washington, and Illinois. These are separate from the federal disclosure document.
4. **Draft the pre-adverse-action letter template** that includes (a) the actual consumer report, (b) the current CFPB Summary of Rights, (c) an explanation of the process, and (d) a wait-period instruction. Specify the waiting period Concord will observe (default 5 business days; longer if state law requires) and cite the source. Flag the CFPB Summary of Rights version and URL as a `<!-- needs-research -->` item to refresh.
5. **Draft the adverse-action letter template** that includes all elements of 15 U.S.C. § 1681m(a) — notice of adverse action; CRA name / address / phone; statement that the CRA did not make the decision; notice of right to obtain a free copy of the report within 60 days; notice of right to dispute accuracy or completeness.
6. **Author the end-to-end operating procedure** — the specific ATS-and-CRA workflow steps, the pipeline stage at which disclosure is sent (post-conditional-offer, not earlier), the ordering of report, the pre-adverse-action trigger, the wait period, and the adverse-action trigger. Include the fair-chance-timing requirements for each of Concord's five US jurisdictions (California CFCA, NYC Fair Chance Act, Illinois Ban-the-Box Act, Washington Fair Chance Act, and any Massachusetts / San Francisco / LA local overlay).

### Part B — Incident response for the adverse-action complaint

Produce an incident-response memo covering:

1. **Diagnosis** — what specifically went wrong (missing CFPB Summary of Rights; same-day adverse-action without a wait period; possibly a defective disclosure document if the same-day letter was based on the pre-corrected disclosure).
2. **Exposure quantification** — the statutory-damages range under 15 U.S.C. § 1681n (willful) and § 1681o (negligent), plus actual damages and attorneys' fees. Note the class-action risk if the disclosure defect and the process defect affected other candidates.
3. **Immediate remediation** — a written response to the candidate's demand letter (in coordination with counsel; the exercise is to structure the analysis, not to draft counsel's letter). Consider whether Concord offers reinstatement of the offer, a settlement, or defends. Recommend a specific path and justify.
4. **Systemic remediation** — the corporation-wide review to identify every candidate in the trailing 12 months who received an adverse action under the defective process, and the decision on whether to affirmatively contact affected candidates.
5. **Attribution and documentation** — the responsible-persons analysis (who signed off on the disclosure document; who ran the same-day adverse action) and the corporation's decision on documentation and, if appropriate, remediation of the responsible-persons pattern.

### Part C — Fair-chance individualised-assessment memo

For the LA senior-ops candidate with the 2019 misdemeanor conviction, produce a full individualised-assessment memo following the EEOC 2012 guidance framework as extended by the California Fair Chance Act (Cal. Gov. Code § 12952) and the Los Angeles Fair Chance Initiative for Hiring Ordinance (if applicable — verify). The memo must cover:

1. **The nature and gravity of the offence** — including whether the offence is directly related to the specific duties of the role.
2. **The time that has elapsed** since the offence (approximately 5 years) and since the sentence completion.
3. **The nature of the job** — the specific duties, responsibilities, and access the role carries. Consider Concord's HIPAA-adjacent trajectory and whether the role touches health data.
4. **Rehabilitation and mitigating factors** — factors the corporation is required to consider under the CFCA.
5. **The written preliminary decision** — Concord's tentative conclusion (rescind, proceed with offer, or a specific mitigation such as delayed access to certain systems).
6. **The written notice to the candidate** — the CFCA-required notice, with the specific content elements the notice must include (the conviction that is the basis; the copy of the report; the candidate's right to respond within a specified window; the specific number of business days; the corporation's contact for the response).
7. **The candidate-response window and process** — what happens if the candidate submits mitigating evidence or a challenge, and how Concord processes that.
8. **The final decision protocol** — after the candidate-response window, how the corporation confirms or reverses the preliminary decision, and how the final adverse-action notice (if any) is delivered.

Do *not* pre-decide the outcome — the exercise is to walk the framework and produce a defensible written analysis. If your analysis lands on "proceed with offer," structure the memo that way. If it lands on "rescind," structure it that way. If it lands on "proceed with a specific mitigation," structure it that way.

### Part D — Reference-call remediation and revised playbook

1. **Incident memo** — the analysis of the hiring manager's protected-category-adjacent questions ("does she have kids?" "is she planning to stay in the area?"). Cite Title VII and analogous NY state / NYC law (including the NYC Human Rights Law's family-status and caregiver protections). Recommend the remediation for the specific candidate (reconstruct the reference-call record, discard the answers to the two protected questions, note the incident, and — if the candidate is under active consideration — do not use the protected-question responses in the decision).
2. **Manager remediation** — the specific coaching and re-training the hiring manager receives before running the next reference call.
3. **Revised reference-check playbook** — the structured template Concord will use going forward. Include:
   - The intro-and-consent script.
   - The relationship-context questions.
   - The competency-evidence questions (mapped to a role's scorecard — use one of the exercise-03 scorecards as an example anchor).
   - The development-areas question.
   - The rehire question.
   - The "anything else?" closer.
   - The explicit *do not ask* list, with a short justification for each item on the list.
4. **The reference-call writeup template** — the artifact stored in the ATS against the candidate record.

### Part E — Back-channel-reference policy

Author the corporation's back-channel-reference policy. Cover:

1. Whether Concord permits back-channels *at all* — and if so, for which roles (director+ only? all senior IC and above? never?).
2. Consent posture — whether Concord notifies the candidate that back-channels may be conducted; whether the candidate can opt out.
3. Structured-question requirement — that back-channel references follow the same rubric as on-panel references.
4. Documentation requirement — that back-channel notes are stored in the ATS against the candidate record.
5. Immediate response to the founder-CEO's proposed back-channel call — a specific recommendation (proceed with a structured call per policy, decline, or seek candidate consent first). Justify.

### Part F — UK background-check operating procedure

Produce the operating procedure for the London research-scientist hire. Cover:

1. **The applicable UK regime** — UK GDPR (Data Protection Act 2018), the DBS (Disclosure and Barring Service) as the lawful source for criminal-history checks, the eligibility of the role for a Basic / Standard / Enhanced DBS check (Basic is the default for most private-sector roles; Standard / Enhanced require statutory authorisation).
2. **The lawful basis for processing** — how Concord establishes a lawful basis under UK GDPR for the background-check processing. Data-minimisation and purpose-limitation posture.
3. **The candidate consent and information notice** — how Concord informs the candidate of the check, the source, the retention period, and the candidate's data-subject rights (access, correction, objection).
4. **The vendor choice** — whether Concord uses Checkr International, HireRight EMEA, Sterling International, or a UK-focused CRA (Zinc, Veremark). Justify.
5. **The comparable scope** — what the UK check does and does not include vs. the US check (employment verification, education verification, sanctions / adverse-media, right-to-work check). Note the right-to-work check is a distinct UK obligation under the Immigration, Asylum and Nationality Act 2006 and is *not* substituted by DBS.
6. **The retention posture** — how long Concord retains the UK background-check results and where they are stored (segregated from the general employee record, similar to the US pattern).
7. **The mod-113 handoff** — a note on which international-workforce operating policy questions Concord defers to [mod-113](../../mod-113-international-expansion-and-global-workforce/) and which Concord decides itself.

Flag the DBS scope and eligibility rules as a `<!-- needs-research -->` item — the specifics shift and any operating policy must be verified against current DBS guidance before use.

## Starter guidance

- Chapter 04 is the primary reference. The four-step FCRA framework, the state-analogue overlay, the ban-the-box / fair-chance framework, and the international variance are all laid out.
- Do not draft counsel's response to the demand letter (Part B). Structure the analysis and let counsel draft. The exercise is the operational and policy design.
- The individualised-assessment memo (Part C) is not a template exercise — it is a real analysis. Land it. Do not punt with "further review required."
- The reference-call incident (Part D) is a Title VII protected-category exposure. The two questions asked ("does she have kids?" "is she planning to stay in the area?") are close to per se problematic — the first is a family-status inquiry; the second is a national-origin / immigration-adjacent inquiry as well as a family-status inquiry. Cite the relevant law without over-claiming (both questions could theoretically be defended in narrow circumstances, but not here).
- The UK background-check procedure (Part F) is deliberately introductory — the deep international coverage is mod-113. The purpose is to establish that the US template does not port.
- Do not invent case names, settlement amounts, or CFCA regulation citations. Where you need a specific citation and are not confident of the current text, flag `<!-- needs-research -->`.
- The pre-adverse-action wait period (5 business days is a common defensible default; some jurisdictions and cases have implied longer) should be cited with the source. Do not treat 5 days as statutory — it is not.

## Deliverables

- `fcra-disclosure-corrected.md`
- `fcra-authorisation-corrected.md`
- `state-analogue-notices/notice-california-icraa.md`, `notice-new-york-article-25.md`, `notice-massachusetts.md`, `notice-washington.md`, `notice-illinois.md`
- `pre-adverse-action-letter-template.md`
- `adverse-action-letter-template.md`
- `end-to-end-background-check-operating-procedure.md`
- `incident-response-adverse-action-complaint.md`
- `individualised-assessment-memo-la-senior-ops.md`
- `reference-call-incident-and-remediation.md`
- `reference-check-playbook-revised.md`
- `back-channel-reference-policy.md`
- `uk-background-check-operating-procedure.md`

## Acceptance criteria

The package is acceptable if:

1. The corrected FCRA disclosure (Part A) contains only the required statement and the authorisation — no logo, no intro, no extraneous check-boxes. It is short and unadorned.
2. State-analogue notices exist as *separate* documents from the federal disclosure; California ICRAA has the required check-box for the candidate to request a copy.
3. The pre-adverse-action letter template includes the actual report, the CFPB Summary of Rights, an explanation, and a wait-period instruction; the adverse-action letter has all six § 1681m(a) elements.
4. The end-to-end procedure honours fair-chance timing in all five jurisdictions — the disclosure is not sent until post-conditional-offer.
5. The incident-response memo (Part B) quantifies exposure with reference to §§ 1681n and 1681o, identifies the systemic-remediation obligation across the trailing 12 months, and recommends a specific response path.
6. The individualised-assessment memo (Part C) walks the EEOC-plus-CFCA framework end-to-end and lands on a specific preliminary decision — it does not punt.
7. The CFCA notice content in Part C includes the specific content elements the statute requires (basis of decision; copy of report; response window; corporation contact).
8. The reference-call incident (Part D) cites Title VII and the NYC Human Rights Law family-status / caregiver protections; the manager-remediation is specific.
9. The revised reference-check playbook includes an explicit *do not ask* list with justifications; the structured questions map to a scorecard.
10. The back-channel-reference policy takes a position (permit for director+ with candidate consent, or decline; either is defensible) and gives the founder-CEO a specific recommendation on the pending call.
11. The UK background-check procedure names DBS as the criminal-history source, cites UK GDPR and the right-to-work Immigration, Asylum and Nationality Act 2006 obligation, and identifies a specific vendor.
12. Every legal citation is either taken from chapter 04 or flagged with `<!-- needs-research -->` — no fabricated case names or made-up statute sections.
