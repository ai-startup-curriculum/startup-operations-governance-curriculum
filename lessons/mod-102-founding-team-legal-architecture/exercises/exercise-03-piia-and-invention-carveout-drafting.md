# Exercise 03 — PIIA and invention-carveout drafting

> Estimated time: **~4 hours** · Related chapter: [04 — The mutual IP assignment (PIIA)](../04-piia-mutual-ip-assignment.md)

## Problem statement

Same three founders as in exercises 01 and 02. The founder agreement is signed; the SPAs and 83(b)s are queued for formation day. The **PIIA** — the mutual IP assignment that makes the corporation the owner of the founders' contributions — is the last document the founders must execute before touching another line of code on the corporation's behalf. Author each founder's PIIA to the standard chapter 04 sets, including the state-law invention-assignment carveouts and a completed Prior Inventions schedule, and reconcile the Prior Inventions schedule with the SPA consideration produced in exercise 02.

The DTSA whistleblower-immunity notice (18 U.S.C. § 1833(b)(3)) is authored in exercise 04; you should reference it here and reserve a slot for it in the PIIA, but you are not producing the full notice text in this exercise.

## Founder facts relevant to the PIIA (in addition to exercises 01 and 02)

- **Alex Chen (CEO)** — resident of California. Prior employer (a public cloud company) had a standard PIIA with a Cal. Lab. Code § 2870 carveout. Alex's 30-page technical memo and 8-month prototype work were done on personal equipment and personal time; the prototype is 100% new code, not derived from the prior employer's codebase. Alex has separately: (a) an open-source Python library `pyfast-tokenizer` (Apache 2.0, unrelated), (b) a personal blog, (c) a co-inventor position on a pending patent application filed at the prior employer's expense, unrelated to the new company's domain.
- **Priya Rao (CTO)** — resident of Washington state. Coming from a Series-C startup where she was subject to a PIIA. Her 3 months of full-time work were during unpaid leave, on personal equipment, on subject matter distinct from her prior employer's product. She has confirmed with a plain-language reading of her prior PIIA that "work done on unpaid leave, outside working hours, and unrelated to employer's business" is not assigned to the prior employer — but she has *not* obtained a written release. Priya also has: (a) a Distributed Systems PhD thesis and two co-authored papers, and (b) prior-startup common-stock holdings.
- **Marcus Hill (VP GTM)** — resident of Illinois. Coming from an enterprise SaaS company where he is currently still employed (through formation day + 2 weeks of transition). His employer's employment agreement includes a broad customer-non-solicit for 12 months post-departure. Marcus has: (a) an outside advisory position with a portfolio company at his current employer's VC arm (paid annually with $10k of stock; disclosed to current employer), (b) a personal LinkedIn newsletter about enterprise-sales strategy (personal IP; unrelated to the new corporation), (c) no prior-invention IP being contributed to the corporation.

## Requirements

### Part A — Founder PIIA (three versions, one per founder)

Draft a PIIA for each founder that includes, at minimum:

1. **Recitals and effective date.**
2. **Present-assignment language** — chapter 04 requires "hereby assigns," not "agrees to assign" (per *Stanford v. Roche*, 583 F.3d 832 (Fed. Cir. 2009), aff'd, 563 U.S. 776 (2011)). Cite the case in your design-choices memo.
3. **Work-made-for-hire language** for copyrightable subject matter that qualifies under 17 U.S.C. § 101, *plus an assignment backstop* for anything that does not qualify.
4. **Confidential-information definition** — technical, business, third-party, and personnel information; obligation to use only for the corporation; obligation to protect; obligation to return on termination.
5. **Ongoing duty to disclose inventions.**
6. **Further-assurances and power-of-attorney** clause for patent and copyright perfection.
7. **Moral-rights waiver** (to the extent permitted) — brief; note in the design memo that this is largely a non-issue for US-only startups and becomes material in international expansion (mod-113).
8. **Post-termination obligations** — continuing confidentiality (indefinite for trade secrets; defined period for other confidential information); return of property; trailing-inventions assignment for a narrow post-termination window (state your window and justify against chapter 04's guidance).
9. **Slot for the DTSA whistleblower-immunity notice** — reference the location where exercise 04 will drop the notice text. Do not leave it as "[TBD]"; state that the notice will be an integral clause and reference § 1833(b)(3).
10. **Prior Inventions schedule** (see Part B).
11. **State-law invention-assignment carveout schedule** (see Part C).

### Part B — Prior Inventions schedule (three schedules, one per founder)

Complete each founder's Prior Inventions schedule per chapter 04. For each item the founder claims as prior work, capture: item name, brief description, date of creation, whether *retained* by the founder (carved out) or *assigned* to the corporation as SPA consideration. Reconcile with the SPA's consideration section from exercise 02 — any IP contributed as SPA consideration should appear here as **assigned** (with a cross-reference to the SPA), not carved out.

Include the correct items per the founder facts above:

- Alex: at minimum, `pyfast-tokenizer`, the blog, the prior-employer pending patent (retained; not assignable by Alex without prior-employer release), and the 8-month prototype + technical memo (contributed as SPA consideration — assigned).
- Priya: at minimum, the PhD thesis, the two co-authored papers, prior-startup common-stock holdings, and the 3-month prototype work (contributed as SPA consideration — assigned).
- Marcus: any items relevant to his outside-advisory arrangement, the newsletter, and confirmation that no prior-invention IP is being contributed.

A **blank Prior Inventions schedule** is a defect — chapter 04 calls it "fill-in-or-forfeit." Signing a schedule with "None" is a legitimate answer only if the founder truly has no prior work; each of these founders has something to list.

### Part C — State-law invention-assignment carveout schedule

For each founder, include the applicable state-law carveout language:

- **Alex (California)** — Cal. Lab. Code § 2870 carveout, plus the § 2872 written notification. Quote or excerpt the statutory text.
- **Priya (Washington)** — RCW 49.44.140.
- **Marcus (Illinois)** — 765 ILCS 1060/2 (Illinois Employee Patent Act).

If a founder later moves states, note in the design memo whether the corporation would amend the PIIA or add a state-specific rider. Do not attempt to draft carveouts for states with no invention-assignment statute (e.g., some southern states) — chapter 04 notes the state list is variable, so use the states relevant to these three founders.

Reference the `<!-- needs-research -->` marker in chapter 04 on the evolving state list; if you are drafting for production and the corporation is hiring across a broad footprint, the best practice is a unified multi-state carveout schedule keyed to each individual's state.

### Part D — Reconciliation with prior-employer obligations

For each founder, produce a short (1–2 paragraph) reconciliation note addressing:

- What the prior-employer PIIA (or absence of one) covers.
- Whether the founder's pre-formation work for the corporation is arguably owned by the prior employer under that PIIA.
- Any pending patent applications, restrictive covenants, or unresolved IP claims from the prior employer.
- The founder's representation in the SPA / PIIA about no-conflicting-obligation, and whether that rep is defensible on the facts.
- Any recommended cleanup (written release from prior employer, legal opinion, disclosed schedule of exception at Series-A).

Priya's case in particular — pre-formation work during unpaid leave, no written release — is chapter 06's "unresolved former employer" pattern. Flag it.

### Part E — Design-choices memo

A 1–2 page memo covering every material drafting choice:

- The present-assignment language and *Stanford v. Roche* citation.
- The trailing-inventions post-termination window (why the window you chose).
- The moral-rights waiver approach.
- The state-carveout drafting approach (per-state vs. unified schedule).
- Any deviations from chapter 04's baseline, with reasoning.
- The reserved slot for the DTSA notice (exercise 04).

## Starter guidance

- Chapter 04's "Present-assignment language" section is authoritative on the tense choice. Any drafter using "agrees to assign" is drafting a defect.
- The Prior Inventions schedule reconciles with the SPA's consideration language; pre-formation IP that is contributed as SPA consideration is *assigned* here, not retained. Chapter 04 lays out the typical two-step: identify the pre-existing work in the schedule, and execute a separate express assignment (or a Prior-Inventions "assigned" line item) that transfers title.
- The Cal. Lab. Code § 2872 notification is a written statement to the employee; make sure Alex's PIIA package includes it, not just the § 2870 carveout language.
- Do not draft the DTSA notice here — reserve the slot. Exercise 04 covers that.
- For any state whose invention-assignment statute you cite, confirm the current citation against the state's code before quoting text. The chapter 04 `<!-- needs-research -->` marker flags the evolving landscape.
- Priya's unresolved prior-employer question is where founders lose ownership in the worst case; do not paper over it. Flag it and recommend a specific cleanup.
- Do not draft a full non-solicit or non-compete inside the PIIA — chapter 04 defers to mod-103 and to the employment agreement (exercise not in this module). Note the deferral.

## Deliverables

- `piia-alex-chen.md`, `piia-priya-rao.md`, `piia-marcus-hill.md` — three founder PIIAs, execution-ready except for the DTSA-notice slot. Part A.
- `prior-inventions-schedule-alex-chen.md`, `prior-inventions-schedule-priya-rao.md`, `prior-inventions-schedule-marcus-hill.md` — completed Prior Inventions schedules. Part B.
- `state-carveout-schedules.md` — the § 2870 / § 2872, RCW 49.44.140, and 765 ILCS 1060/2 carveout language keyed to each founder. Part C.
- `prior-employer-reconciliation.md` — Part D.
- `piia-design-choices-memo.md` — Part E.

## Acceptance criteria

The package is acceptable if:

1. Every PIIA uses **"hereby assigns"** present-assignment language. Any "agrees to assign" is a fail.
2. Every PIIA has a work-made-for-hire clause paired with an assignment backstop.
3. Every Prior Inventions schedule is populated per each founder's facts — no blank schedules, no lazy "None."
4. Pre-formation IP contributed as SPA consideration is assigned via the Prior Inventions schedule (with a cross-reference to the SPA) or via a parallel express IP assignment, not merely carved out.
5. Cal. Lab. Code § 2870 carveout **and** § 2872 written notice are both present for Alex.
6. State carveouts are present and correct for Priya (Washington) and Marcus (Illinois).
7. Every PIIA reserves a slot for the DTSA whistleblower-immunity notice (per chapter 05 / exercise 04) rather than treating the notice as optional.
8. The prior-employer reconciliation flags Priya's unresolved unpaid-leave question and Alex's pending prior-employer patent explicitly.
9. Nothing left as `[FILL IN]` or `[TBD]` — every field populated or explicitly flagged as a cross-reference to another document.
10. Statute and case citations (17 U.S.C. § 101, *Stanford v. Roche*, Cal. Lab. Code §§ 2870 / 2872, RCW 49.44.140, 765 ILCS 1060/2) are correct.
