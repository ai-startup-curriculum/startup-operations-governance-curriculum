# Exercise 06 — First-90-day onboarding programme authoring

> Estimated time: **~4 hours** · Related chapter: [06 — The first-day / first-week / first-90-day onboarding programme](../06-first-90-day-onboarding.md)

## Problem statement

Marlowe Software is a Series-A B2B SaaS company, 41 employees, growing to 90 in the next 15 months. Marlowe runs on Rippling (HRIS), Ashby (ATS), Okta (identity), and Kandji (MDM). The corporation has employees in California, New York, Washington, Colorado, Illinois, and Georgia.

Onboarding today is inconsistent. Some new hires get a warm pre-boarding packet from their hiring manager; others show up on day one with no laptop, no SSO account, no first-week agenda, and no manager 1:1 scheduled. The Head of People (you) has just been given a 6-month mandate from the CEO to stand up a designed onboarding programme.

The trigger event: new-hire NPS (piloted quarterly by an outside consultant) came back at a 21 for the most recent cohort — a number the CEO reads as "we're failing our new hires." Two of the most recent five hires have already given notice inside their 60-day mark, both citing "broken onboarding" in exit conversations. The 6-hire engineering cohort scheduled to start in the next 90 days is the immediate stress test.

The corporation also has three specific complications:

1. **A fully remote engineering hire in Atlanta.** No local office, no local peer for in-person buddying, no local IT for on-site provisioning. Section 2 of the I-9 will be completed via authorised representative (Rippling's network).
2. **A first executive hire — VP Sales — starting in 45 days.** Exec onboarding has its own overlay (see [chapter 08](../08-executive-hiring-playbook.md)); Marlowe wants the first-90-day programme to be *coherent with* the exec onboarding programme, not a separate track.
3. **Mandatory sexual-harassment-prevention training** required in California (SB 1343), New York State and NYC (annual for employees), Connecticut, Illinois, Delaware, and Maine. Marlowe has no current LMS deployment; training completion is not currently tracked.

Produce (a) a pre-boarding programme, (b) a day-one / first-week programme, (c) a 30 / 60 / 90-day check-in cadence, (d) a new-hire NPS instrument, and (e) a specific 90-day programme for the 6-hire engineering cohort.

## Requirements

### Part A — Pre-boarding programme (offer acceptance → day 0)

Author the pre-boarding programme. Cover:

1. **Immediate acknowledgment** — the personalised welcome the recruiter or hiring manager sends within one business day of offer acceptance. Include the specific script (2–3 sentences, personalised, named point of contact).
2. **The pre-boarding packet** — a specific list of what the packet contains, when it is sent (target: 1 week before start date), and the delivery mechanism (Rippling onboarding module; email; both). Include:
   - Start-date confirmation and start-day logistics.
   - Countersigned employment documents (PIIA, at-will acknowledgment, arbitration agreement if applicable, handbook acknowledgment).
   - Form I-9 Section 1 request via Rippling.
   - Benefits summary and enrollment-window explanation.
   - First-week draft agenda.
   - Buddy assignment (with buddy's name and note that the buddy will reach out).
   - Manager 1:1 pre-scheduled.
   - "What to bring on day one" checklist (I-9 documents, direct-deposit banking info).
3. **Pre-start touchpoints** — the specific 1–4 week cadence between offer acceptance and start. The hiring manager's message. The buddy's message. Any team-all-hands invitation.
4. **The provisioning checklist** — the concrete IT / HR / manager tasks that must be complete *before* day one. Include target completion dates relative to start date:
   - Laptop shipped by IT via Kandji (target: arrives 2 days before start).
   - SSO account created in Okta (target: 3 business days before start).
   - SaaS tool access provisioned via SCIM (target: 2 business days before start).
   - Email address live and directory listed (target: 2 business days before start).
   - Building badge (in-office hires) / desk assigned (target: 1 business day before start).
   - Direct-deposit + W-4 collected (target: 1 week before start).
5. **The pre-boarding-checklist owner** — the head of people's discipline for making sure every item is complete before day one, and the escalation if an item is at risk.

### Part B — Day-one and first-week programme

1. **Day-one agenda** — a specific hour-by-hour schedule. Adapt the chapter's canonical template for Marlowe's specific stack. Include (at minimum):
   - Welcome and orientation with head of people.
   - Form I-9 Section 2 (in-person if in-office; authorised-representative or DHS alternative procedure if remote — see [chapter 05](../05-i9-and-e-verify.md)).
   - Employment-document countersign.
   - Benefits-enrollment kickoff.
   - 1:1 with manager.
   - Buddy introduction.
   - Team introductions.
   - Setup verification with IT.
2. **The buddy programme** — the buddy-role design: peer level, not on the reporting line, some domain overlap, trained on the buddy role. Include the specific expectations (weekly touchpoint for first 4 weeks; monthly through 90 days), the boundaries (buddy is a resource, not a mentor or coach), and the escalation paths (buddy raises concerns about broken onboarding to head of people).
3. **The first-week programme** — the specific first-week schedule beyond day one:
   - Manager 1:1 (weekly cadence established).
   - First-week standing team meetings the new hire attends.
   - Onboarding-curriculum access (self-serve modules via Rippling's onboarding tool or an LMS — recommend which).
   - Cross-functional intros (3–5 × 30 minutes, scheduled *by the manager*, not the new hire).
   - Mandatory training (security, sexual-harassment prevention — Marlowe's California / NY / CT / IL / DE / ME footprint requires it — plus role-specific compliance).
   - First deliverable assigned by end of week one.
4. **The remote-hire variant** — the specific adjustments for the Atlanta engineering hire: authorised-representative I-9 workflow, video-call buddy introduction, extra care on team introductions (all-team video intro with structured Q&A), enhanced week-one 1:1 cadence with the manager (daily 15-minute check-ins in the first week to reduce isolation).

### Part C — 30 / 60 / 90-day check-in cadence

Author the check-in cadence and templates:

1. **30-day check-in** — with manager (structured conversation on what is working / not / blockers / role expectation); with head of people (onboarding-experience check); with a deliverable check.
2. **60-day check-in** — with manager (deeper role-fit); cross-functional feedback from 2–3 peers; benefits-enrollment-window-closed follow-up.
3. **90-day check-in** — with manager (formal 90-day review); with head of people (retention check); documented outcome in the HRIS.
4. **Templates** — provide the specific question prompts each check-in uses. These should be reusable across hires, not custom per person.
5. **Escalation** — the specific process when a 30 / 60 / 90 check-in surfaces a broken onboarding signal (missed deliverable, disengagement, misaligned role expectation). Who is notified; what happens next; the "how do we save this hire" conversation.

### Part D — New-hire NPS instrument

Author the new-hire NPS instrument. Cover:

1. **Survey cadence** — day 14, day 30, day 60, day 90 (following the chapter's template).
2. **Survey content** — 5–10 questions per checkpoint. Mix of Likert-scale (1–5 or 1–10) and free-text. Include:
   - Day 14: pre-boarding and day-one experience.
   - Day 30: onboarding curriculum, manager relationship, buddy relationship.
   - Day 60: team integration, expectations from interview loop.
   - Day 90: overall experience, "how likely to recommend Marlowe as a place to work" NPS score, free-text on what to change.
3. **Delivery mechanism** — Rippling's engagement-survey module or a dedicated tool (Culture Amp, Lattice, 15Five, Officevibe). Recommend one and justify.
4. **Anonymity** — whether the survey is anonymous, semi-anonymous, or attributable, and the trade-offs (small cohorts can be deanonymised even from Likert scores; free-text can accidentally identify).
5. **Review cadence** — how frequently the head of people reviews trends (monthly baseline; ad-hoc on a dip); who else sees the results (CEO monthly; executive team quarterly).
6. **The "act on it" discipline** — the specific mechanism by which surfaced themes are converted into fixes. A running "onboarding improvement backlog" the head of people owns.

### Part E — 90-day programme for the 6-hire engineering cohort

Apply the entire programme to a specific cohort — the 6 engineers starting in the next 90 days (assume they start on the same date, or in three overlapping start-date waves 2 weeks apart). Cover:

1. **Cohort pre-boarding** — the packet, the pre-start touchpoints (including a cross-cohort "welcome to Marlowe" video call in the week before start), the provisioning-checklist status tracking.
2. **Cohort day-one** — a *cohort orientation session* (60–90 minutes) that batches the head-of-people welcome across all cohort hires, followed by individual manager 1:1s and team introductions.
3. **Cohort first-week** — the shared onboarding-curriculum modules; a cohort-cross-team lunch or virtual social; individual manager cadence.
4. **Cohort 30 / 60 / 90** — individual check-ins per the Part C templates; a cohort-level retrospective at the 60-day mark to surface shared themes.
5. **The VP Sales handoff** — how the VP Sales's exec-onboarding overlay (see [chapter 08](../08-executive-hiring-playbook.md)) sits *on top of* this 90-day programme without duplicating or contradicting. The VP Sales still gets the pre-boarding packet, the day-one orientation, the 30 / 60 / 90 check-ins — plus the 100-day plan, the board-relationship-establishment cadence, and the CEO-partnership norms from the exec playbook.

## Starter guidance

- Chapter 06 is the primary reference. The pre-boarding / day-one / first-week / 30-60-90 / new-hire-NPS framing is the design skeleton.
- Do not invent onboarding statistics. Where you cite "the majority of new-hire attrition happens in the first year" or similar folk claims, either cite the chapter's `<!-- needs-research -->` marker and refresh with a defensible source (SHRM, Gartner, LinkedIn Talent, Brandon Hall Group) or omit.
- The Rippling / Ashby / Okta / Kandji stack is the corporation's substrate. Design against those tools' actual capabilities. If a design requires a tool Marlowe does not have (an LMS, a dedicated engagement-survey product), recommend the acquisition explicitly with a cost note.
- The remote-hire variant (Atlanta) is deliberately included to force you to design for isolation. The chapter's authorised-representative workflow and the buddy programme both matter more for remote hires.
- The mandatory sexual-harassment-prevention training landscape shifts. Marlowe's California / NY / CT / IL / DE / ME footprint currently mandates it; other states and cities have added mandates in recent legislative sessions. Verify the current landscape as a `<!-- needs-research -->` item.
- The VP Sales overlay is the point where the 90-day programme meets the exec-onboarding programme. Do not duplicate the exec playbook; layer it.
- The new-hire NPS "act on it" discipline is the single largest failure mode of any survey programme. Design for the action, not just the survey.
- The 30 / 60 / 90 templates should be reusable. If your templates are personalised to a specific hypothetical hire, you have not designed for reuse.

## Deliverables

- `pre-boarding-programme.md` — Part A.
- `day-one-and-first-week-programme.md` — Part B.
- `30-60-90-check-in-cadence-and-templates.md` — Part C.
- `new-hire-nps-instrument.md` — Part D.
- `engineering-cohort-90-day-programme.md` — Part E.
- `provisioning-checklist.md` (or `.csv`) — the concrete list of every pre-boarding provisioning task with owner, target date, and status.

## Acceptance criteria

The package is acceptable if:

1. The pre-boarding programme (Part A) has an immediate-acknowledgment script, a specific packet contents list, defined pre-start touchpoints, a provisioning checklist with target dates relative to start, and a named owner for pre-boarding-checklist completion.
2. The provisioning checklist has target dates *before* day one for laptop, SSO, SaaS access, email, and direct-deposit / W-4 collection.
3. The day-one agenda is hour-by-hour and includes I-9 Section 2, employment-document countersign, benefits-enrollment kickoff, manager 1:1, buddy introduction, team introductions, and setup verification.
4. The buddy programme has explicit peer-level / not-in-reporting-line / trained / weekly-touchpoint / escalation-path design.
5. The remote-hire variant explicitly addresses I-9 Section 2 via authorised representative and the specific adjustments (video-call buddy, all-team video intro, daily first-week check-ins).
6. The 30 / 60 / 90-day templates are reusable and include specific question prompts.
7. The escalation for a broken-onboarding signal is specific — who is notified, what happens next.
8. The new-hire NPS instrument has cadence, content per checkpoint, delivery mechanism, anonymity posture, review cadence, and an act-on-it discipline.
9. The engineering-cohort programme includes a cohort orientation session, shared onboarding-curriculum modules, a cohort retrospective at the 60-day mark, and the individual VP-Sales exec-onboarding overlay.
10. Mandatory sexual-harassment-prevention training is covered for California, New York, and the other applicable jurisdictions, with completion tracked in Rippling (or a recommended LMS).
11. Every folk claim about onboarding statistics is either cited to the chapter's `<!-- needs-research -->` marker with a defensible source or omitted.
12. Nothing left as `[TBD]` or `[FILL IN]`.
