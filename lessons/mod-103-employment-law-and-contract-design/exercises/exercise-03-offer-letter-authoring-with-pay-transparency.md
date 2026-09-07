# Exercise 03 — Offer-letter authoring with pay transparency

> Estimated time: **~4 hours** · Related chapter: [03 — Offer letters and pay transparency](../03-offer-letter-architecture-and-pay-transparency.md)

## Problem statement

The classification decisions from exercises 01 and 02 are baked. Acme Robotics is now issuing offers for the Q4 hires. You are drafting the offer letters and the surrounding job-posting compliance workflow — the state-of-the-art, pay-transparency-compliant, EFAA-aware, *McLaren Macomb*-compliant, PIIA-integrated, contingent-condition-aware offer-letter package that mod-103 chapter 03 sets the standard for.

The corporation hires across California (LA and SF), New York State (Manhattan), Washington (Seattle), Colorado (Denver), and Illinois (Chicago). All four of the following hires must go out this week:

- **Hire 1 — Senior Software Engineer, San Francisco, Bay Area.** W-2 exempt (computer-employee), $220k base, standard equity grant of 40,000 options at the current $0.75 strike, one-time signing bonus of $15,000, standard benefits package.
- **Hire 2 — Head of Marketing, Los Angeles.** W-2 exempt (executive), $220k base, standard equity grant of 60,000 options at the current $0.75 strike, standard benefits.
- **Hire 3 — Executive Assistant to CEO, San Francisco.** W-2 non-exempt (per exercise 02), $95k base (annualised from an hourly rate), no signing bonus, no equity, standard benefits. Because the role is non-exempt, hourly-rate framing is required.
- **Hire 4 — Enterprise SDR, Seattle.** W-2 non-exempt (per exercises 01 and 02), $60k base + commission (OTE $110k), 10,000 option grant, standard benefits.

Each offer must also comply with the applicable state's job-posting range-disclosure and salary-history-ban statutes, and with the federal and state FCRA / Fair Chance rules if the offer is contingent on a background check.

## Requirements

### Part A — Offer-letter drafts (four letters)

For each of the four hires, draft a complete offer letter. Each letter must include, at minimum:

1. **Recital and effective date.** Corporation name, addressee, effective date.
2. **Position, reporting line, and location.** Job title, department, reporting-line manager, primary work location (with state cited), and remote-work posture if applicable.
3. **Start date.** With any contingent-condition language attached.
4. **At-will framing.** The clear at-will statement, with the Montana carve-out where applicable (none of the four hires are in Montana — but state where in the template the Montana carve-out would appear if the corporation opened a Montana office).
5. **Compensation.**
   - **Cash compensation.** Base salary (for exempt) or hourly rate (for non-exempt, with annualisation reference), pay-period cadence, payroll cycle.
   - **Bonus or commission structure** where applicable. For Hire 4, sketch the commission-plan reference; do not draft the full commission plan (it is a separate document).
   - **Equity.** Reference to the equity grant subject to board approval, standard four-year vesting with one-year cliff, exercise price determined by 409A valuation, reference to the equity plan document. Do not attempt to author the option grant agreement — that is mod-105.
   - **Benefits.** Reference to the standard benefits package (health/dental/vision, 401(k), FSA/HSA, PTO, sick leave, paid family leave to the extent state law requires) with a note that specific benefit-plan terms govern.
   - **Signing bonus** where applicable, with the clawback / repayment condition if the employee leaves within a defined period.
6. **Reference to standalone agreements.** PIIA (exercise 04), arbitration agreement (exercise 08), any relocation agreement, any commission-plan agreement.
7. **Employee-handbook reference.** With the standard "handbook is not a contract, employer reserves right to amend" language, tempered by the *McLaren Macomb* concerns about overbroad workplace-rule language.
8. **Contingent conditions.**
   - I-9 Form completion within 3 business days of start.
   - Reference-check completion (state whether a formal reference check is required for the role).
   - Background check with FCRA / applicable state-law consent (Fair Chance rules for California, Illinois, NYC Fair Chance if applicable, Washington, Colorado, per chapter 08).
   - Any drug-testing requirement (for a technology-industry startup with no safety-sensitive roles, typically none; state so).
   - Evidence of authorisation to work in the US (E-Verify if the corporation is enrolled).
9. **Pay-transparency-compliant range disclosure** — see Part B.
10. **Non-solicitation of prior employer** — a representation that the employee's acceptance and performance of the offer does not violate any obligation to a prior employer, and does not require the use of any prior employer's confidential information or trade secrets. Reference to the PIIA's more-detailed treatment.
11. **Signature block and date.**

Do NOT draft:

- The PIIA (exercise 04).
- The NDA / MNDA (exercise 04).
- The arbitration provision (exercise 08).
- The full commission plan (a separate document).
- The equity grant agreement (mod-105).

Instead, reference these documents in the offer letter with placeholder cross-references.

### Part B — Pay-transparency compliance

For each of the four postings that led to these offers, produce the job-posting range disclosure that must have appeared on the posting per the applicable state and city statute. Cite the statute (California SB 1162 / Cal. Lab. Code § 432.3(c); New York State Lab. Law § 194-b; New York City Local Law 32; Illinois HB 3129 / 820 ILCS 112; Washington RCW 49.58.110; Colorado C.R.S. § 8-5-201 et seq. as expanded by SB 23-105).

For each posting, produce:

1. **The compensation range** — reasonable good-faith range for the role and location.
2. **The benefits summary** — the states differ on what is required (Colorado requires a "general description of benefits and any other compensation"; Washington requires wage-and-benefits disclosure; California requires the pay scale; New York requires the minimum-and-maximum annual salary or hourly rate).
3. **The equity or additional-compensation disclosure** — Colorado requires "any other compensation" including equity; states diverge on this.
4. **The compliance rationale** — a short paragraph tying the range to the corporation's compensation architecture (which would be authored in mod-106), noting that the range is a good-faith estimate under the applicable state statute and that individual offers may fall anywhere in the range based on skills, experience, and location.

If the same role is posted to multiple states (e.g., the SDR posting appears on Seattle, LA, Denver, and Chicago boards), you must comply with each applicable state's disclosure requirements, which may require different range disclosures per posting.

### Part C — Salary-history-inquiry compliance workflow

Produce a short (1–2 page) workflow memo for the ATS and recruiting team addressing:

- **Prohibited inquiries.** No question about the candidate's prior salary, benefits, or total compensation on the application, in the initial screen, in the interview, or in the offer-negotiation conversation. This is required in California, New York, Massachusetts, Colorado, Washington, Oregon, Illinois, and many cities where the corporation may source from.
- **Permitted disclosures.** The candidate may voluntarily disclose their salary expectations or their prior compensation; the corporation may then rely on those disclosures without violating the statute in most jurisdictions, but must not solicit them.
- **Recruiter training and ATS configuration.** Rewrite the ATS pre-screen fields to remove any "current compensation" or "desired compensation" field that requires an answer. Update the recruiter script to prohibit the "so what are you making now?" or "what are your salary expectations?" question — the first is prohibited; the second is permitted but risky and creates a documentation problem.
- **Pay-setting methodology.** The offer is set from the compensation architecture (level + role + location) and the posted range, not from the candidate's prior compensation. Document the methodology so the corporation can defend against a state pay-equity / EPA claim.

### Part D — Fair Chance / background-check compliance workflow

For each of the four hires, produce a workflow entry for the FCRA / applicable Fair Chance Act compliance:

- **Pre-conditional-offer restrictions.** No criminal-history inquiry prior to conditional offer. The initial application is scrubbed of any criminal-history question. Any early recruiter screen does not ask about criminal history.
- **Consent and disclosure.** After conditional offer, FCRA disclosure and consent form (15 U.S.C. § 1681b(b)(2)) — standalone document, not embedded in an application, per federal case law and FTC guidance.
- **Pre-adverse-action notice.** If the corporation is considering rescinding the offer based on the background-check report, deliver the pre-adverse-action notice with (a) a copy of the report, (b) a copy of the FTC summary of consumer rights, (c) the state-required individualised-assessment write-up (California Fair Chance Act, Illinois Employee Background Fairness Act, NYC Fair Chance Act, Washington Fair Chance Act, Colorado Chance to Compete Act — each has specific requirements).
- **Response period.** Federal FCRA requires a reasonable time; California requires a minimum of 5 business days after receipt; other states have their own minimums. Cite the applicable state's minimum.
- **Post-adverse-action notice.** If the corporation proceeds with adverse action after considering the candidate's response, deliver the post-adverse-action notice.
- **State-specific individualised-assessment methodology.** The California Fair Chance Act requires consideration of the nature and gravity of the offense, the time elapsed, and the nature of the job. Illinois and NYC have their own factor lists. Produce a template individualised-assessment write-up.

### Part E — NYC / Colorado / Illinois-specific posting language for hires posted to multiple cities

Assume Hire 4 (Seattle SDR) is posted to Seattle, LA, Denver, Chicago, and NYC. Produce the posting-compliance matrix showing, for each city:

- The applicable statute.
- The specific disclosure required.
- Any additional disclosure elements (benefits, equity, other compensation).
- Any additional Fair Chance or salary-history-ban language required in the posting.

Note that the NYC posting has its own posting-transparency requirement (NYC Local Law 32); the state NY law (Lab. Law § 194-b) also applies. Confirm both.

### Part F — Design-choices memo

A 2–3 page memo covering:

- The offer-letter template structure and why (chapter 03's architecture).
- Any deviations from chapter 03's baseline, with reasoning.
- The Montana carve-out placement.
- The signing-bonus clawback structure and the applicable-state enforcement considerations (California disfavors mandatory-repayment clauses that operate as de facto restrictive covenants; consider a graduated repayment schedule).
- The at-will drafting and the interaction with the introductory-period or contingent-condition framing.
- The interaction with the EFAA carve-out language (chapter 09) — the offer letter's confidentiality references must anticipate the EFAA / Speak Out Act / *McLaren Macomb* posture.
- Any `<!-- needs-research -->` items you flagged (current-year state salary-basis thresholds, current-year FCRA / Fair Chance procedural specifics, current-year pay-transparency-statute amendments).

## Starter guidance

- Chapter 03 is the primary reference. Use its architecture — recitals, at-will, compensation, contingent conditions, standalone-agreement references, pay-transparency range — as the spine of your template.
- Do NOT draft the PIIA, NDA, or arbitration provision here; reserve slots and cross-reference. Those are exercises 04 and 08.
- Do NOT compute the equity-grant details or 409A valuation; reference the equity plan and cite the current 409A valuation source.
- For the non-exempt hires (Hire 3, Hire 4), the compensation framing must be hourly rate with annualisation reference, not "salary." This is a material distinction — treating a non-exempt employee as if they were salaried creates back-overtime exposure regardless of the offer-letter label.
- Signing-bonus clawback for Hire 1 requires California-specific care. A "if you leave within 12 months, you repay 100%" clause has been treated as a restraint of trade in some California cases. A graduated schedule (100% in month 1, decaying to 0% by month 12) is the more defensible pattern.
- Pay-transparency compliance is a *posting* obligation, not an *offer-letter* obligation — but the offer letter should state the range as consistent with the posting.
- Salary-history-inquiry rules are strict in each of the corporation's five states. The workflow memo is the operational compliance mechanism.
- Fair Chance procedures are procedurally specific and jurisdiction-variable. Do not draft a generic FCRA-only workflow — each state's Fair Chance overlay has its own steps.
- Do not include a "confidentiality of this offer letter" clause that would run afoul of *McLaren Macomb*. Any non-disparagement or confidentiality language must carry the NLRA / EEOC / government-cooperation carve-out.

## Deliverables

- `offer-letter-hire-1-swe.md`, `offer-letter-hire-2-marketing.md`, `offer-letter-hire-3-ea.md`, `offer-letter-hire-4-sdr.md` — Part A. Four offer letters.
- `job-posting-range-disclosures.md` — Part B. One posting per role.
- `salary-history-workflow-memo.md` — Part C.
- `background-check-and-fair-chance-workflow.md` — Part D.
- `sdr-multi-city-posting-matrix.md` — Part E.
- `offer-letter-design-choices-memo.md` — Part F.

## Acceptance criteria

The package is acceptable if:

1. Every offer letter has all eleven core elements (recital, position/reporting/location, start date, at-will, compensation, standalone-agreement references, handbook reference, contingent conditions, pay-transparency range, prior-employer rep, signature block).
2. Hire 3 (EA, non-exempt) is framed in hourly-rate terms; annualisation is a note, not the primary framing.
3. Hire 4 (SDR, non-exempt) has a commission-plan reference (not a full commission plan) and is framed as non-exempt with time-tracking obligations flagged.
4. Hire 1's signing-bonus clawback is drafted with a California-defensible graduated repayment structure.
5. The Montana carve-out is present in the template (or explicitly noted as reserved for future Montana expansion).
6. Pay-transparency disclosure is present in each posting per the applicable state statute, with the correct statutory citation.
7. The salary-history-workflow memo prohibits the specific "current comp" and "expected comp" questions, distinguishes prohibited vs. permitted disclosures, and addresses ATS configuration and recruiter training.
8. The Fair Chance workflow includes pre-conditional-offer restrictions, standalone FCRA disclosure, individualised-assessment methodology per state, and the specific state-required minimum response periods.
9. The SDR multi-city posting matrix identifies the correct statutes and disclosure requirements for each city.
10. Every offer letter reserves — but does not draft — the PIIA, NDA, and arbitration provisions.
11. Every offer letter's confidentiality references anticipate *McLaren Macomb* and the EFAA carve-outs.
12. Statutory citations (Cal. Lab. Code § 432.3; NY Lab. Law § 194-b; NYC Local Law 32; Illinois HB 3129 / 820 ILCS 112; RCW 49.58.110; C.R.S. § 8-5-201 et seq.; 15 U.S.C. § 1681b(b)(2); California Fair Chance Act / Cal. Gov. Code § 12952; NYC Fair Chance Act; Illinois Employee Background Fairness Act; Washington Fair Chance Act; Colorado Chance to Compete Act) are correct.
13. Nothing left as `[FILL IN]` — every field populated or explicitly flagged with a `<!-- needs-research -->` marker.
