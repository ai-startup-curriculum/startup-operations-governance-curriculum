# Exercise 03 — Structured interview scorecard and panel authoring

> Estimated time: **~5 hours** · Related chapter: [03 — Structured interviewing: panels, scorecards, and anti-affinity-bias operating norms](../03-structured-interviewing.md)

## Problem statement

You are the Head of Talent (or founder-CEO acting as head of talent) at Ferris Analytics, a Series-A data-tooling startup. You have three concurrent hires to stand up interview kits for, and the corporation has never run a structured hiring loop before. The current pattern is that the founder-CEO or the hiring manager does a first call, brings the candidate to the office for "a day," has 3–4 informal conversations, and then decides over drinks that evening.

The three open roles are deliberately picked to stress different parts of the structured-interviewing playbook:

1. **Senior Backend Engineer.** Reports to the Head of Engineering. Owns critical-path platform work in Go and Postgres. Ferris has 6 engineers today; this hire is number 7. Function-competency-heavy, moderate-cross-functional.
2. **First Product Manager.** Reports to the founder-CEO. Owns product prioritisation, PRDs, cross-functional planning, and go-to-market coordination for the flagship product. The corporation has no PM today — this is a first-of-role hire.
3. **Enterprise Account Executive.** Reports to the (newly hired) VP Sales. Ferris's second AE. Owns a defined territory of Fortune 500 accounts. Cross-functional-heavy (must partner with SEs, CSMs, product, and finance), close-focused.

The corporation's stated values are (a) *bias to ownership*, (b) *rigor with humility*, and (c) *build-in-the-open*.

Two operating constraints:
- Ferris has employees and interviews candidates in California, New York, Washington, and Colorado (all salary-history-ban jurisdictions; all pay-transparency jurisdictions).
- Two of the corporation's current 22 employees have publicly disclosed disabilities requiring accommodations; every interview loop must have an accommodation-request pathway.

Produce the interview kits, the panel designs, the interviewer-training plan, and the debrief-and-consensus playbook.

## Requirements

### Part A — Job scorecards (all three roles)

For each of the three roles, produce a full scorecard following the chapter's template. Each scorecard must include:

1. **Role summary** — one paragraph on what the role is and what it must accomplish in year one. Include the "outcomes at 90 / 180 / 365 days" variant.
2. **Core competencies** — 4 to 7 competencies. For each competency:
   - The **name** (a competency-level phrase, not a skill).
   - A **definition** (2–4 sentences on what "meets the bar" looks like for this role).
   - The **rating scale** — the four-point Strong No / No / Yes / Strong Yes scale.
   - The **evidence** the interviewer will rely on (behavioural example, work-sample output, response to case).
   - The **interviewer(s) assigned** to evaluate this competency (fill in after Part B).
3. **Values competencies** — 1–3 competencies operationalising Ferris's stated values (*bias to ownership*, *rigor with humility*, *build-in-the-open*) as observable behaviours. These are *not* "did the interviewer like them"; they are "did the candidate provide a specific behavioural example demonstrating the value?"
4. **Bar for hire** — the overall standard the candidate must meet to receive an offer. Pick a defensible pattern ("every core competency at Yes+, no Strong No on any competency" or a role-tuned variant). Justify.
5. **Explicit non-competencies** — the things this scorecard is *not* evaluating (e.g., "we are not evaluating culture fit as a standalone axis; we are evaluating specific values behaviours" or "we are not evaluating whether the candidate is like us; we are evaluating whether the candidate demonstrates the competencies").

### Part B — Interview panel design (all three roles)

For each of the three roles, produce the panel design. Each panel must include:

1. **Panel members** — 4 to 6 interviewers (executive loops go longer — see [chapter 08](../08-executive-hiring-playbook.md), but these are IC / senior-IC roles). For each panelist:
   - Their **role at Ferris** (title and function).
   - Which **scorecard competencies** they own.
   - The **interview type** they run (function-competency, values, cross-functional, case / work-sample, hiring manager, skip-level).
   - The **duration** of the interview slot.
2. **Panel diversity** — explicitly address gender, race, tenure, function, seniority, and geography. Where the diversity dimension cannot be met from the current 22-person team, name the constraint honestly and propose a mitigation (e.g., a rotating outside-advisor slot for the values interview to prevent the panel from being founder-heavy).
3. **Case interview / work-sample** — for each role, design the specific case interview. Include:
   - The **prompt** the candidate receives.
   - The **format** (take-home + live discussion; live exercise; written memo).
   - The **timing** (how far in advance the candidate receives the prompt; the duration of the live discussion).
   - The **rubric** the panel scores against (be specific — this is the highest-signal interview and the loosest rubric is where the panel drifts).
4. **Interviewer-slot ownership map** — who owns which slot on which candidate's on-site, load-balancing rules (no interviewer runs more than two slots per candidate; the founder-CEO does not run all three cases per candidate; every candidate gets at least one interviewer they have not spoken to in an earlier stage).

### Part C — Interviewer-training programme

Author the interviewer-training programme Ferris will run before its first structured on-site. Cover:

1. **Baseline training curriculum** — the 60–90-minute session all new interviewers complete before they are eligible to run interviews. Outline the specific modules (interview philosophy, scorecard and rating rubric, structured-question technique, anti-affinity-bias norms, legal do's-and-don'ts including salary-history-ban compliance and ADA-accommodation handling). Reference [mod-103 chapter 07](../../mod-103-employment-law-and-contract-design/07-eeoc-protected-category-framework.md) for the legal grounding.
2. **Shadowing and reverse-shadowing** — the specific number of interviews for each direction and the feedback rubric.
3. **Certification** — the specific interview types the corporation certifies interviewers on (technical function, values, cross-functional, case), the certification-tracking mechanism (in the ATS from exercise 02), and the recertification cadence.
4. **Interviewer-bar monitoring** — the ongoing operating norm for identifying "easy" and "impossible" interviewers, the debrief-facilitation coaching pattern for calibration drift, and what the corporation does with an interviewer whose calibration cannot be brought into range.
5. **The salary-history-ban script** — a specific interviewer script for the "what were you making at your last job?" moment that complies with California, New York, Washington, and Colorado law. See [mod-103 chapter 03](../../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md).
6. **The ADA-accommodation intake script** — the specific process for a candidate requesting an accommodation (extended time on a take-home, a different format for the live coding exercise, an interpreter). Who routes the request, who fulfils it, and how the panel is instructed not to adjust evaluation based on the accommodation.

### Part D — Debrief-and-consensus playbook

Author the debrief-and-consensus playbook. Cover:

1. **The pre-debrief scorecard-submission gate** — how the ATS is configured to hide scorecards from an interviewer until they have submitted their own; how the debrief facilitator verifies compliance before starting.
2. **Debrief order** — the "junior speaks first, senior speaks last" rule, and specifically who is "junior" and "senior" on each of the three panels.
3. **The evidence-not-vibes norm** — the specific facilitator script for the moment an interviewer says "I liked them" instead of citing evidence.
4. **The disagreement norm** — how disagreement is welcomed and structured; the specific facilitator move when two interviewers strongly disagree.
5. **The decision framework** — how the pre-defined "bar for hire" is applied; the tie-breaking rule; the "Strong No on a core competency" veto rule.
6. **The written decision record** — the template the facilitator uses to write up the debrief in the ATS. Include a sample writeup for a hypothetical candidate on one of the three roles.

### Part E — Anti-affinity-bias operating norms

Produce the corporation-wide operating-norms memo covering:

1. **Blind resume screens** — where Ferris will deploy blind screening (IC / manager screens) and where it will not (senior IC and above where full context is required). The specific redaction pattern (name, university, personal identifiers) and the ATS support required.
2. **Structured questions** — the corporation's policy that every interviewer for a given interview slot asks the *same baseline questions* of every candidate. Include a specific example baseline-question set for the Senior Backend Engineer's function-competency interview.
3. **Competency-anchored scoring** — the corporation's policy that every score is against a specific competency, never a global impression. The facilitator's script for a scorecard that says only "Yes."
4. **Interview-question review** — the periodic (quarterly? semiannual?) review of every scorecard for questions that (a) do not map to a listed competency, (b) invite protected-category inference, or (c) advantage a candidate profile the corporation has already over-hired.
5. **Recording and transcription consent** — if Ferris deploys Metaview / BrightHire / Pillar interview-intelligence tools, the two-party-consent flow for California, Washington, and other applicable states (see [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/) — flag the cross-module handoff). If Ferris is not deploying interview-intelligence yet, say so and describe the trigger that would prompt reconsideration.

## Starter guidance

- Chapter 03 is the primary reference. The four-artifact framing (scorecard, panel, training, debrief) is the design skeleton.
- The chapter's worked example (Series-A "first PM" hire) is a direct analogue for one of the three roles. Do not just copy it — Ferris has three roles with different characteristics.
- The Senior Backend Engineer competencies should differ meaningfully from the PM competencies. If your scorecards look identical across roles, you have not designed for the role.
- Values scorecard items are hard to write well. "Did the candidate demonstrate bias to ownership?" is not a scoring question; "Describe a time you owned a problem end-to-end that no one else was asking you to own — what did you do?" produces evidence. Design the values interview against evidence, not vibe.
- For the Enterprise AE, the case / work-sample interview is likely a role-play (discovery call, close conversation). Design the rubric carefully — a bad AE role-play interview scores charisma; a good one scores discovery discipline and objection-handling.
- Do not manufacture accommodation examples. The problem statement names two employees with disclosed disabilities; the point is that the intake script is required, not that you fabricate specific accommodations for specific hypothetical candidates.
- The salary-history-ban jurisdictions matter. In California, New York, Washington, and Colorado, asking prior compensation is prohibited; the interviewer script has to work under all four states' rules (which are similar but not identical).
- Do not confuse the *scorecard* (a rubric) with the *interview kit* (the questions each interviewer asks). Chapter 03 uses "interview kit" loosely to mean the combined scorecard + panel design + interview questions; a well-organised set of artifacts separates them.

## Deliverables

- `scorecards/scorecard-senior-backend-engineer.md`
- `scorecards/scorecard-first-product-manager.md`
- `scorecards/scorecard-enterprise-account-executive.md`
- `panels/panel-senior-backend-engineer.md`
- `panels/panel-first-product-manager.md`
- `panels/panel-enterprise-account-executive.md`
- `interviewer-training-programme.md` — Part C.
- `debrief-and-consensus-playbook.md` — Part D.
- `anti-affinity-bias-operating-norms.md` — Part E.

## Acceptance criteria

The package is acceptable if:

1. Each scorecard has 4–7 core competencies plus 1–3 values competencies, each with a name, definition, rating scale, and evidence description.
2. The three scorecards are *meaningfully different* across roles — the Senior Backend Engineer's competencies are not a re-skin of the PM's.
3. Each panel has 4–6 interviewers, with each competency owned by at least one panelist, and every panelist owns at least one competency.
4. Each panel design engages with panel diversity honestly — either the diversity is met or the constraint is named with a mitigation.
5. Each case / work-sample interview has a prompt, a format, a timing, and a specific rubric.
6. The interviewer-training programme covers baseline curriculum, shadowing / reverse-shadowing, certification, interviewer-bar monitoring, and the two specific scripts (salary-history-ban, ADA-accommodation).
7. The debrief playbook explicitly requires scorecard submission before scorecard visibility, junior-speaks-first ordering, evidence-not-vibes facilitation, and a written decision record.
8. The anti-affinity-bias memo names a specific blind-screening policy and identifies at least one baseline-question set for a specific interview slot.
9. The salary-history-ban script complies with all four applicable jurisdictions (California, New York, Washington, Colorado). It does not just say "don't ask."
10. Interview-intelligence deployment (if included) has an explicit two-party-consent flow; if not deployed, the trigger to reconsider is named.
11. Every reference to a legal requirement (Title VII, ADA, state salary-history bans, state pay-transparency, two-party-consent recording) is either cited to the relevant chapter of mod-103 / mod-104 / mod-110 or is flagged with a `<!-- needs-research -->` marker.
