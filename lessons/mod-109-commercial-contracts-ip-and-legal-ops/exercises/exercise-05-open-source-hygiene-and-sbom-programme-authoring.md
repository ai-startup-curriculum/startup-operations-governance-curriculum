# Exercise 05 — Open-source hygiene and SBOM programme authoring

> Estimated time: **~8 hours** · Related chapter: [05 — Open-source hygiene and the SBOM programme](../05-open-source-hygiene-and-sbom-programme.md)

## Problem statement

Lumen Parallax is a Series-A Delaware C-corp selling a SaaS data-analytics product into enterprise. The corporation is 60 FTE (38 engineering, 10 go-to-market, 8 product-and-design, 4 G&A), closed a $12M Series A six months ago, and ships two surfaces: a browser-delivered web application and a thin desktop installer that reaches customer data warehouses over an encrypted tunnel. The license scan the lead investor's technical-diligence vendor ran during Series A counted 480 direct and transitive open-source dependencies across the backend (Python / FastAPI / SQLAlchemy), the frontend (TypeScript / React / Vite), the desktop installer (Electron shell with a Rust bridge), and the Terraform / Helm infrastructure graph. The clean-up Lumen Parallax committed to in the Series A disclosure schedule was never finished — the head of security was hired three months post-close and inherited an open workstream rather than a closed one.

Last week a Fortune-500 procurement team pushed an in-flight $280k ACV enterprise deal into vendor-security review and sent back a questionnaire that materially raises the bar. The questionnaire demands, among forty-six other line items, (a) a current SBOM for the Service in SPDX or CycloneDX format, (b) a written OSS-approval policy and evidence it is enforced on every production build, and (c) a signed representation from the corporation that the Service contains no AGPL-licensed code. The deal is already slotted into the Q4 commit; the CRO has told the exec team the deal "cannot slip."

The head of security pulled the SBOM-request through the engineering team's existing CI vulnerability scanner and discovered the four live problems the OSS programme now has to resolve on the record:

- A direct dependency published under **AGPL v3** — a browser-side visualisation library a staff engineer added into a six-week customer POC in late 2024 and that shipped unchanged into the production bundle when the POC became a feature. The library is called from the frontend build and its minified output is served to every logged-in user.
- Two direct dependencies published under **LGPL v3** — a numerical routines library and an audio-decoding library — both **statically linked** into the Rust bridge inside the desktop installer. Neither ships the LGPL § 4 object-code-relink mechanism the LGPL would otherwise require for static linking.
- Three **Apache License 2.0** libraries present as direct dependencies but missing from the `NOTICE` file the product currently ships. Two were added since the last manual NOTICE-file refresh; one has been missing since the Series-Seed codebase.
- Seventeen **transitive dependencies with license-ambiguous metadata** — missing SPDX identifiers in the package manifest, GitHub repositories without a `LICENSE` file at the root, or `LICENSE` files that reference a license by name without reproducing the license text. The CI vulnerability scanner flags them as "unknown" rather than mapping them to the OSS-approval tier policy.

The head of security has eight weeks to publish the full OSS programme, remediate the four live findings, and send the Fortune-500 questionnaire response under signature of the general counsel. The head of security has an engineering-lead counterpart, a general counsel who joined four months ago, and a $0 incremental tooling budget until the Series B — any paid tool recommended must either fit within the existing engineering-tools line or be routed through the CFO.

## Requirements

### Part A — OSS-approval tier policy

Author the operative tier policy Lumen Parallax will publish as the corporation's OSS-approval instrument. Draft the operative text, not a summary. Cover:

1. **Permissive tier** — default-approved. Enumerate MIT, BSD 2-Clause, BSD 3-Clause, Apache License 2.0, and ISC by name. For Apache 2.0 specifically, name the three obligations the policy preserves: the § 4 `NOTICE`-file propagation requirement, the § 3 express patent-license grant and its patent-litigation termination consequence, and the retention of copyright / patent / trademark notices through the build chain.
2. **Weak-copyleft tier** — approved with named architectural constraints. For LGPL v2.1 and LGPL v3, name the dynamic-linking-only discipline and the specific failure mode (static linking triggers the copyleft obligation absent the § 4 relink mechanism). For MPL 2.0, name the file-boundary discipline that keeps the copyleft trigger scoped to MPL-licensed files. For EPL 2.0, name the module-boundary discipline and the sign-off step before adoption.
3. **Strong-copyleft tier** — prohibited for shipped-binary and SaaS-backend use. GPL v2 and GPL v3 are disapproved for the production product. **AGPL v3 is prohibited outright**; name the § 13 network-use trigger as the specific reason and explain, in plain language a staff engineer can read, why the SaaS deployment pattern fires the trigger even for internal-user-facing surfaces.
4. **Non-OSI and source-available licenses** — treated as commercial licenses, not open source. Name BUSL, SSPL, Elastic License v2, Confluent Community License, and Redis Source Available License explicitly; name the default-deny posture on hand-drafted / non-standard licenses.
5. **Exception process.** The written path for case-by-case approval of a disapproved-tier component — who requests, who reviews, who signs, and the discipline that an exception is a documented architectural decision rather than an informal manager grant. Name whether general counsel is the first stop or whether external IP counsel is retained for an AGPL / GPL exception review.
6. **Enforcement linkage.** The CI build-time enforcement path that fails a build on introduction of a prohibited-tier license, and the review cadence for the approved component inventory.

### Part B — License-compliance-tooling selection memo

Author the selection memo the head of security will route to the CFO and the general counsel. Evaluate **FOSSA, Snyk Open Source, Black Duck, Tidelift, and GitHub Advanced Security (Dependabot + CodeQL)** against the following named criteria and arrive at a specific pick with named justification:

1. **SBOM output format support.** SPDX (ISO/IEC 5962:2021) and CycloneDX (OWASP) at minimum; name whether both are supported and in which encodings.
2. **In-repo CI integration.** Native GitHub Actions / build-tool integration; emit results in a machine-readable format; fail-build-on-policy-violation mechanic.
3. **Transitive-dependency resolution with license inference for unlabelled components.** The specific posture each tool takes on the seventeen license-ambiguous transitive dependencies in the problem statement.
4. **Policy-enforcement mechanic.** Configurable approved / disapproved / requires-review list at the license level, with per-component overrides, and audit-log evidence sufficient for enterprise procurement and Series-B diligence.
5. **Automated SBOM generation.** Per-build SBOM artefact, with timestamping and the ability to retain the SBOM alongside the release.
6. **Container-image / lockfile / go-module coverage.** The specific ecosystem coverage each tool offers against Lumen Parallax's stack (Python / pip, TypeScript / npm, Rust / cargo, Electron, Terraform / Helm, container images).
7. **Pricing posture.** Flag any specific vendor pricing with `<!-- needs-research: ... -->` — do not invent dollar figures or current-year pricing tiers. Name the pricing axis (per-developer, per-repo, per-SBOM-artefact, subscription-with-support) each tool bills on and the posture Lumen Parallax takes toward the $0 incremental budget.

The memo ends with a specific pick, a one-paragraph justification against the criteria, and the fallback option if the CFO denies the budget request.

### Part C — SBOM production workflow

Author the written SBOM production workflow Lumen Parallax will publish and operate against. Cover:

1. **Output format.** The choice between SPDX 2.3 (or the current SPDX version at authoring time — flag the version with `<!-- needs-research: ... -->` if the current version has moved) and CycloneDX, and the choice to emit one or both. Name the format the enterprise-customer-facing deliverable is published in.
2. **Component-identifier scheme.** The choice among purl (Package URL), CPE, and SWID for component identification; name the scheme the SBOM uses as its primary identifier and the fallback scheme for components the primary cannot resolve.
3. **Production trigger.** Per-release SBOM generation vs. continuous (per-commit / per-build) generation. Name the trigger Lumen Parallax adopts and the retention posture for superseded SBOMs.
4. **Delivery mechanic.** The pattern by which an enterprise customer obtains the current SBOM — a signed URL, a vendor-security-portal (Vanta / Drata / SafeBase / similar), a Trust Center page, or an MSA deliverable. Name the pattern Lumen Parallax adopts and the authentication posture (public vs. NDA-gated vs. customer-only).
5. **Retention posture.** How long SBOM artefacts are retained, where (S3 with versioning, a signed-artefact store, the vendor-portal data store), and the audit-log evidence posture.
6. **NTIA / OMB / EO alignment.** Name alignment with the NTIA "Minimum Elements for a Software Bill of Materials" (supplier name, component name, version, unique identifier, dependency relationships, author of SBOM data, timestamp), OMB M-22-18 / M-23-16, and Executive Order 14028 § 4(e)–(k). Flag the current status of the CISA Secure Software Development Attestation Form with `<!-- needs-research: ... -->` — do not state the current filing-deadline posture from memory.
7. **Vulnerability-data posture alongside the SBOM.** The role of VEX (Vulnerability Exploitability eXchange) and VDR (Vulnerability Disclosure Report) alongside the SBOM; whether Lumen Parallax ships a VEX statement with the SBOM or on request; the linkage to [mod-112](../../mod-112-security-review-and-vulnerability-management/) for the vulnerability-management workstream that operates against the same SBOM.

### Part D — Outbound-contribution and corporate-open-source-release policy

Author the written policy covering what Lumen Parallax employees contribute back to upstream OSS projects and what the corporation releases as its own open source. Cover:

1. **Approval workflow for employee contributions.** Who approves (engineering-lead for routine, engineering-lead + general counsel for substantive), the triage SLA (acknowledge within N business days; decide within M business days — name specific numbers), and the lightweight path for typo / small bug fixes.
2. **IP-assignment interaction with the PIIA.** The policy references the employee PIIA ownership chain but defers the PIIA mechanics to [mod-103](../../mod-103-employment-law-and-contract-design/) and [mod-102](../../mod-102-founding-team-legal-architecture/); name the deferral explicitly and name the chain-of-title interaction with [chapter 04](../04-ip-protection-strategy.md).
3. **Trademark-and-brand review.** The review step a corporate open-source release passes through before public launch — name the project-name trademark check, the logo review, and the trademark-use policy the released project publishes.
4. **CLA vs. DCO posture.** The corporation's posture on which mechanism it accepts for inbound contributions to its own released projects (DCO for lightweight, CLA for strategic; name the Apache ICLA / CCLA framework by name) and the authority to sign CLAs on the corporation's behalf when contributing outbound.
5. **License-selection framework for corporate releases.** Apache License 2.0 as the default; the specific justification required for any copyleft release; the decision rule for MIT vs. Apache 2.0 on small utility projects.

### Part E — Enterprise OSS-warranty position in the MSA

Author the OSS-warranty operative language the corporation takes into the customer MSA, deferring the broader MSA architecture to [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md). Cover:

1. **Warranty-of-non-infringement posture.** The operative text for the no-copyleft-contamination warranty and the license-compliance warranty; the SBOM-availability undertaking.
2. **Knowledge qualifier.** The "to the knowledge of corporation's authorised personnel" qualifier, named authorised personnel, and the diligence posture the knowledge qualifier assumes.
3. **Carve-outs.** The carve-outs the warranty does not cover — customer modifications, open-source components provided by the customer for the corporation to incorporate at customer direction, combinations with third-party components outside the corporation's control.
4. **Indemnity interaction.** Name whether the IP-indemnity clause (see [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md)) carves out OSS claims or covers them, and the pricing posture Lumen Parallax takes toward that choice given the internal-programme strength coming out of Parts A–D.

### Part F — Resolution of the four live dependency findings

Author the written remediation plan the head of security will route to the engineering lead and the general counsel. For each of the four findings, specify a named remediation action and a timeline the Fortune-500 questionnaire response can honestly cite:

1. **The AGPL v3 direct dependency** (frontend visualisation library). Name the remediation — remove and re-architect against a permissive-tier equivalent, replace with a named permissive alternative, or (as a documented exception) commit to source-disclosure under § 13. Name the engineering-week estimate, the responsible engineer, and the completion date before the questionnaire response is signed.
2. **The two LGPL v3 statically-linked dependencies** inside the desktop installer. Name the remediation — re-link dynamically with the § 4 relink mechanism, ship object-code-plus-relink per § 4, replace with permissive-tier equivalents, or (if the specific library has no permissive equivalent) document the architectural review and the LGPL compliance path. Name the engineering-week estimate and the completion date.
3. **The three Apache 2.0 libraries missing from the NOTICE file.** Name the remediation — add the libraries to the `NOTICE` file, publish the updated file through the product-release pipeline, and name the audit step that confirms NOTICE propagation on every subsequent release. This is the lowest-effort finding; do not over-engineer.
4. **The seventeen license-ambiguous transitive dependencies.** Name the remediation path for each sub-category — upstream a `LICENSE` file PR to the dependency's source repository, add a SPDX identifier to the package manifest via upstream PR, replace with a license-labelled permissive equivalent, defensively publish the corporation's understanding of the license as a documented decision pending upstream clarification, or route to counsel. Name the triage posture — which sub-category is handled by the engineering team unilaterally and which routes through the general counsel.

The remediation plan ends with a completion-date table and the specific date the Fortune-500 questionnaire response can honestly state the four findings are resolved as of.

### Part G — Fortune-500 questionnaire response

Author the operative language Lumen Parallax will send to the Fortune-500 procurement team under general-counsel signature. Cover:

1. **The signed representation on the AGPL question.** The exact representation text, drafted to be accurate as of a stated remediation date (from Part F), with a knowledge qualifier that reflects the actual diligence posture the OSS programme supports.
2. **The current SBOM link.** The delivery mechanic from Part C (signed URL, portal, Trust Center page) and the format the SBOM is delivered in; name the authentication posture the customer will encounter.
3. **The OSS-approval policy summary.** A one-paragraph summary of the Part A policy with a link to the full policy published through the Trust Center; the auditable-enforcement claim and the evidence the corporation can produce on request.
4. **The ongoing-compliance commitment.** The written commitment to continuous SBOM generation, policy enforcement on every build, and notification posture if a prohibited-tier license is subsequently introduced.
5. **The gaps the questionnaire response does not represent to.** The questionnaire asks forty-six questions; the OSS programme answers four of them. Name the explicit scope limit of the response and the handoff to the broader security-review workstream in [mod-112](../../mod-112-security-review-and-vulnerability-management/).

## Starter guidance

- Chapter 05 is the primary reference. The three-tier license taxonomy (permissive, weak copyleft, strong copyleft), the SBOM-format landscape (SPDX, CycloneDX, SWID), the NTIA minimum elements, EO 14028 § 4(e)–(k), and OMB M-22-18 are reproduced in chapter 05; do not re-derive the law from first principles.
- The four live findings are the forcing function on Parts F and G. Ducking any one of them — deferring the AGPL dependency to "Series B," claiming the LGPL static linking is "probably fine," or treating the NOTICE-file gap as not-a-finding — is a fail.
- Chapter 05 names FOSSA, Tidelift, Snyk, Black Duck, Mend, and Sonatype Nexus IQ as the commonly-evaluated tools. The exercise names a sub-set (FOSSA, Snyk Open Source, Black Duck, Tidelift, GitHub Advanced Security). Evaluate against the named criteria; do not import unlisted tools without naming them.
- Any specific vendor pricing figure, current-year pricing tier, or current-year EO / OMB / NIST memo version gets `<!-- needs-research: ... -->` — propagate the discipline from chapter 05's handling of the CISA attestation-form status.
- The IP chain-of-title mechanics that touch open-source-release decisions live in [chapter 04](../04-ip-protection-strategy.md); reference the chain-of-title discipline where Part D interacts with it, do not re-author it.
- The MSA architecture lives in [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md); Part E owns only the OSS-warranty position inside the MSA, not the MSA's cap-and-indemnity structure.
- The employee PIIA mechanics that underpin the outbound-contribution policy's IP-assignment claim live in [mod-103](../../mod-103-employment-law-and-contract-design/) and [mod-102](../../mod-102-founding-team-legal-architecture/); defer the mechanics and reference the deferral in Part D.
- The vulnerability-management workstream that operates against the same SBOM lives in [mod-112](../../mod-112-security-review-and-vulnerability-management/); Part C's VEX / VDR posture references the deferral.
- Do not invent real peer company names. Chapter 05's concrete example uses "Acme Robotics" as a hypothetical; follow the pattern and treat Lumen Parallax as the only named corporation in the authoring package.
- Do not plagiarise the GitHub `NOTICE` file of an actual permissively-licensed project; draft the NOTICE-propagation discipline in Part F as a workflow, not as a verbatim third-party notices file.

## Deliverables

- `oss-approval-policy.md` — Part A.
- `tooling-selection-memo.md` — Part B.
- `sbom-production-workflow.md` — Part C.
- `outbound-contribution-policy.md` — Part D.
- `msa-oss-warranty-position.md` — Part E.
- `remediation-plan.md` — Part F.
- `fortune-500-questionnaire-response.md` — Part G.

## Acceptance criteria

The package is acceptable if:

1. Part A's tier policy is operative text (not a summary), names MIT / BSD 2-Clause / BSD 3-Clause / Apache 2.0 / ISC in the permissive tier with the Apache 2.0 § 3 patent grant and § 4 NOTICE propagation obligations named, names LGPL v2.1 / v3 / MPL 2.0 / EPL 2.0 in the weak-copyleft tier with the dynamic-linking / file-boundary / module-boundary disciplines named, prohibits GPL v2 / v3 / AGPL v3 for shipped product with the AGPL § 13 network-use trigger explained in plain language, and treats BUSL / SSPL / Elastic License v2 / Confluent Community License / Redis Source Available License as commercial licenses.
2. Part A names a specific exception process (requester, reviewer, signer) and an auditable CI-side enforcement linkage; a "requires engineering judgement" formulation without named sign-off is unacceptable.
3. Part B evaluates each of FOSSA, Snyk Open Source, Black Duck, Tidelift, and GitHub Advanced Security against the seven named criteria, arrives at a specific pick with named justification, names the fallback option, and flags all specific pricing with `<!-- needs-research: ... -->`.
4. Part C names the output format (SPDX, CycloneDX, or both), the component-identifier scheme (purl / CPE / SWID), the production trigger, the delivery mechanic to enterprise customers, the retention posture, and names alignment with NTIA minimum elements, OMB M-22-18 / M-23-16, and EO 14028 § 4(e)–(k) — with current-year memo versions and CISA attestation-form status flagged `<!-- needs-research: ... -->`.
5. Part C names the posture on VEX and VDR alongside the SBOM, and references [mod-112](../../mod-112-security-review-and-vulnerability-management/) for the vulnerability-management workstream that operates against the SBOM.
6. Part D's outbound policy names the approval workflow with triage SLA, defers the PIIA mechanics to [mod-103](../../mod-103-employment-law-and-contract-design/) and [mod-102](../../mod-102-founding-team-legal-architecture/) and references [chapter 04](../04-ip-protection-strategy.md) for the IP chain-of-title interaction, names the trademark-and-brand review step, names the CLA vs. DCO posture (with the Apache ICLA / CCLA framework named), and names the license-selection default (Apache 2.0 or MIT, with justification required for any copyleft release).
7. Part E's MSA OSS-warranty position names the no-copyleft-contamination warranty, the license-compliance warranty, the SBOM-availability undertaking, the knowledge qualifier with authorised personnel named, the specific carve-outs, and the IP-indemnity-interaction posture — deferring the broader MSA architecture to [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md).
8. **Part F names a specific remediation action, a specific responsible engineer or team, an engineering-effort estimate, and a specific completion date for each of the four live findings (AGPL direct dependency, LGPL static linking, Apache 2.0 NOTICE gap, license-ambiguous transitive dependencies).** A generic "we will address these findings" without the per-finding specifics is unacceptable.
9. Part G's questionnaire response includes a signed representation on the AGPL question accurate as of a stated remediation date, a current SBOM link, a one-paragraph OSS-approval-policy summary, an ongoing-compliance commitment, and an explicit scope-limit statement that names the handoff to [mod-112](../../mod-112-security-review-and-vulnerability-management/) for the broader security-review workstream.
10. Any specific vendor pricing figure, current-year pricing tier, current-year EO / OMB / NIST memo version, and current-year CISA attestation-form status is flagged `<!-- needs-research: ... -->`. No real peer company names are invented; nothing is left as `[TBD]` or `[FILL IN]`.
11. Deferrals to sibling modules and chapters are named explicitly where the chapter 05 ownership boundary assigns the mechanic elsewhere — [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md) for the MSA architecture, [chapter 04](../04-ip-protection-strategy.md) for the IP chain-of-title, [mod-102](../../mod-102-founding-team-legal-architecture/) and [mod-103](../../mod-103-employment-law-and-contract-design/) for the PIIA mechanics, and [mod-112](../../mod-112-security-review-and-vulnerability-management/) for the vulnerability-management workstream.
12. The package reads as a coherent eight-week programme the head of security can walk the general counsel and the CFO through, not as seven disconnected documents; the completion-date table in Part F and the stated-remediation-date representation in Part G reconcile.
