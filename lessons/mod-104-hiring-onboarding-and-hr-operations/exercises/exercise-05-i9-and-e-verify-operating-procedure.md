# Exercise 05 — I-9 and E-Verify operating procedure

> Estimated time: **~4 hours** · Related chapter: [05 — Form I-9 and E-Verify](../05-i9-and-e-verify.md)

## Problem statement

Redwood Sensor Systems is a Delaware C-corp, 61 employees, on Gusto as its HRIS. Redwood has W-2 employees in California, Colorado, New York, Massachusetts, Florida, and Georgia, plus one H-1B visa holder (in California, with work authorisation valid through 2028) and one recent university-graduate hire on an F-1 STEM OPT extension (in Massachusetts, current work authorisation valid for another 20 months). The corporation is not a federal contractor but is preparing to bid on a Department of Defense pilot program in Q2 which would trigger FAR 52.222-54 within 90 days of contract award.

Three things have surfaced in the last 30 days:

1. **Internal-audit discovery.** The Head of People (you) has just inherited the function from a departing predecessor. Reviewing the I-9 files reveals: 4 missing I-9s (employees who started 3–14 months ago); 7 I-9s where Section 2 was completed more than three business days after the start date (typical delay 5–12 days); 3 I-9s where the wrong document combination was recorded (a List B + List B pattern); 2 I-9s using the *prior* USCIS edition of the form; and 1 I-9 for an employee who terminated 18 months ago that is still in the active file (retention window may or may not be current).
2. **Remote-hire growth.** Redwood plans to hire 15 fully remote employees in the next 6 months, across states where Redwood has no physical office presence. The current in-person Section 2 workflow does not scale to remote hires. Gusto's authorised-representative network is available but has been ad-hoc so far.
3. **Reverification calendar.** The H-1B employee's I-797 approval extends through 2028, but a routine amendment was filed 60 days ago and the corporation's HR does not have a tickler system to track the current-authorisation-document expiration. The F-1 STEM OPT extension expires in 20 months; no reverification workflow is scheduled.

The CEO wants (a) an internal-audit report with corrections completed, (b) a written I-9 / E-Verify operating procedure the corporation can hand to its counsel and its auditors, (c) an E-Verify enrollment decision, and (d) a specific NOI response plan.

## Requirements

### Part A — Internal-audit report and corrections

Produce a written internal-audit report covering:

1. **Findings inventory** — the specific list of errors from the current I-9 files, categorised by severity per USCIS's substantive-vs-technical framework:
   - **Substantive violations** — missing I-9s, unverified documents, wrong document combinations (List B + List B), unsigned Section 2, missing Preparer / Translator Certification when required.
   - **Technical / procedural violations** — Section 2 completed late, wrong form edition, missing dates in specific fields, incorrect but re-verifiable document details.
2. **Correction plan** — for each finding, the specific corrective action per the USCIS M-274 correction methodology:
   - Missing I-9s: complete a new I-9 immediately using the *current* date (not the original hire date), and record the circumstances of the correction. Cite the M-274.
   - Late Section 2: correct is not possible retroactively; note the delay, do *not* backdate.
   - Wrong document combination: engage the employee to present acceptable documents from Lists A or B+C, then correct Section 2 with the single-line-through / initial / date methodology.
   - Prior form edition: complete new I-9 on the current form and staple the prior form behind it with a note.
   - Terminated-employee retention: apply the "three years after hire, or one year after termination, whichever is later" rule; determine whether the file is past its retention window and, if so, document destruction.
3. **Communications plan** — the messaging to each employee whose I-9 requires their engagement to correct (missing I-9s, wrong document combination). Include the specific wording the head of people will use (in coordination with counsel).
4. **Documentation posture** — how the corporation records the audit itself, the corrections made, and the counsel review — in a way that reads defensibly in a future ICE NOI.

### Part B — Written I-9 / E-Verify operating procedure

Produce the corporation's written I-9 and E-Verify operating procedure, the artifact that Redwood's counsel and future auditors will read. Cover:

1. **Roles and responsibilities** — who owns which step (recruiter, hiring manager, Head of People, HRIS admin, authorised representative for remote hires, immigration counsel for edge cases).
2. **Pre-boarding I-9 workflow** — Section 1 sent from Gusto at offer acceptance, target completion date the day before start.
3. **Day-one / day-three Section 2 workflow** — the in-person path (in-office hires), the authorised-representative path (remote hires), and — if the corporation enrolls in E-Verify — the DHS alternative remote-procedure path. Include the deadline (three business days after the first day of employment) and the escalation if that deadline slips.
4. **The acceptable-documents list** — a summary Redwood presents to new hires. Include the important reminders: the employee chooses which documents to present; the employer may not require specific documents; List A alone is sufficient; List B + List C is the alternative.
5. **The Section 3 / reverification workflow** — the tickler system (Gusto's native alerts, or a supplementary calendar), the 90-days-before-expiration reminder cadence, the acceptable documents for reverification, and the explicit *do not reverify* rules (no green cards; no List B identity documents).
6. **Storage and retention** — segregated I-9 storage in Gusto's compliance module (or a segregated folder if Gusto's segregation is inadequate); electronic storage compliance with 8 C.F.R. § 274a.2(e); the retention schedule.
7. **The annual internal-audit cadence** — Q4 review of every I-9 in the current retention window, with counsel oversight; the audit report retained in the corporate record.
8. **The NOI response plan** — see Part D.
9. **Common errors and prevention** — the specific patterns to prevent (late Section 2, wrong document combination, expired form edition, forgotten reverification).

### Part C — E-Verify enrollment decision

Produce a decision memo on whether Redwood enrolls in E-Verify now. Cover:

1. **The mandatory-state analysis** — Redwood has employees in Florida and Georgia. Determine whether Redwood is currently required to enroll under Fla. Stat. § 448.095 (25+ employees threshold since July 1, 2023) or O.C.G.A. § 36-60-6. Cite the chapter's state list and flag the specific-per-state text as `<!-- needs-research -->` if not confidently sourced.
2. **The federal-contractor analysis** — the Q2 DoD pilot bid will trigger FAR 52.222-54 within 90 days of any contract award. Recommend enrolling in advance so the corporation is not scrambling to enroll and populate the contract-eligible workforce within the FAR clause's 30-day / 90-day windows.
3. **The remote-hire operating benefit** — E-Verify enrollment is a prerequisite for the DHS alternative remote-examination procedure. With 15 remote hires planned in the next 6 months, this is a material operating simplification.
4. **The obligations E-Verify enrollment adds** — the TNC workflow, no-adverse-action-during-TNC-resolution rule, poster requirement (English and Spanish), no-pre-hire-prescreening, no-selective-use, no-reverification-of-green-cards, MOU compliance, recordkeeping.
5. **Recommendation** — the specific enrollment decision (yes / no / defer), the target enrollment date, the poster deployment plan, and the training curriculum for the Head of People and the recruiter on the TNC workflow.

### Part D — NOI response plan

Produce a written NOI response plan the corporation can hand to counsel and its executive team. Cover:

1. **Day 0 — Notice served.** The specific actions in the first 4 business hours: (a) contact immigration counsel; (b) preserve the I-9 record set as of the moment of service; (c) identify the person who will interact with ICE (typically counsel; the corporation's Head of People supports); (d) internal-communications discipline (no one else discusses the audit).
2. **Days 1–3 — Production.** How Redwood produces every I-9 in the current retention window within the three-business-day statutory window (8 C.F.R. § 274a.2(b)(2)(ii)). The role of Gusto in extracting the I-9 data set; the format ICE typically requests; the accompanying documentation (E-Verify records if enrolled; annual-internal-audit reports).
3. **Days 3+ — Audit interaction.** The pattern of ICE's audit — Notice of Suspect Documents, Notice of Discrepancies, Notice of Intent to Fine (NIF). The corporation's response window (30 days on the NIF). The negotiation posture.
4. **Documentation** — every interaction with ICE recorded in a running log; every document produced logged; every finding tracked.
5. **The employee-communications posture** — how (or whether) the corporation communicates with employees during an audit. Cite the specific NLRA / privacy considerations without over-claiming; coordinate with counsel.

### Part E — Reverification calendar and workflow

Produce the specific reverification calendar and workflow. Cover:

1. **The H-1B employee.** Even though the I-797 extends through 2028, the current authorisation document (Section 2 record) may have a specific expiration date depending on what was originally recorded. Determine the reverification trigger. Note the 60-day amendment filing and its implications for the H-1B holder's continued authorisation (LCA-portability considerations; consult immigration counsel).
2. **The F-1 STEM OPT extension employee.** Reverification trigger 90 days before the STEM OPT expiration (approximately 17 months from today). The specific documents the employee must present to reverify (an unexpired EAD or the STEM OPT extension approval notice per M-274 guidance).
3. **The tickler system.** Where the reverification alerts are configured (Gusto native; a supplementary tool if needed); who receives the alert; the escalation if reverification cannot be completed by the expiration date (the corporation may not employ the person without a valid Section 3 update after the expiration).
4. **The do-not-reverify guardrails** — the explicit rules preventing the corporation from reverifying green-card expirations, List B identity-document expirations, or other non-reverifiable items.

## Starter guidance

- Chapter 05 is the primary reference. The three-day Section 2 rule, the acceptable-documents framework, the reverification triggers, the retention schedule, the storage / audit posture, and the E-Verify overlay are all covered.
- The USCIS M-274 Handbook is the operating reference — cite it when your correction methodology or edge-case handling requires an authoritative source. Do not summarise; cite.
- Do not manufacture I-9 civil penalty numbers. The chapter flags the DHS Federal Civil Penalties Inflation Adjustment schedule as a `<!-- needs-research -->` item — treat it the same way in your exposure discussion.
- The DHS alternative remote-examination procedure (88 Fed. Reg. 47990, July 25, 2023) has narrower eligibility than the COVID-era flexibility it replaced. Requires E-Verify enrollment plus good-standing criteria — cite the chapter's needs-research marker.
- For the H-1B and F-1 STEM OPT reverification questions, the specific document-acceptance rules are in the M-274 and depend on the initial Section 2 record. If your analysis requires the specific record to answer, name the record and note the analysis is contingent on what was originally recorded.
- The Florida E-Verify statute has an employer-size threshold (25+ employees) that Redwood now exceeds. The Georgia statute has its own thresholds and applicability. Verify per-state text; do not assume "we're on the list, so we're covered."
- Do not commit to a specific NOI settlement posture — that is counsel's call. The exercise is to structure the operational response.
- The employee-communications posture during an audit is legally sensitive. NLRA-protected concerted-activity rules apply if employees discuss the audit collectively. Do not over-claim; note the sensitivity and defer specifics to counsel.

## Deliverables

- `internal-audit-report-and-corrections-plan.md` — Part A.
- `i9-and-e-verify-operating-procedure.md` — Part B.
- `e-verify-enrollment-decision-memo.md` — Part C.
- `noi-response-plan.md` — Part D.
- `reverification-calendar-and-workflow.md` — Part E.

## Acceptance criteria

The package is acceptable if:

1. The internal-audit report categorises findings into substantive vs. technical / procedural per USCIS's framework and applies the M-274 correction methodology (single-line-through / initial / date; no backdating; no white-out) explicitly.
2. Missing-I-9 corrections use the *current* date (not the original hire date) with the correction circumstances documented, per the chapter and M-274.
3. The employee-communications plan (Part A) has specific wording, not a summary.
4. The written operating procedure (Part B) covers pre-boarding through retention, includes the reverification workflow, and names the annual internal-audit cadence.
5. The E-Verify enrollment decision (Part C) analyses Florida and Georgia mandatory status explicitly, addresses the Q2 federal-contractor trigger, and identifies the DHS alternative-remote-procedure eligibility benefit.
6. The E-Verify decision names the specific TNC-workflow training the Head of People will complete.
7. The NOI response plan (Part D) starts at Day 0 with counsel contact and record preservation, produces I-9s within the three-business-day statutory window, and includes a documentation-log discipline.
8. The reverification calendar (Part E) addresses both the H-1B and F-1 STEM OPT employees with 90-days-before-expiration tickler cadence and cites the M-274 for acceptable-document specifics.
9. The do-not-reverify rules are explicit — no green-card reverification, no List B identity-document reverification.
10. Every civil-penalty range, form-edition reference, and DHS-procedure citation is either taken from chapter 05 or flagged with `<!-- needs-research -->`.
11. Nothing left as `[TBD]` or `[FILL IN]`.
