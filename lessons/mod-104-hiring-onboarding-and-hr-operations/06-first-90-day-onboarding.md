# 6. The first-day / first-week / first-90-day onboarding programme

> Onboarding is not "the day one welcome email and a swag box." It is a designed programme that runs from offer acceptance through the 90-day anniversary — and it is where broken hiring shows up as early attrition.

## Motivation

The corporation spent weeks sourcing, screening, interviewing, and closing the new hire. It ran background checks, prepared the offer, and got the countersign. On paper the hire is complete. In practice, the corporation's investment produces value only if the new hire (a) starts productively, (b) integrates into the team, and (c) is still there in twelve months.

Broken onboarding is the failure mode where all three of those go wrong. The new hire arrives on day one to a laptop that has not been provisioned, an SSO account that does not work, no benefits enrollment window explanation, no first-day agenda, no manager 1:1 scheduled, and a buddy who did not know they were assigned. The new hire wastes their first two weeks debugging their own workstation. Their manager is busy on something else. The corporation wonders in month three why the new hire is disengaged and in month six why the new hire has already left.

The single most read finding in this area is that early attrition is disproportionately concentrated in the first year — and specifically in the first 90 days. <!-- needs-research: cite a defensible source for early-attrition statistics (SHRM, Gartner, LinkedIn Talent, Brandon Hall Group) rather than a folk figure. Common folk claims like "20% of new hires leave in the first 45 days" are widely cited but often trace back to marketing whitepapers rather than peer-reviewed sources. --> The mechanism is largely operational — the new hire's early impressions are formed against the daily friction of onboarding, and broken onboarding compounds.

This chapter builds the onboarding programme as a designed operating loop, covering (a) pre-boarding, (b) day one, (c) first week, (d) first 30 / 60 / 90-day check-in cadence, and (e) the new-hire-NPS instrument that closes the loop before broken onboarding becomes attrition.

## Pre-boarding (offer acceptance → day 0)

Pre-boarding is the window between offer acceptance and the first day. It is the highest-leverage window in the entire employee lifecycle — the new hire is most engaged, most excited, and most in-need-of-signal about whether the corporation is what they were told.

### Pre-boarding communications

- **Immediate acknowledgment.** Within one business day of offer acceptance, the recruiter (or the hiring manager) sends a personalised welcome — congratulations, a summary of what will happen next, and a named point of contact for questions. A generic system-triggered "your offer has been received" email is fine as an *addendum*; it is not sufficient as a welcome.
- **The pre-boarding packet.** Within one week of offer acceptance, the new hire receives a structured packet with:
  - Start date confirmation and start-day logistics (address, time, dress, parking, or the remote-day equivalent).
  - The offer letter and all countersigned employment documents (PIIA, at-will acknowledgment, arbitration agreement, handbook acknowledgment — see [mod-103](../mod-103-employment-law-and-contract-design/)).
  - The Form I-9 Section 1 request (see [chapter 05](./05-i9-and-e-verify.md)).
  - The benefits summary and the enrollment-window explanation.
  - A first-week draft agenda.
  - Buddy assignment (see below) with the buddy's name and a note that the buddy will reach out.
  - Manager 1:1 pre-scheduled for day one or day two.
  - A "here's what you'll need to bring on day one" checklist (I-9 documents, banking info for direct deposit).
- **The pre-start touchpoints.** In the 1–4 weeks between offer acceptance and start, the hiring manager and buddy each send at least one personal message — inviting the new hire to a team all-hands, sharing a reading list or a link to the current OKRs / roadmap, or just checking in. This is deliberately low-friction — the goal is to reduce the "starting somewhere I don't know anyone" feeling.

Pre-boarding is where a candidate who has multiple competing offers decides whether to actually show up.

### Provisioning — laptop, SSO, tools, access

The single most operational-visible failure of onboarding is a new hire who cannot log in on day one. Provisioning must be complete *before* day one:

- **Laptop.** Shipped to arrive at least 1–2 days before start date. Pre-imaged with the corporate MDM (JAMF, Kandji, Intune, or the corporation's chosen mobile-device-management product) and the corporate baseline software (browser, communication client, document suite, developer tools if applicable).
- **SSO account.** Created in the identity provider (Okta, Google Workspace, Microsoft Entra ID) 3–5 days before start date. Not on start date — that is too late for the identity provider's downstream provisioning to have propagated to all SaaS systems by day one.
- **SaaS tool access.** Every tool the new hire needs on day one is provisioned via SSO / SCIM before start date — Slack or Teams; the ATS if applicable; the HRIS employee-self-service portal; email; document repository; project-management tool; role-specific systems.
- **Email address and directory listing.** Live before start date. New hire's name shows in the directory. Manager and buddy have seen the new hire's entry in the directory before day one.
- **Physical access.** Building badge (if in-office) provisioned before start date. Desk (if in-office) assigned and known.
- **Payroll and banking.** HRIS direct-deposit information collected during pre-boarding. Tax withholding forms (Form W-4 federal, plus state equivalents) collected during pre-boarding.

The single most valuable operating discipline here is a **pre-boarding checklist** owned by the head of people (or, at scale, the People Operations function). Every item on the checklist has an owner (IT, HR, hiring manager, recruiter). Every item is complete before day one, or the day-one experience breaks.

## Day one

Day one is the new hire's first impression of the corporation *from inside*. It should feel deliberate, welcoming, and low-friction.

### The day-one agenda

A defensible day-one agenda includes:

1. **Welcome and orientation.** The head of people (or, at scale, the People Ops or HR team) meets the new hire in the first hour. Reviews the day-one paperwork, the first-week schedule, the org overview, the culture and values, the benefits summary, and how to get help.
2. **I-9 Section 2.** The employer completes Section 2 of Form I-9 — either in person on day one or scheduled with the authorised representative to be complete within three business days (see [chapter 05](./05-i9-and-e-verify.md)). Day one is the operational default when the new hire is in the office.
3. **Employment documents countersign.** Any documents not already countersigned (PIIA acknowledgment if not pre-signed, handbook acknowledgment, benefits enrollment) are completed. Handbook acknowledgment in particular is time-stamped on day one so the corporation has a clean record that the handbook was received.
4. **Benefits enrollment kickoff.** The benefits-enrollment window (typically 30 days from start date, often shorter for some plans) is explained. New hire is directed to the enrollment portal (HRIS or benefits-broker portal). Health, dental, vision, 401(k), commuter, FSA / HSA, life / disability, ESPP if applicable.
5. **1:1 with manager.** Scheduled for day one or day two. Manager confirms the first-90-day expectations (see below), the first-week priorities, and the working-relationship norms (how the manager wants to be reached, the manager's 1:1 cadence, how to raise issues).
6. **Buddy introduction.** The assigned buddy has a scheduled introduction — coffee, lunch, or the video-call equivalent for remote. The buddy is a peer, deliberately outside the new hire's reporting line, whose job is to be the "how does this actually work here?" resource for the first 90 days.
7. **Team introductions.** The new hire meets their direct team. If in-office, the manager walks the new hire around. If remote, an all-team introduction is scheduled.
8. **Setup verification.** IT walks the new hire through login and access verification. Any provisioning gaps caught on day one are unblocked before end of day.

The day-one agenda is *given to the new hire in writing before day one*. Surprise agendas are stressful; scheduled agendas are welcoming.

### The buddy programme

The buddy is a designed role. Common properties:

- Peer level (not manager, not skip-level).
- Not on the new hire's reporting line.
- Some domain overlap so the buddy can answer role-relevant questions ("how do we ship code?" "how do we run customer calls?" "how does our sales-review cadence work?").
- Trained on the buddy role — expectations (weekly touchpoint for first 4 weeks; monthly through 90 days), boundaries (buddy is a resource, not a mentor or a coach), and escalation paths (buddy raises concerns about broken onboarding to the head of people).

At scale, the buddy assignment is a rotation — no single peer is a buddy for every new hire; the load is distributed and the buddy pool is diverse.

## First week

Week one is the transition from "welcome to the corporation" to "here is your team and your work."

- **Manager 1:1.** Day one or day two, as above. Recurring weekly 1:1 scheduled.
- **First-week team meetings.** New hire attends the team's standing meetings — standup, all-hands, sprint planning, sales review, whatever the team runs. This is the fastest path to context.
- **Onboarding curriculum.** The corporation should have a defined new-hire onboarding curriculum — some combination of self-serve content (culture deck, product primer, org overview, key policies, security training) and live sessions (all-hands attendance, cross-functional 1:1s with adjacent-team leads). Common tools: an LMS (Learn.com, TalentLMS, or a lightweight home-grown wiki), the HRIS's onboarding module (Rippling, Gusto, and others have solid native onboarding curriculum tools), or a company-specific tool like Trainual or WorkRamp.
- **Cross-functional intros.** The new hire meets 1:1 (30 minutes each) with 3–5 cross-functional peers whose work intersects with theirs. Scheduled *by the manager* — not left to the new hire to arrange. This is one of the operational discipline items that most often gets skipped.
- **Mandatory training.** Security training, sexual-harassment-prevention training (California AB 1825 / SB 1343 for employers with 5+ employees; NY State and NY City mandate for employees; Connecticut, Illinois, Delaware, and Maine also mandate — check the corporation's hiring footprint against current law), and any role-specific compliance training. Training completion is recorded in the HRIS or LMS with a timestamped acknowledgment.
- **First deliverable.** By the end of week one, the manager has assigned a small, concrete first deliverable — something the new hire can start, meaningfully progress, and use as a talking point in their day-14 or day-30 check-in.

## The 30 / 60 / 90-day cadence

The first 90 days are the window in which the new hire either integrates into the team or begins to disengage. The 30 / 60 / 90-day check-in is the operating instrument the corporation uses to catch the drift.

### 30-day check-in

- **With the manager.** Structured conversation. What is working? What is not? Any blockers? Is the role what was described in the interview? Is the manager providing enough context and direction, or too much?
- **With the head of people (or People Ops).** Onboarding-experience check. Did pre-boarding work? Did day one work? Any early friction points to unblock?
- **Deliverable check.** The first-week concrete deliverable should be on track or complete. If it is not, the manager surfaces why.

### 60-day check-in

- **With the manager.** Deeper role-fit conversation. Now that the new hire has had two months, are they seeing what they expected? Are the corporation's values what they were pitched? Is there a stretch project the manager can offer?
- **Cross-functional feedback.** The manager solicits informal feedback from 2–3 cross-functional peers — how has the new hire shown up so far?
- **Compensation-and-benefits check.** The benefits-enrollment window (usually 30 days) has closed. Are there any questions or issues the new hire is still resolving?

### 90-day check-in

- **With the manager.** Formal 90-day review. What has the new hire accomplished? What does the manager see as the strongest and the growth areas? What is the expectation for the next quarter?
- **With the head of people.** Retention check. Is the new hire engaged? Any concerns about attrition risk?
- **Documented outcome.** The 90-day review is recorded in the HRIS (or the performance-management system, if separate). It is the anchor for the first formal performance conversation. See [mod-107](../mod-107-performance-promotion-and-offboarding/) for the performance-review programme this connects into.

The 30 / 60 / 90 rhythm is designed to catch broken onboarding *early*. Broken onboarding surfaced at day 30 is repairable; broken onboarding surfaced at day 180 has usually already turned into a leaver.

## The new-hire NPS feedback loop

An anonymous or semi-anonymous feedback survey to every new hire at fixed intervals is the corporation's leading indicator of onboarding quality. Typical cadence:

- **Day 14.** How was the pre-boarding and day-one experience?
- **Day 30.** How is the onboarding curriculum, the manager relationship, the buddy relationship?
- **Day 60.** How is your integration into the team? Are your expectations from the interview loop being met?
- **Day 90.** How is your overall experience? How likely are you to recommend the corporation as a place to work? (This is the "new-hire NPS" question — a 0–10 scale, with a written follow-up.)

The survey is short (5–10 questions), anchored to a mix of Likert-scale and free-text, and *reviewed*. The head of people reviews new-hire NPS trends monthly and surfaces themes to the executive team. A running dip in the day-14 score reliably signals a broken provisioning workflow; a dip in the day-60 score signals a broken team-integration pattern; a dip in the day-90 score is a retention leading indicator.

The single largest failure mode of the new-hire NPS is failing to *act* on it. Collecting the data and not addressing the surfaced issues teaches the new hire that the corporation asks and does not listen — and worse, that the survey is theater.

## The intersection with the HRIS and the ATS

Nearly every operational surface in this chapter is instrumented in the ATS or the HRIS:

- Pre-boarding packet and countersign — ATS-driven at offer acceptance, HRIS-driven at start.
- Provisioning — identity provider (Okta / Google Workspace / Entra ID) with SCIM into every SaaS system, triggered by the HRIS at start.
- I-9 Section 1 and 2 — HRIS onboarding workflow.
- Benefits enrollment — HRIS or benefits-broker portal.
- Training and acknowledgments — LMS or HRIS training module.
- 30 / 60 / 90 check-in — HRIS or performance-management tool.
- New-hire NPS — HRIS or dedicated engagement-survey tool (Culture Amp, Lattice, 15Five, Officevibe, and others).

The onboarding programme lives in the HRIS. The HRIS choice (see [chapter 07](./07-hris-peo-payroll-stack.md)) constrains how well the onboarding programme can be operationalised at scale.

## A worked example — a Series-A first-90-day onboarding programme

The corporation is at Series-A with 22 employees, hiring 33 more over the next 18 months (see [chapters 01](./01-sourcing-operating-model-by-stage.md) and [02](./02-ats-selection-and-integration.md)). The head of people has ~2 hours per week to spend on onboarding programme design; the rest of the operating load falls on the HRIS (Rippling) and the hiring manager.

**Pre-boarding.**
- Automated welcome email from the recruiter within one business day of offer acceptance.
- Ashby → Rippling handoff triggers Rippling's onboarding workflow: I-9 Section 1, W-4, direct-deposit collection, benefits enrollment queued.
- Laptop shipped by IT at least 2 days before start date via the corporation's chosen MDM (Kandji).
- SSO account created in Okta 3 business days before start date.
- Pre-boarding packet emailed 1 week before start date: first-week agenda, buddy introduction, manager 1:1 pre-scheduled, benefits summary.
- Buddy sends a personal welcome message during pre-boarding.

**Day one.**
- 9:00 — Welcome + orientation with head of people (60 min).
- 10:00 — I-9 Section 2 (if in-office) or authorised-representative session scheduled (if remote).
- 10:30 — Setup verification with IT.
- 11:30 — 1:1 with manager (60 min).
- 12:30 — Lunch with buddy.
- 14:00 — Team introductions.
- 15:00 — Onboarding curriculum kickoff (self-serve modules).
- 16:30 — End-of-day wrap.

**First week.**
- Weekly 1:1 with manager scheduled.
- Cross-functional intros (3 × 30 min) scheduled by manager.
- Attend standups, all-hands, and one cross-functional meeting.
- Mandatory training (security, sexual-harassment-prevention, code-of-conduct) via the HRIS training module.
- First concrete deliverable assigned by end of week.

**30 / 60 / 90-day check-ins.** Scheduled at offer acceptance, recurring in the manager's and head-of-people's calendar. Templates in Rippling's onboarding module. Outcome recorded.

**New-hire NPS.** Rippling triggers a 5-question survey at day 14, day 30, day 60, and day 90. Head of people reviews the trend monthly. Themes surfaced to CEO at monthly staff meeting.

## Summary

- Onboarding runs from offer acceptance through the 90-day anniversary — it is a designed programme, not a day-one welcome event.
- Pre-boarding is the highest-leverage window: personalised welcome, pre-boarding packet, buddy assignment, pre-scheduled 1:1s, and complete provisioning *before* day one.
- Day one has a scheduled agenda — orientation, I-9 Section 2, employment-document countersign, benefits-enrollment kickoff, manager 1:1, buddy introduction, team introductions, setup verification.
- First week is the transition from "welcome" to "your work" — recurring 1:1s, team meetings, cross-functional intros, mandatory training, first deliverable assigned.
- 30 / 60 / 90-day check-ins are the operating instrument that catches broken onboarding before it becomes attrition. Each has a defined structure and a documented outcome.
- New-hire NPS at 14 / 30 / 60 / 90 days is the leading indicator of onboarding quality. Collect it, review it, and *act* on it.
- The onboarding programme lives in the HRIS. The ATS → HRIS handoff at offer acceptance is what makes onboarding an operational workflow rather than an ad-hoc scramble.
