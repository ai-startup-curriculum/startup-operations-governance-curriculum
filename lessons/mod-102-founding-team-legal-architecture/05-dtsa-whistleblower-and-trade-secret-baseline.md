# 5. The DTSA whistleblower-immunity notice and the trade-secret baseline

> One paragraph in every PIIA. Omit it and you forfeit the corporation's ability to recover exemplary damages and attorneys' fees when someone walks out with the code.

## Motivation

The Defend Trade Secrets Act of 2016 (DTSA), 18 U.S.C. §§ 1836–1839, gave trade-secret owners a federal civil cause of action for misappropriation. Prior to the DTSA, trade-secret litigation was almost entirely state-law (typically the Uniform Trade Secrets Act, adopted in some form in most states). The DTSA is now the primary vehicle for cross-border and multi-jurisdiction trade-secret cases, and its remedy stack (injunctive relief, damages, exemplary damages up to 2× compensatory, attorneys' fees for willful and malicious misappropriation) is what makes it attractive to plaintiffs.

There is a catch: **18 U.S.C. § 1833(b)(3)** requires the employer to provide a specific whistleblower-immunity notice in "any contract or agreement with an employee that governs the use of a trade secret or other confidential information," entered into or updated after May 11, 2016 (the DTSA's effective date). If the notice is not provided, the employer *cannot* recover exemplary damages or attorneys' fees under § 1836(b)(3) in a DTSA action against that employee for misappropriation of a trade secret.

The notice is a single paragraph. Every startup PIIA has it (or should). And yet the omission is one of the most frequently observed defects in retroactive PIIA cleanup work, because template PIIAs drafted before 2016 do not include it and template PIIAs copied from lightweight incorporation services occasionally still do not.

## The exact statutory text

The DTSA whistleblower-immunity provision (18 U.S.C. § 1833(b)(1)–(2)) gives immunity to individuals who disclose a trade secret to (i) a federal, state, or local government official (or an attorney) solely for reporting a suspected violation of law, or (ii) in a complaint or other document filed in a lawsuit under seal. It also permits an individual who files a retaliation lawsuit against an employer to disclose the trade secret to their attorney and use the information in court proceedings, provided the individual files any documents containing the trade secret under seal and does not disclose the trade secret except pursuant to court order.

§ 1833(b)(3) — the *notice* requirement — requires the employer to provide notice of these immunities. The statute allows the notice to be provided by *cross-reference* to a policy document if the policy provides notice of the employer's reporting policy for a suspected violation of law.

The market-standard drafting integrates the notice directly into the PIIA (chapter 04). A representative form of the notice reads substantially as follows:

> **Notice of Immunity Under the Defend Trade Secrets Act of 2016.** Notwithstanding any other provision of this Agreement, you are hereby notified in accordance with the Defend Trade Secrets Act of 2016 that you will not be held criminally or civilly liable under any federal or state trade-secret law for any disclosure of a trade secret that: (i) is made (A) in confidence to a federal, state, or local government official, either directly or indirectly, or to an attorney, and (B) solely for the purpose of reporting or investigating a suspected violation of law; or (ii) is made in a complaint or other document that is filed under seal in a lawsuit or other proceeding. Additionally, if you file a lawsuit for retaliation by the Company for reporting a suspected violation of law, you may disclose the trade secret to your attorney and use the trade secret information in the court proceeding, provided that you (x) file any document containing the trade secret under seal and (y) do not disclose the trade secret, except pursuant to court order.

Substitute the corporation's name for "the Company" and adopt whichever heading style matches the surrounding document. The substance is what matters; the wording is not statutory verbatim, but it should track the immunities in § 1833(b)(1)–(2) closely enough that a court reading the notice can confirm the employee was informed of them.

## Where the notice goes

The notice must be in "any contract or agreement with an employee that governs the use of a trade secret or other confidential information." In practice, this means:

- **The PIIA / CIIAA.** Every version. Founder version. Employee version. Contractor version.
- **Any stand-alone confidentiality agreement (NDA)** with an employee (or contractor, given the DTSA's broad definition of "employee" — see below).
- **Any separation / severance agreement** that contains ongoing confidentiality obligations.
- **Any specialised trade-secret-access agreement** (e.g., access to a specific source-code repository, model weights, or customer data).

The DTSA defines "employee" broadly to include "any individual performing work as a contractor or consultant for an employer" (18 U.S.C. § 1833(b)(4)). So the notice is required in contractor confidentiality agreements as well. Do not treat "employee" as narrowly meaning W-2 workers only.

The notice can also be provided by cross-reference to a policy document (§ 1833(b)(3)(B)) — for example, the corporation's Code of Conduct or Whistleblower Policy — if that policy contains the notice. The market-standard practice is to inline the notice in every relevant agreement anyway, because the cross-reference route requires the corporation to prove the referenced policy was current, on-file, and made available at the time the agreement was signed.

## What the notice buys, and what happens without it

**With the notice:** in a DTSA action against an employee (or contractor) for misappropriation of a trade secret, the corporation is eligible to seek (i) exemplary damages up to 2× the amount of compensatory damages for willful and malicious misappropriation (§ 1836(b)(3)(C)) and (ii) attorneys' fees for willful and malicious misappropriation (§ 1836(b)(3)(D)).

**Without the notice:** the corporation *cannot* recover exemplary damages or attorneys' fees under § 1836(b)(3) against that employee (§ 1833(b)(3)(C)). Compensatory damages and injunctive relief remain available; the *enhanced* remedy stack does not. State-law claims under the Uniform Trade Secrets Act may still allow enhanced damages, subject to state-specific requirements.

The exemplary-damages and fee-shift remedies are what make DTSA litigation economically viable in cases where compensatory damages are hard to quantify (e.g., misappropriation of a trade secret whose commercial value has not yet been realised). Forfeiting them is a real cost.

## The trade-secret baseline: what makes something a "trade secret"

The DTSA (§ 1839(3)) defines a trade secret as information that:

1. The owner has taken *reasonable measures* to keep secret; and
2. Derives independent economic value from not being generally known and not being readily ascertainable through proper means.

State-law analogues (the Uniform Trade Secrets Act, adopted in most states with variations) use substantially similar language.

The "reasonable measures" requirement is where the corporation's operating hygiene matters. Courts assess whether the owner *actually treated the information as a secret*. Elements a court will look at include:

- **Written confidentiality obligations** — PIIA / NDA in place for every individual with access. (This is the PIIA's trade-secret hook, chapter 04.)
- **Access controls** — technical access limits on source code, customer data, model weights (RBAC, VPN, MFA, principle of least privilege).
- **Marking and classification** — documents labeled "Confidential"; internal policies distinguishing categories of information.
- **Onboarding and offboarding hygiene** — employees informed of confidentiality obligations on entry; access revoked and property returned on exit; exit interviews confirming return of information.
- **Vendor / partner obligations** — NDAs with third parties who receive trade-secret information.
- **Physical security** — badge access, visitor policies, laptop encryption, secure disposal.
- **Board and executive-level attention** — trade-secret protection as an operating policy, not an ad-hoc reaction to a specific incident.

The corporation that has taken zero of these steps and then sues a departed founder for trade-secret misappropriation faces a "you didn't treat it as a secret" defence and often loses on the trade-secret element before reaching the misappropriation element. The point is that the trade-secret protection is a *program*, not a lawsuit strategy — mod-109 (commercial contracts and IP) and mod-112 (enterprise risk) build out the depth. This chapter's ownership is: the PIIA and DTSA notice are the front-line trade-secret hook, and the trade-secret baseline is a corporate hygiene commitment starting at formation.

## The "reasonable measures" checklist a formation-day corporation adopts

At formation, the corporation should adopt a lightweight but real baseline:

1. **Every founder and every employee signs a PIIA on day one, including the DTSA notice.**
2. **Every contractor signs a contractor PIIA (or an IP-and-confidentiality agreement) before starting work, including the DTSA notice.**
3. **A written "confidential information" policy** in the employee handbook (mod-104 owns the handbook depth), describing what is confidential, how it is protected, and the individual's obligations.
4. **A written whistleblower policy** — separately from the DTSA notice — that gives employees a channel to report suspected violations of law without retaliation. This is a governance discipline that supports both the DTSA notice and the *Caremark* oversight duty ([chapter 06](./06-founder-conflict-of-interest.md); mod-111 has depth).
5. **Access controls on source code and confidential data.** MFA on GitHub / GitLab; SSO with automatic offboarding; least-privilege access on customer data and model weights.
6. **NDA with every vendor, partner, and prospect** who receives non-public information about the corporation's business.
7. **Board-approved intellectual-property strategy** (patents, trade secrets, open source) that documents the corporation's choices — the ownership question is board-owned, not a founder-hobby.
8. **Marking discipline** — internal documents identified as Confidential where they contain non-public information.
9. **Onboarding checklist** integrating PIIA execution, access provisioning, and confidentiality training. Offboarding checklist mirroring these with access revocation, property return, and exit-interview confirmation of ongoing obligations.

None of this is expensive at formation-day scale. All of it is expensive to retrofit at Series-B scale after a departed employee walks out with the training data.

## The DTSA remedy stack at a glance

The DTSA gives the trade-secret owner:

- **Injunctive relief** (§ 1836(b)(3)(A)) — including an order to prevent actual or threatened misappropriation, subject to state-law policies against restraints on employment.
- **Damages** (§ 1836(b)(3)(B)) — either (i) both actual loss and unjust enrichment (to the extent not covered by actual loss), or (ii) a reasonable royalty.
- **Exemplary damages** (§ 1836(b)(3)(C)) — up to 2× compensatory damages for willful and malicious misappropriation.
- **Attorneys' fees** (§ 1836(b)(3)(D)) — for willful and malicious misappropriation (as well as bad-faith claims or bad-faith motions to terminate an injunction).
- **Ex parte seizure** (§ 1836(b)(2)) — in "extraordinary circumstances," a court can order seizure of property necessary to prevent the propagation or dissemination of the trade secret. High bar; used rarely; requires specific findings.

Federal-court jurisdiction (§ 1836(c)) is a real advantage over state-court trade-secret actions in some cases.

The five-year statute of limitations (§ 1836(d)) runs from when the misappropriation is discovered or should have been discovered by the exercise of reasonable diligence.

## Interaction with state trade-secret law

The DTSA does not preempt state trade-secret law (§ 1838). A plaintiff can (and typically does) plead both DTSA and state-law trade-secret claims. The state-law claim may reach conduct that predates the DTSA's May 2016 effective date; the DTSA claim reaches conduct after that date.

State-law analogues (typically the state's version of the Uniform Trade Secrets Act) have their own notice, damages, and fee-shift regimes. Some states are more plaintiff-friendly than the DTSA on specific issues; some are less. In practice, a corporation drafts its PIIA to the DTSA standard (which includes the whistleblower notice) and relies on the same PIIA to support state-law claims.

Some states (notably California under Bus. & Prof. Code § 16600 and its 2023–2024 amendments) restrict how far post-employment confidentiality can extend into "general knowledge" the individual carries into their next role. The distinction between "confidential information" (broad; contractual) and "trade secret" (narrow; statutory) matters — post-employment obligations that reach beyond genuine trade secrets are increasingly limited. <!-- needs-research: track the current status of California AB 1076 (2023) and its amendments to Bus. & Prof. Code § 16600, and any FTC final-rule developments on non-competes, before publishing state-specific enforceability guidance. -->

## The failure modes

### The PIIA has no DTSA notice at all

Symptom: template PIIA drafted pre-2016, or copied from an incorporation service that has not updated its language.

Consequence: no exemplary damages, no attorneys' fees under DTSA § 1836(b)(3) against individuals who signed that PIIA.

Fix: adopt an updated PIIA and have every individual re-sign. New employees sign the updated PIIA on day one going forward. Because § 1833(b)(3) applies to agreements "entered into or updated" after May 11, 2016, the update itself brings the individual under the notice regime prospectively.

### The DTSA notice is in the PIIA but not in the NDA / severance

Symptom: the PIIA has the notice; a separate NDA a contractor signed does not; a departure severance agreement with a former founder does not.

Consequence: the missing-notice document is what a court reads when the disputed disclosure occurred under that document.

Fix: update every trade-secret-related agreement template (NDA, severance, specialised access agreements) to include the notice. Re-execute for individuals still in scope.

### The notice is cross-referenced to a policy that does not contain the notice

Symptom: the PIIA cross-references the corporation's "Confidentiality and Whistleblower Policy," but that policy does not contain the § 1833(b)(1)–(2) immunities.

Consequence: the cross-reference does not satisfy § 1833(b)(3)(B); the notice is effectively absent.

Fix: either (i) inline the notice in the PIIA (recommended) or (ii) update the referenced policy to contain the notice and confirm the policy was in effect at the time of PIIA execution.

### The corporation has never actually protected the trade secret

Symptom: no access controls, no marking, no onboarding / offboarding hygiene, no NDAs with vendors. A departed employee is alleged to have taken source code; the corporation sues; the defendant argues the information was not treated as a secret.

Consequence: the corporation loses on the *trade secret* element before reaching *misappropriation*. Compensatory damages and injunctive relief are unavailable regardless of the DTSA notice.

Fix: the reasonable-measures program. This is a discipline maintained forward, not a defence assembled at the last minute.

## Concrete example: the retroactive-cleanup call

An incoming COO / GC joining a 22-employee, 3-founder company at seed-to-Series-A stage reviews the corporate record. Findings:

- Founder PIIAs (all three) contain the DTSA notice. Good.
- Employee PIIAs (18 of 19 employees): 12 contain the DTSA notice; 6 use an older 2015 template that does not.
- Contractor agreements (7 individual and firm contractors): 3 contain a full PIIA with DTSA notice; 4 contain a lightweight NDA without a DTSA notice.
- The "Confidentiality Policy" in the employee handbook does not contain the § 1833(b) immunities.
- Vendor NDAs: mixed. Most contain some form of confidentiality; none contain a DTSA notice (which is not required for vendor NDAs unless the vendor is a contractor of the corporation).

The cleanup plan:

1. Adopt an updated PIIA template that contains the DTSA notice.
2. Adopt an updated Contractor Confidentiality and IP Agreement template with the DTSA notice.
3. Have every current employee and current contractor re-sign the updated agreement. Explain in the accompanying memo that this is an update to conform to a 2016 federal statute; not a change to their existing obligations.
4. Update the employee handbook's Confidentiality Policy to include the § 1833(b) immunities.
5. Provisionally treat pre-update trade-secret conduct as covered only by the older-template scope (no enhanced remedies for that period); update the compliance calendar to catch template drift going forward.
6. Add the DTSA-notice check to the standard onboarding and PIIA-execution checklist.

Cost: legal fees to update templates, a two-week roll-out to have everyone re-sign, and one board consent authorising the updated program. Downside of not doing it: forfeited exemplary damages and attorneys' fees in any future DTSA action.

## Summary

- The DTSA (18 U.S.C. §§ 1836–1839) is the federal civil cause of action for trade-secret misappropriation, with a remedy stack including exemplary damages (up to 2×) and attorneys' fees for willful and malicious conduct.
- **18 U.S.C. § 1833(b)(3)** requires a whistleblower-immunity notice in every contract or agreement with an employee (or contractor) that governs the use of a trade secret or confidential information. Without the notice, the exemplary-damages and attorneys'-fees remedies are unavailable.
- The notice is a single paragraph. Inline it in every PIIA, contractor agreement, NDA, and severance agreement that touches confidentiality. Cross-reference to a policy is technically allowed but riskier.
- A trade secret exists only if the owner has taken *reasonable measures* to keep it secret. This is a program, not a lawsuit strategy — PIIAs, access controls, marking discipline, onboarding / offboarding hygiene, board-level attention.
- Contractor agreements need the DTSA notice too — the statute's "employee" is broader than W-2.
- Retroactive cleanup for a missing DTSA notice is straightforward but real: update the template, have everyone re-sign, integrate the check into onboarding.
