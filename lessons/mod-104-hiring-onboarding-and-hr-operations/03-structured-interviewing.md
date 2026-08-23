# 3. Structured interviewing: panels, scorecards, and anti-affinity-bias operating norms

> An unstructured interview is a series of nice conversations that produces a "gut" recommendation. A structured interview is a repeatable evaluation the corporation can defend, calibrate, and improve.

## Motivation

Unstructured hiring feels efficient. The founder or hiring manager sits down with a candidate, has a good talk, forms a view, and either extends or declines. It is fast and low-friction. It also has three well-documented failure modes:

1. **Low predictive validity.** Meta-analytic research in industrial-organisational psychology has for decades found unstructured interviews to be *substantially less predictive of job performance* than structured interviews with the same interviewer time budget. <!-- needs-research: cite the Schmidt & Hunter meta-analyses (1998 original and 2016 update) on the predictive validity of hiring methods; note that the 2016 update has been re-examined and some effect sizes revised — check the current-canonical citation before quoting a validity coefficient. -->
2. **Affinity bias.** Absent structure, interviewers systematically favour candidates who resemble themselves — same school, same accent, same demographic, same conversational style. This is not a moral failing of any single interviewer; it is a robust feature of human evaluation under ambiguity. It also produces disparate-impact exposure under Title VII, the ADA, the ADEA, and analogous state statutes (see [mod-103 chapter 07](../mod-103-employment-law-and-contract-design/07-eeoc-protected-category-framework.md)).
3. **No calibration or improvement.** Without structured scorecards, the corporation cannot look back at a decision and ask "was this call right?" — because there is no record of what the call actually said. Hiring quality cannot compound.

Structured interviewing solves for all three at once: it improves predictive validity, it suppresses affinity bias by anchoring evaluation to job-relevant criteria, and it produces an auditable record that can be reviewed and improved.

This chapter builds the four artifacts every hiring loop needs — the **job scorecard**, the **interview-panel design**, the **interviewer-training programme**, and the **debrief-and-consensus playbook** — and layers on the operating norms that suppress affinity bias.

## Artifact 1 — The job scorecard

The job scorecard is a written document that names, for a specific role, the competencies against which every candidate for the role will be evaluated. It exists *before* the first candidate is interviewed and is the same for every candidate.

A typical scorecard structure:

- **Role summary** — one paragraph on what the role is and what it must accomplish in year one. (This is where the "outcomes" version of a scorecard adds "what does success look like at 90 / 180 / 365 days?" — a common variant popularised by the *Who* framework and adopted widely in startup hiring.)
- **Core competencies** — 4 to 7 competencies the role requires. Each competency has:
  - A **name** (e.g., "Ability to scope and execute a technical project independently").
  - A **definition** (2–4 sentences on what "meets the bar" looks like for this role).
  - A **rating scale** (typically a 4-point scale — "Strong No / No / Yes / Strong Yes" — deliberately even to force a decision rather than allow neutral middle scores).
  - The **evidence** the interviewer will rely on (behavioural examples, work-sample output, response to a specific case).
- **Assignment to interviewers.** Each competency is owned by one or two interviewers in the panel; every interviewer knows in advance which competencies they are evaluating.
- **Bar for hire.** The overall standard the candidate must meet to receive an offer. Common patterns: "Every core competency at Yes or Strong Yes, no Strong No on any competency" or "≥ N/M competencies at Yes+ and no Strong No."

The scorecard is the shared vocabulary the entire hiring loop speaks. Without it, "we like them" is the only vocabulary available.

### Competency vs. skill vs. trait

A competency is *what the person can do in the context of this role*. It is broader than a skill (a discrete capability, e.g., "can write Python") and narrower than a trait (a stable personality attribute, e.g., "curious"). Scorecards should be written at the competency level. "Writes clean, well-tested Python" is a skill; "Can independently take a fuzzy technical problem, decompose it into a plan, and ship a working solution" is a competency. Interview evidence for the latter is much richer than for the former.

### Values as scorecard items

Most startups add 1–3 "values" competencies to the scorecard — the corporation's specific values operationalised as observable behaviours. "Values" here is not "we like them," it is *"in a specific behavioural example the candidate described, did they demonstrate the corporation's stated values?"* This is designed by the hiring team, with the head of people or the CEO involved in the definition, and evaluated by a specific "values interviewer" on the panel (see below).

## Artifact 2 — The interview-panel design

Every role has a **panel** — the specific interviewers who will meet the candidate at the on-site loop. The panel is not thrown together the day before the on-site; it is designed against the scorecard.

A canonical Series-A / Series-B on-site loop has four to six interviews covering the following slots:

1. **Function-competency interview(s)** — one or two interviews that assess the candidate's core technical / functional capability against the scorecard's function-competencies. For an engineer, this is usually a technical coding or systems-design interview. For a PM, a product-thinking case. For an AE, a discovery-and-close role-play. Owned by a senior IC or manager in the function.
2. **Values interview** — one interview that assesses the values competencies. Owned by an interviewer specifically trained on the values rubric, ideally someone *outside* the hiring team to avoid reinforcement bias.
3. **Cross-functional interview** — one interview from a peer function the candidate will work closely with (e.g., an engineer interviewing a PM candidate, a designer interviewing an engineer candidate). Assesses partner-readiness and cross-functional collaboration.
4. **Case / work-sample interview** — a role-relevant simulated exercise (a take-home coding project with a live discussion; a live product-strategy exercise; a written strategy memo followed by discussion). Work-sample interviews are among the highest-predictive-validity signals in the I/O literature. <!-- needs-research: confirm the validity coefficient for work-sample tests from the Schmidt & Hunter meta-analyses and the more recent Sackett et al. re-analysis; work samples are consistently near the top of the validity hierarchy but the specific coefficient has been re-estimated. -->
5. **Manager interview** — the direct hiring manager, if not already covered above.
6. **"Skip level" / executive interview** — for senior IC / manager / director hires, the manager's manager (and, at earlier stages, often the founder-CEO) meets the candidate. This is a bar-setting conversation, not a competency-evaluation conversation, though scorecard input is still captured.

**Panel size.** Four to six interviews is the durable range. More than six causes candidate fatigue and diminishing marginal information; fewer than four produces gaps in the scorecard evidence. Executive loops (see [chapter 08](./08-executive-hiring-playbook.md)) go longer.

**Panel diversity.** The panel should be diverse across the dimensions relevant to the corporation's hiring goals and to the reduction of affinity bias — gender, race, tenure, function, seniority, and geography. Homogeneous panels systematically produce homogeneous hires. Panel diversity is designed at the level of the *panel-composition policy*, not at the level of a specific candidate ("we need a woman on this panel because the candidate is a woman" is both a bad policy and an affinity-bias pattern in reverse).

## Artifact 3 — The interviewer-training programme

An interviewer who has never been trained will interview badly by default — asking hypothetical brain-teasers, evaluating on surface impression, forgetting to submit a scorecard, sharing their view in the debrief before others have shared theirs (see below).

A working interviewer-training programme has three phases:

1. **Baseline training.** All new interviewers complete a 60–90-minute training before they are eligible to run interviews. Content: the corporation's interview philosophy, the scorecard and rating rubric, structured-question technique (STAR / behavioural anchor / probe pattern), the anti-affinity-bias norms (see below), the legal do's-and-don'ts (Title VII protected categories, ADA-compliant question phrasing, salary-history-ban compliance — see [mod-103](../mod-103-employment-law-and-contract-design/)).
2. **Shadowing and reverse-shadowing.** The new interviewer shadows an experienced interviewer on 2–3 interviews. Then the experienced interviewer reverse-shadows the new interviewer on 2–3 interviews, providing feedback on question quality, probing, note-taking, and scorecard submission.
3. **Certification and ongoing calibration.** The new interviewer is certified for a specific interview type (e.g., "certified to run the technical function interview" or "certified to run the values interview"). Certification is tracked in the ATS or a training tool. Ongoing calibration happens through periodic re-training and through debrief facilitation (a lead interviewer coaches interviewers whose scores are consistently off-panel).

At scale, the corporation should measure **interviewer bar** — the score distribution each interviewer produces — and identify outliers (an interviewer who scores everyone Yes / Strong Yes may be an "easy" interviewer; one who scores everyone No / Strong No may be an "impossible" interviewer). Both are calibration targets, not termination targets; both bias the panel unless surfaced.

## Artifact 4 — The debrief-and-consensus playbook

The debrief is where the panel converts individual scorecards into a decision. Done well, it improves the quality of the decision. Done badly, it collapses the panel into whoever spoke first or loudest.

The rules of a good debrief:

1. **Scorecards submitted before the debrief starts.** The ATS should refuse to display any interviewer's scorecard until that interviewer has submitted their own. This prevents the "wait to see what everyone else thought" pattern that is the largest single source of debrief noise.
2. **Junior speaks first.** In the debrief itself, the most junior interviewer speaks first, the most senior speaks last (or after everyone else). This prevents the "the CEO said yes so everyone says yes" collapse.
3. **Evidence, not vibes.** Every interviewer states their rating on each competency they assessed and reads the specific behavioural evidence that supported it. "I liked them" is not evidence. "They walked through a project where they identified a scoping ambiguity, escalated it to their PM, and re-scoped in a day" is evidence.
4. **Disagreement is welcomed.** A debrief where every interviewer says Yes is not necessarily a good debrief — it may be a homogenous-panel debrief. A debrief where two interviewers disagree strongly is often the highest-signal debrief; the disagreement forces a re-examination of the evidence.
5. **Explicit decision framework.** The panel applies the pre-defined "bar for hire" (see scorecard). Where the panel is split, the hiring manager owns the decision, unless the split includes a "Strong No" on a core competency, in which case the default is not to extend an offer.
6. **Written decision record.** Whoever facilitates the debrief writes a short (few-paragraph) decision note stored in the ATS against the candidate: what the panel concluded on each competency, the decision, and the reasoning. This is what a future diligence request or an EEOC / OFCCP inquiry reads.

## Anti-affinity-bias operating norms

The scorecard, the panel design, the training, and the debrief already suppress affinity bias substantially. Three further operating norms add margin:

### Norm 1 — Blind resume screens

Where feasible, the initial resume review is conducted with candidate name, university, and personal identifying details redacted. What is visible: role history, achievements, and skills. This is easier than it sounds — most ATS platforms support "blind screening" modes; the recruiter or a designated screener redacts identifiers before passing the resume to the hiring team. Blind screens are most useful at the top of the funnel where interviewer time is shortest and the "gut" pattern is strongest.

Blind screening is not universal — some senior / exec searches require full context — but for IC and manager screens it is a low-cost, high-margin practice.

### Norm 2 — Structured questions

Every interviewer for a given interview slot asks the *same questions* of every candidate. The candidate's answers are noted against the pre-defined scorecard rubric. This does not mean the interview is a script — the interviewer probes deeper as needed — but the *baseline* questions are common. This is what makes candidates comparable to each other.

The alternative — "I ask whatever comes to mind" — is what makes the comparison "did I like Candidate A more than Candidate B?" instead of "how did Candidate A perform against the rubric relative to Candidate B?"

Standard structured-question anchors: behavioural (STAR — Situation, Task, Action, Result), case (a role-relevant scenario with a right-order-of-thinking rubric), and work-sample (do the work, evaluate the output).

### Norm 3 — Competency-anchored scoring

Every score is against a *specific competency*, not a global impression. "I'd hire" is not a score. "Ability to scope and execute a technical project independently: Yes — evidence: X" is a score. The scorecard forces the interviewer to make the evaluation at the competency level; the debrief keeps it there.

### Additional practices worth adopting

- **Interview-question review.** The scorecard and interview kit for every role is reviewed periodically for questions that (a) do not map to a listed competency, (b) invite protected-category inference (marital status, family plans, national origin, religion, disability), or (c) advantage a candidate profile the corporation has already over-hired. The head of people or an outside advisor can facilitate this review; [mod-103 chapter 07](../mod-103-employment-law-and-contract-design/07-eeoc-protected-category-framework.md) covers the protected-category framework in detail.
- **Salary-history-ban compliance.** In jurisdictions where asking a candidate about prior compensation is prohibited (California, New York, Colorado, Washington, and many others), interviewers must not ask. Recruiter training must include the salary-history-ban script for the corporation's hiring footprint. See [mod-103 chapter 03](../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md).
- **Accommodation requests.** Candidates with disabilities may request reasonable accommodations for the interview (extended time on a take-home, a different format for a live coding exercise, an interpreter). The corporation must have a documented process for handling these requests (typically routed through the recruiter or head of people), and interviewers must not adjust their evaluation criteria based on the accommodation.
- **Recording and transcription.** Interview-intelligence tools (Metaview, BrightHire, Pillar) that record and transcribe interviews require candidate consent, and in two-party-consent states (California and others — check applicable state law) they require *explicit* consent captured before the recording begins. Consent, storage, retention, and access controls sit at the intersection of [mod-110 (privacy)](../mod-110-privacy-data-governance-and-sector-compliance/) and the ATS integration decision (see [chapter 02](./02-ats-selection-and-integration.md)).

## A worked example — a Series-A "first PM" hire

The corporation is hiring its first product manager, reporting directly to the founder-CEO. The engineering-founder / CTO will co-interview. The corporation has one PM advisor.

**Scorecard (before any candidate is screened).**

Role summary: "First PM. Owns product prioritisation, PRDs, cross-functional planning, and go-to-market coordination for the corporation's flagship product. In year one, ships two major releases and stands up the product-strategy cadence."

Core competencies:
1. Product judgment — can synthesise customer, market, and technical signal into a defensible prioritisation.
2. Cross-functional leadership — can rally engineering, design, and GTM without formal authority.
3. Written communication — can produce a PRD that engineers and executives both trust.
4. Discovery discipline — can plan and run structured customer conversations.
5. Values: bias to ownership; low ego.

Bar for hire: every competency at Yes+, no Strong No, product-judgment competency at Yes+ from at least one of the technical interviewers.

**Panel.**
1. Founder-CEO — cross-functional leadership + values (owner of two competencies).
2. CTO — product judgment + written communication (co-owner with the advisor).
3. PM advisor — product judgment + discovery discipline + written communication.
4. Design lead (cross-functional) — cross-functional leadership.
5. GTM peer (an early customer-facing hire) — cross-functional leadership.

Case interview: a written PRD exercise (2 hours, take-home, provided at least 4 business days before the on-site) and a 60-minute live walk-through-and-discussion with the CTO and the PM advisor. This is the highest-signal single interview in the loop; the scorecard for it is the most detailed.

**Training.** Every panelist reviews the scorecard, the STAR question guide, and the values rubric in a 30-minute recruiter-led briefing before the first candidate on-site. The PM advisor calibrates the technical panelists (CTO + design lead + GTM peer) on the product-judgment rubric with two example answers (a Yes-caliber answer and a Strong No-caliber answer).

**Debrief.** Scorecards submitted first. Design lead (most junior) speaks first, founder-CEO speaks last. Each competency reviewed against the evidence. Decision recorded in the ATS.

## Summary

- Structured interviewing is *higher predictive validity, lower affinity bias, and auditable* — the opposite of "we had a nice chat and I like them."
- The four artifacts every hiring loop needs: the scorecard, the panel design, the interviewer-training programme, and the debrief-and-consensus playbook. Every one of them should exist before the first candidate is screened.
- The scorecard is the shared vocabulary. Every competency is defined, has a rating scale, and is owned by a specific interviewer.
- Anti-affinity-bias operating norms: blind resume screens where feasible, structured (shared) questions across candidates, competency-anchored scoring, salary-history-ban compliance, panel-composition policy for diversity.
- The debrief converts individual scorecards into a decision. Rules: submit scorecards first, junior speaks first, evidence not vibes, disagreement welcomed, explicit decision framework, written decision record.
- The interview kit is a *living* artifact — reviewed periodically for protected-category exposure, question quality, and calibration drift.
