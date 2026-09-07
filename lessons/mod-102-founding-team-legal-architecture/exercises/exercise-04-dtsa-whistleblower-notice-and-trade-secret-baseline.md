# Exercise 04 — DTSA whistleblower notice and trade-secret baseline

> Estimated time: **~2 hours** · Related chapter: [05 — The DTSA whistleblower-immunity notice and the trade-secret baseline](../05-dtsa-whistleblower-and-trade-secret-baseline.md)

## Problem statement

The three-founder corporation from exercises 01–03 has drafted PIIAs with a reserved slot for the DTSA whistleblower-immunity notice (18 U.S.C. § 1833(b)(3)). Two additional artefacts need the notice too: a lightweight contractor NDA the corporation will use for the machine-learning research advisor it plans to onboard next week, and the separation-agreement template the corporation is standing up ahead of a departure it does not currently expect but must be ready for.

You are also inheriting an active problem: the corporation's outside counsel provided the founders with a 2015-vintage PIIA template on formation day, and although the founders' PIIAs from exercise 03 will use the updated template, three employees hired via a lightweight incorporation service in the first four months of the corporation's life signed the 2015-vintage template. The 2015 template has *no* DTSA notice.

Author the DTSA notice, drop it into the three template families (PIIA / NDA / separation agreement), stand up the corporation's "reasonable measures" trade-secret baseline, and produce a retroactive-cleanup plan for the three affected employees.

## Requirements

### Part A — The DTSA whistleblower-immunity notice

Draft the DTSA notice as a stand-alone clause suitable for insertion into any trade-secret-related agreement. The notice must track 18 U.S.C. § 1833(b)(1)–(2) closely enough that a court reading it can confirm the employee (or contractor) was informed of the immunities. Chapter 05 provides a representative form; you may adapt it, but do not omit any of the three immunity elements:

1. Disclosure to a government official or attorney solely for reporting a suspected violation of law.
2. Disclosure in a complaint or other document filed under seal in a lawsuit.
3. Use of the trade secret in a retaliation lawsuit, subject to under-seal filing and no-disclosure-except-court-order restrictions.

State whether you are inlining the notice or cross-referencing to a policy document (chapter 05 notes that cross-reference is technically allowed under § 1833(b)(3)(B) but riskier); if you cross-reference, produce the referenced policy paragraph as well.

### Part B — Drop the notice into three template families

Insert the notice into each of:

1. **Founder PIIA** — into the reserved slot from exercise 03. Confirm placement (typically inside the confidentiality section).
2. **Contractor NDA (lightweight)** — a short (2–3 page) NDA suitable for a machine-learning research advisor with limited access to a specific model checkpoint. Include the DTSA notice per chapter 05's rule that the DTSA definition of "employee" includes contractors and consultants (18 U.S.C. § 1833(b)(4)).
3. **Separation-agreement template** — a template for a hypothetical future founder or employee departure, including the DTSA notice in the confidentiality-obligations section. Also include an OWBPA-compliant release skeleton for age-40-and-over departures (21-day consideration, 7-day revocation, written eligibility factors; see chapter 07). You are not drafting a full separation agreement — the departure playbook lives in exercise 06 — but the template's confidentiality and release sections need to be authored to standard here.

For each template, mark up (with a comment or bracketed callout) the exact clause where the DTSA notice sits, and confirm the notice is *inlined* (not cross-referenced) unless you have a written reason to cross-reference.

### Part C — Corporation's "reasonable measures" trade-secret baseline

Produce a written trade-secret protection program that satisfies the DTSA § 1839(3) "reasonable measures" element. Chapter 05 gives a nine-item checklist; adapt it for this corporation's actual formation-day scale (3 founders, ~4 employees, plans to hire quickly). At minimum:

1. PIIA-before-access hygiene.
2. Contractor confidentiality / IP assignment before any code or data access.
3. Written "Confidential Information" policy for the employee handbook (produce the policy paragraph — mod-104 owns the handbook depth, but the paragraph belongs here so it exists on formation day).
4. Whistleblower policy (produce the paragraph).
5. Access controls — MFA on GitHub / GitLab, SSO with automatic offboarding, least-privilege access on production data and model weights.
6. Vendor NDAs.
7. Board-approved IP strategy (a two-paragraph placeholder — this is a board-level decision that will be revisited but should exist on formation day).
8. Marking discipline — internal documents labeled "Confidential."
9. Onboarding and offboarding checklists — PIIA execution, access provisioning, access revocation, property return, exit-interview confirmation.

The output should be a `trade-secret-baseline-program.md` that a board can adopt via written consent on the same day as formation.

### Part D — Retroactive-cleanup plan for the three 2015-template employees

The three employees signed a 2015-vintage PIIA with no DTSA notice. Produce a written cleanup plan:

1. **Diagnosis.** State exactly what the corporation forfeits under 18 U.S.C. § 1836(b)(3)(C)–(D) against these three employees — chapter 05 says exemplary damages up to 2× and attorneys' fees under DTSA are unavailable for pre-update conduct.
2. **Cleanup mechanic.** Adopt an updated PIIA template. Have each of the three employees re-sign the updated PIIA. Per chapter 05, "entered into or updated after May 11, 2016" is the § 1833(b)(3) trigger — the update itself brings the individual under the notice regime prospectively.
3. **Communication.** Draft a 3–4 sentence internal-comms note the corporation will send to the three employees explaining the update. Chapter 05 recommends framing this as a conformance update to a 2016 federal statute, not as a change to existing obligations.
4. **Handbook update.** Confirm the employee-handbook "Confidential Information" policy contains the DTSA notice or cross-references it correctly.
5. **Board consent.** A one-page board consent authorising the updated program and the re-signing.
6. **Compliance-calendar entry.** Add a recurring "template drift review" to the compliance calendar so a future 2016-style oversight does not repeat.

### Part E — Design and drafting notes

A short memo (1 page) covering:

- Where you placed the notice in each template and why.
- Whether you inlined or cross-referenced (with reasoning).
- The DTSA remedy stack the notice preserves (injunctive relief, compensatory damages, exemplary damages up to 2×, attorneys' fees for willful and malicious misappropriation, ex parte seizure in extraordinary circumstances).
- Any deviations from chapter 05's guidance.

## Starter guidance

- The DTSA notice is a *single paragraph*. Chapter 05 provides a representative form. Do not over-draft it.
- Do not draft language that narrows or waives the immunities themselves — the notice is a *disclosure*, not a contractual restraint. Any language purporting to limit the immunities is a fail (and probably unenforceable).
- 18 U.S.C. § 1833(b)(4) defines "employee" to include contractors and consultants. The NDA needs the notice.
- The separation-agreement template's OWBPA formalities apply only to age-40-and-over releases of federal age-discrimination claims. Do not apply them to a hypothetical age-30 departure — but the template should call out the age threshold.
- The "reasonable measures" checklist is meant to be operationally realistic at formation-day scale — do not draft a Fortune 500 information-security program. The point is that the corporation is *taking* measures, in writing, from day one.
- For the retroactive cleanup, the three employees should be told the update is not adverse to their existing obligations — chapter 05 recommends framing.
- Reference the `<!-- needs-research -->` markers in chapter 05 on California Bus. & Prof. Code § 16600 amendments and FTC non-compete rule status if you draft any employee-facing language that intersects with post-employment obligations. Do not invent current-state legal conclusions.

## Deliverables

- `dtsa-notice-clause.md` — the stand-alone notice. Part A.
- Updated `piia-alex-chen.md` / `piia-priya-rao.md` / `piia-marcus-hill.md` — with the notice dropped in, or an addendum file `piia-dtsa-notice-insertion.md` if you prefer not to touch the exercise-03 output.
- `contractor-nda-template.md` — the lightweight ML-research-advisor NDA with the notice. Part B.
- `separation-agreement-template.md` — the template with the notice and OWBPA release skeleton. Part B.
- `trade-secret-baseline-program.md` — the reasonable-measures program. Part C.
- `retroactive-cleanup-plan.md` — the plan for the three employees. Part D.
- `dtsa-design-notes.md` — the design and drafting memo. Part E.

## Acceptance criteria

The package is acceptable if:

1. The DTSA notice tracks 18 U.S.C. § 1833(b)(1)–(2) closely enough that all three immunity elements are covered. Missing any immunity is a defect.
2. The notice is present (inlined by default) in the founder PIIA, the contractor NDA, and the separation-agreement template.
3. The contractor NDA is drafted with the recognition that contractors are within § 1833(b)(4)'s "employee" scope.
4. The separation-agreement template's OWBPA release skeleton is present and gated to age-40-and-over departures.
5. The reasonable-measures program covers all nine chapter 05 items, adapted for formation-day scale.
6. The retroactive-cleanup plan is honest — it does not claim to *cure* pre-update conduct (which is not curable); it explains what is forfeited and how prospective coverage is restored.
7. The board consent authorising the updated program is included.
8. Statutory citations (18 U.S.C. §§ 1836–1839, § 1833(b), § 1839(3)) are correct.
9. No fabricated "current status" of the FTC non-compete rule or California § 16600 landscape is asserted — any such reference is deferred to the `<!-- needs-research -->` markers or is explicit about the drafting date.
