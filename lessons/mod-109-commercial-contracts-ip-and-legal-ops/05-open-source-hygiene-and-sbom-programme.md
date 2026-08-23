# 5. Open-source hygiene and the SBOM programme

> Every modern software product is 80–95% third-party open source by line count. Which open-source components are inside the product, under which licenses, and with which known vulnerabilities is now a first-order diligence question — for enterprise procurement, for federal-agency sales, and for every Series-A / B investor's technical diligence workstream. The SBOM is how the corporation answers that question, and the OSS-approval policy is how it stays out of trouble in the first place.

## Motivation

Open-source software governance sits at the intersection of licensing law, product architecture, procurement, and security. It matters for four independent reasons, each of which is enough on its own to justify a written programme:

1. **License compliance is a legal-risk topic.** Copyleft licenses (GPL v2, GPL v3, AGPL v3) require that if the corporation *distributes* a work that is a derivative of GPL-licensed code, it must license the combined work under the same terms — which for a proprietary SaaS or shipped-binary product would mean open-sourcing the corporation's own source code. AGPL v3 § 13 extends this trigger to network use ("interacting with users remotely through a computer network"), which is why AGPL is on the "do not use" list for most commercial SaaS. Violating a copyleft license is a copyright infringement claim with statutory damages (17 U.S.C. § 504) and injunction risk.

2. **Series-A / B investor diligence.** Institutional investors' technical / legal diligence workstreams routinely run a license scan of the corporation's codebase (via FOSSA, Black Duck, Snyk, or similar) as part of the pre-investment checklist. Discovering a GPL v3 dependency shipped into a proprietary product mid-diligence is a deal-slowing (occasionally deal-killing) surprise. Presenting a clean SBOM and a written OSS-approval policy on day one of diligence shortens the workstream.

3. **Enterprise procurement now asks for the SBOM.** Fortune-500 procurement questionnaires — even absent any federal-contract flow-down — increasingly include: "Provide a software bill of materials for the Service in SPDX or CycloneDX format." The corporation without an SBOM programme fails the vendor-security review or delays it while it manually assembles one.

4. **Federal contracts require the SBOM.** Executive Order 14028 (May 12, 2021), *Improving the Nation's Cybersecurity*, § 4(f) directs NIST to publish guidelines for software supply-chain security and § 4(k) requires that federal software vendors comply with the resulting standards, including "providing a purchaser a Software Bill of Materials (SBOM) for each product." OMB M-22-18 (September 14, 2022) implements this for agency procurement of software. If the corporation sells to federal agencies (directly or through a system integrator on flow-down terms), the SBOM is not optional.

This chapter treats the OSS programme in three parts: (i) the license taxonomy and its go-to-market implications, (ii) the SBOM requirement and its tooling, and (iii) the outbound-contribution and corporate-open-source-release policy. It closes with the customer-facing OSS warranty in the MSA (the mirror on the customer side of the corporation's own hygiene), the standard failure modes, and a concrete Series-A example.

## The OSI-license taxonomy: permissive, weak copyleft, strong copyleft

The Open Source Initiative (OSI) maintains the list of OSI-approved licenses (currently ~100). For practical governance purposes, the corporation's approval policy should sort them into three tiers.

### Permissive licenses — safe to combine with proprietary code

- **MIT License** — the shortest and most permissive of the widely-used licenses. Obligations: reproduce the copyright notice and license text in copies or substantial portions.
- **BSD 2-Clause ("Simplified BSD")** and **BSD 3-Clause ("New BSD" / "Modified BSD")** — attribution + license text. The 3-clause variant adds a no-endorsement clause (may not use the name of the licensor to endorse derived products without permission).
- **Apache License 2.0** — attribution, license text, retention of copyright / patent / trademark notices, and a NOTICE-file propagation requirement (§ 4). Two additional features that matter for commercial use:
  - Express patent-license grant (Apache 2.0 § 3): each contributor grants to recipients a perpetual, worldwide, royalty-free patent license for the contribution.
  - Patent-litigation termination (Apache 2.0 § 3): if a recipient sues alleging that the Apache-licensed work or a contribution embodied within it infringes a patent, the recipient's patent license under Apache 2.0 terminates.
- **ISC License** — functionally equivalent to a simplified MIT / BSD; attribution and license text.

**Go-to-market implication.** Permissive licenses can be freely combined with proprietary code, incorporated into a distributed binary, run in a SaaS backend, and modified without triggering source-disclosure obligations. The obligations are (a) attribution — reproduce the copyright notice and license text in the product's third-party-notices file — and (b) for Apache 2.0, propagate the NOTICE file per § 4 and honour the § 3 patent-termination consequence. Permissive licenses are the default-approved tier.

### Weak-copyleft licenses — require architectural care

Weak copyleft imposes source-disclosure obligations on the *licensed files themselves* or on a defined *module* / *library* boundary, but does not extend the disclosure obligation to code that merely uses or links to the licensed component in an approved manner.

- **LGPL v2.1 / v3 (GNU Lesser General Public License).** The LGPL is designed so that a proprietary program can *dynamically link* to an LGPL library without the proprietary program itself becoming subject to LGPL. LGPL v3 §§ 3–4 permit combined works if (i) the LGPL library is used unmodified or with modifications made under LGPL, (ii) the combined work displays LGPL notices and provides a copy of the LGPL, and (iii) the combined work either uses dynamic linking or provides object code / a mechanism for the user to relink against a modified LGPL library. **Static linking of LGPL code into a proprietary binary generally triggers the copyleft obligation** (because the user cannot substitute a modified LGPL library without the source of the proprietary side), and is the failure mode.
- **MPL 2.0 (Mozilla Public License).** File-level copyleft. Modifications *to MPL-licensed files* must themselves be MPL. Files that are *not* MPL-licensed can be combined with MPL files in a larger work and remain under whatever license they were originally under. This is the practitioner-friendly copyleft: it protects the community's shared files without contaminating adjacent proprietary code, provided the file boundary is respected.
- **EPL 2.0 (Eclipse Public License).** Module-level copyleft — closer in spirit to LGPL than to MPL. Modifications to EPL-licensed modules must be EPL; new modules that merely interact with EPL modules through defined interfaces can be under other licenses.

**Go-to-market implication.** Weak copyleft is workable in a commercial product provided the corporation understands and enforces the boundary — dynamic linking for LGPL, file boundary for MPL, module boundary for EPL — and is willing to publish modifications to the copyleft components. The approval policy should permit LGPL and MPL 2.0 with a documented linkage / file-boundary requirement, and require sign-off before adopting an EPL component.

### Strong-copyleft licenses — architectural constraint or outright ban

- **GPL v2 (GNU General Public License).** Distribution of a work "based on" the GPL'd program requires that the whole combined work be licensed under GPL v2. "Based on" is broad — static or dynamic linking, incorporation of GPL headers, and derivative works in the copyright sense all qualify under FSF's interpretation and the prevailing case-law framing.
- **GPL v3.** GPL v3 § 5 preserves the strong-copyleft trigger for conveyance (distribution) of covered works, adds explicit anti-Tivoization and patent-termination language, and clarifies system-library exclusions. Same practical effect for the corporation: shipping GPL v3 code inside a distributed proprietary product requires GPL-licensing the combined work.
- **AGPL v3 (GNU Affero General Public License).** AGPL v3 § 13 extends the copyleft trigger to *network use*: if the corporation modifies AGPL-licensed code and makes it available over a network (which is how every SaaS product exposes its backend), it must offer the corresponding source code to the network users of that modified version. AGPL was designed specifically to close the "SaaS loophole" in GPL, and its trigger fires in the operating environment of every hosted service — which is why AGPL is on the "do not use" list for commercial SaaS unless the corporation is willing to open-source the affected component.

**Go-to-market implication.** Strong copyleft is incompatible with proprietary distribution unless the corporation is deliberately choosing to build in the open on top of the GPL'd component (a legitimate strategy but a whole-product choice, not a per-dependency one). The default approval policy for a commercial SaaS or shipped-binary corporation is: GPL v2, GPL v3, AGPL v3 are **disapproved**; adopting any of them requires a written architectural review and (for AGPL) a specific commitment to source-disclosure compliance.

### The "non-OSI" and dual-licensed hazards

Beyond the OSI-approved list, the corporation encounters non-OSI licenses that superficially look open but impose commercial-use restrictions the OSS-approval policy typically forbids:

- **"Source-available" licenses** — Business Source License (BUSL), Server Side Public License (SSPL), Elastic License v2, Confluent Community License. These are *not* OSI-approved and may forbid the exact commercial use the corporation intends (typically, running the software as a managed service). They should be reviewed as commercial licenses, not open source.
- **Dual-licensed projects** — a project offered under both GPL and a commercial license (MySQL under GPL v2 or Oracle commercial; Qt under LGPL or commercial). The corporation must choose which license it takes the software under and comply with that license; picking GPL v2 and treating it as "just open source" is the failure mode.
- **Custom / non-standard licenses** — hand-drafted licenses on niche packages that have never been reviewed by counsel. The approval policy should default-deny non-standard licenses.

## The SBOM requirement and the federal timeline

### Executive Order 14028 and its implementing guidance

Executive Order 14028 was issued May 12, 2021 in response to the SolarWinds and Colonial Pipeline incidents. § 4 (*Enhancing Software Supply Chain Security*) directs a series of NIST, NTIA, and OMB actions:

- § 4(e) directs NIST to publish guidelines identifying practices that enhance software supply-chain security, incorporating existing standards (the resulting document is NIST SP 800-218, *Secure Software Development Framework (SSDF)*).
- § 4(f) directs NTIA to publish minimum elements for an SBOM.
- § 4(k) requires that agencies procuring software require the seller to attest to conformance with the § 4(e) guidelines and to provide an SBOM.

**NTIA "Minimum Elements for a Software Bill of Materials"** (July 12, 2021) establishes the baseline data fields every SBOM must contain: supplier name, component name, version, unique identifiers, dependency relationships, author of the SBOM data, and timestamp. Plus practices around SBOM automation, depth, and known unknowns.

**OMB M-22-18** (September 14, 2022), *Enhancing the Security of the Software Supply Chain through Secure Software Development Practices*, implements EO 14028 for federal agency software procurement. Agencies must obtain a self-attestation from software producers that the producer follows the SSDF, and may require an SBOM and other artifacts.

<!-- needs-research: verify the current status of the CISA Secure Software Development Attestation Form and the timeline for federal-agency SBOM ingestion requirements (which have been extended multiple times) -->

The practical upshot for a corporation selling software to (or through a prime that sells to) a federal agency: expect to sign the CISA attestation form, expect to produce an SBOM on request, and expect the SBOM to be a machine-readable file in one of the three recognised formats below.

### SBOM formats

Three formats dominate; each is machine-readable and covers the NTIA minimum elements plus extensions.

- **SPDX (Software Package Data Exchange).** Originated at the Linux Foundation; standardised as **ISO/IEC 5962:2021**. Rich metadata model including licensing information, security references, and package relationships. Emitted as tag-value, JSON, YAML, or RDF/XML.
- **CycloneDX.** OWASP project. Designed with a security-and-supply-chain focus; supports vulnerability data (VEX — Vulnerability Exploitability eXchange), pedigree, and services alongside components. JSON or XML. Widely adopted in the security-tooling ecosystem.
- **SWID (Software Identification Tags).** **ISO/IEC 19770-2**. More common in enterprise asset-management contexts than in developer-facing supply-chain tooling.

For a commercial software corporation, the practical choice is **CycloneDX** (developer-toolchain default, best vulnerability-data integration) or **SPDX** (broader license-metadata coverage, ISO-standardised). Many corporations generate both. Choice of format is usually driven by the tooling the corporation adopts.

### The enterprise-customer SBOM ask

Even outside federal-contract flow-down, Fortune-500 procurement / vendor-security questionnaires now routinely include an SBOM question. The pattern is:

- "Provide an SBOM for the Service in SPDX or CycloneDX format."
- "Describe how the SBOM is updated on each release."
- "Describe how the corporation monitors known vulnerabilities against components in the SBOM."
- "Provide a VEX (Vulnerability Exploitability eXchange) statement for any CVEs identified against the SBOM components."

A corporation without an SBOM programme cannot answer these questions credibly and either fails vendor security review (and the deal) or spends weeks manually reconstructing one. See [mod-112 SecReview](../../mod-112-security-review-and-vulnerability-management/) for the parallel security-review workstream that operates against the same SBOM.

## License-compliance and SBOM tooling

The tooling market for license scanning and SBOM generation is well-established. The evaluation dimensions are the same across vendors:

- **Language / ecosystem coverage.** JavaScript / npm, Python / pip / poetry, Java / Maven / Gradle, Go modules, Rust cargo, C / C++, Ruby, PHP, .NET / NuGet, Swift, Kotlin, and container images. Coverage gaps translate to blind spots in the SBOM.
- **License-detection accuracy.** Ability to detect the license from package metadata, from LICENSE / COPYING files in the source tree, and from license headers in individual source files.
- **False-positive rate.** Distinguishing a genuine license issue from a policy-configurable non-issue.
- **Policy-configuration granularity.** Ability to define an approved / disapproved / requires-review list at the license level, with per-component overrides.
- **CI / build-tool integration.** Ability to run in CI, fail a build on policy violation, and emit results in a machine-readable format.
- **SBOM output format support.** SPDX and CycloneDX at minimum.
- **Vulnerability-data sources.** NVD (National Vulnerability Database), GHSA (GitHub Security Advisories), OSV, vendor-specific advisories, and proprietary curation.
- **Remediation guidance.** Suggested upgrade paths, backported fixes, patch availability.

The commonly-evaluated tools:

- **FOSSA** — license-and-vulnerability scanning; strong CI integration; SPDX / CycloneDX output.
- **Tidelift** — subscription model that includes commercial support / indemnification for a curated set of packages; useful adjunct to a license-scanning tool.
- **Snyk (Snyk Open Source)** — developer-first workflow; strong ecosystem coverage; integrated with vulnerability scanning across the Snyk suite.
- **Black Duck (Synopsys, now part of Sonatype).** Enterprise-grade with deep license-detection catalogue; historically the incumbent in regulated / large-enterprise contexts.
- **Mend (formerly WhiteSource)** — similar scope to Snyk / Black Duck; policy-driven remediation.
- **Sonatype Nexus IQ** — component-lifecycle policy management, integrated with Nexus Repository.

The selection is a CTO-adjacent decision — see the parallel cto-curriculum treatment of SBOM tooling implementation for the engineering-side evaluation and CI wiring. From the legal-ops side, the requirements are: SPDX or CycloneDX output, configurable license policy that maps to the corporation's approved / disapproved list, and audit-log evidence sufficient to demonstrate to an enterprise procurement team or a Series-A diligence workstream that the policy is enforced on every build.

## The outbound-open-source-contribution policy

The inbound-license policy governs what the corporation *ingests*. The outbound-contribution policy governs what the corporation's employees *contribute back* to third-party projects and what the corporation *releases* as its own open source.

### Employee contributions to third-party projects

The PIIA ([mod-103 chapter 04](../mod-103-employment-law-and-contract-design/04-employee-piia.md)) assigns all IP the employee creates within the scope of employment to the corporation. Absent a written outbound-contribution policy, an employee contributing a patch to an upstream open-source project during the workday is potentially assigning corporation-owned IP to that project — which is exactly what the corporation wants when it is contributing back, but which requires an explicit policy so that (i) the employee has clear authorisation, (ii) the corporation's copyright ownership is disclosed, and (iii) the contribution flows through the project's contributor-license mechanism cleanly.

The written outbound policy typically addresses:

- **Approved license list for contributions.** The corporation approves contributions to projects under licenses on the inbound-approved list (permissive and weak copyleft). Contributions to GPL / AGPL projects require case-by-case sign-off.
- **Copyright ownership.** The corporation owns the copyright in the contribution (per the PIIA). The contribution is authorised to be licensed under the target project's license.
- **Attribution.** The contribution should be attributed to the corporation (either via the corporate email address in the commit / sign-off, or via an explicit copyright header where the project convention supports it).
- **Time treatment.** Whether contributions during work hours are treated as billable time-in-lieu or as off-the-clock. Most corporations that value upstream contribution treat aligned contributions as on-the-clock work.
- **Approval workflow.** Manager / engineering-lead approval for substantive contributions; a lightweight process for typo fixes and small bug fixes.

### CLAs and the DCO

Third-party projects use one of three mechanisms to accept contributions:

- **Individual CLA (Contributor License Agreement).** The individual contributor signs a CLA that grants the project (or its steward foundation) the rights it needs to accept and redistribute the contribution. The **Apache Software Foundation Individual CLA (ICLA)** is the widely-used template — copyright license + patent license from the contributor.
- **Corporate CLA (CCLA).** The corporation signs a corporate CLA that grants the project the rights and authorises a list of named individuals to make contributions on the corporation's behalf. The **Apache Corporate CLA** is the standard. The Apache CCLA is what a corporation whose employees contribute to Apache projects (or projects that use the Apache CLA framework) executes.
- **Developer Certificate of Origin (DCO).** A lightweight alternative to a CLA — the contributor certifies via a `Signed-off-by:` line in the commit message that they have the right to submit the contribution under the project's license. The Linux kernel uses DCO; many projects have moved to DCO to reduce onboarding friction.

The corporation's outbound-contribution policy should identify who is authorised to sign CLAs on the corporation's behalf (per the delegation-of-authority policy — see [chapter 09 boundary map](./09-legal-boundary-map.md)) and should maintain a list of the CLAs the corporation has signed (so that a project-level dispute can be traced back to the governing CLA).

### Releasing the corporation's own open source

A separate decision from "should our employees contribute upstream" is "should we release something we built as open source?" The strategic reasons (community-building, standards influence, hiring signal, commoditising a complement) are outside this chapter's scope; the legal / governance choices are:

- **Choice of license.** For most corporate-released projects, **MIT** or **Apache License 2.0** are the practitioner-standard defaults. Apache 2.0 is preferred when the project involves patent-relevant technology (because of the express § 3 patent grant and termination — the corporation wants both the outbound patent license and the reciprocity of the termination clause). MIT is preferred when the project is small and the simplicity is valuable.
- **Governance.** For a project the corporation intends to keep as its own artefact, a benevolent-dictator model (the corporation appoints maintainers) is standard. For a project the corporation intends to become a community standard, a steering-committee or foundation model (Linux Foundation, CNCF, Apache Software Foundation) is more appropriate; foundation stewardship also solves the CLA / patent-pool / trademark issues.
- **CLA vs. DCO for inbound contributions to the released project.** DCO is lower-friction and increasingly the norm; CLA (with an Apache-style ICLA / CCLA) is more protective and standard for larger / more-strategic projects. The corporation-as-project-steward makes this choice on the same axes as an upstream project would.
- **Trademark policy.** The project's name and logo are trademarks. The corporation should register the mark (see [chapter 04 IP strategy](./04-ip-strategy-trade-secrets-patents-trademarks.md) on the trademark register) and publish a project-trademark-use policy (permitting community references and forbidding endorsement misuse) — otherwise the corporation loses control of the mark as the project grows.
- **Contribution and code-of-conduct policies.** Standard now; typically a `CONTRIBUTING.md`, a `CODE_OF_CONDUCT.md` (Contributor Covenant is the widely-adopted default), and a `SECURITY.md` describing vulnerability-reporting channels.

## The customer-facing OSS warranty in the MSA

The internal OSS hygiene programme has a mirror on the customer-contract side. The MSA ([chapter 01 customer contract](./01-customer-contract-msa-order-form-sla-dpa.md)) typically includes an open-source warranty from the corporation to the customer:

- **No copyleft contamination.** The corporation warrants that the Service does not incorporate open-source software in a manner that would require the customer to (i) disclose, license, or make available its own source code, (ii) license its own intellectual property under an open-source license, or (iii) grant any rights in its own intellectual property to third parties. This is the "no copyleft-triggering combination is present in the delivered Service" warranty.
- **License compliance.** The corporation warrants that all open-source software incorporated into the Service is used in compliance with the applicable open-source license terms.
- **SBOM availability.** Increasingly, the MSA or DPA includes an undertaking to provide an SBOM in a specified format on request or on each release.

The **indemnification interaction** matters. The MSA's IP-infringement indemnity ([chapter 01](./01-customer-contract-msa-order-form-sla-dpa.md)) typically covers third-party claims that the Service infringes a patent, copyright, or trade secret. Many MSAs, however, carve out open-source claims from the IP indemnity — the theory being that OSS licenses are the OSS licensor's business and the corporation should not be indemnifying the customer against the OSS licensor's enforcement. In those MSAs, the **OSS warranty is the customer's substantive protection** against OSS-license-compliance risk; a breach of the OSS warranty gives the customer a contract claim (typically capped at the general liability cap) even though it is outside the indemnity. The corporation should understand which pattern its MSA uses and price the risk accordingly.

## Failure modes

- **GPL v2 / v3 code linked into a distributed proprietary binary.** The FSF's interpretation and the prevailing view of copyright law treat the combined work as a derivative work of the GPL'd code; distribution requires GPL-licensing the whole. Remediation is often architectural rewrite — expensive.
- **AGPL v3 code in a SaaS backend.** § 13 triggers on network-user interaction with a modified version. The corporation either (i) uses the AGPL code unmodified (and then arguably only § 13 for the AGPL work itself applies), (ii) replaces the AGPL component, or (iii) commits to source-disclosure of the modified AGPL code.
- **Missing attribution on MIT / BSD / Apache 2.0 code.** Even permissive licenses require reproducing the copyright notice and license text in copies or substantial portions. Failure is both a license violation (technical copyright infringement) and a contractual breach if the OSS warranty is in play.
- **Failing to preserve upstream copyright headers.** Some corporations' engineering practice includes stripping headers "for cleanliness"; this is a license violation for essentially every permissive and copyleft license.
- **Static linking of LGPL library into a proprietary binary without providing the object-code-relink mechanism.** LGPL §§ 3–4 permit dynamic linking cleanly but require additional steps for static linking that most proprietary builds do not implement.
- **Bundling BUSL / SSPL / Elastic License components as if they were open source.** These licenses forbid the exact managed-service use the corporation may intend; treating them as OSS-approved is a commercial-license breach.
- **SBOM omissions.** The enterprise customer's vendor-security questionnaire flags a dependency the corporation didn't know it was shipping (a transitive dependency of a transitive dependency, often). The dependency itself may be fine; the tracking failure is the finding.
- **No documented outbound-contribution policy.** An employee's upstream contribution is later disputed (or the upstream project is acquired and the acquirer challenges contribution provenance). The corporation cannot demonstrate the CLA chain because the CLA-signing authority and record-keeping were never centralised.
- **Trademark loss on a corporation-released open-source project.** The project grows, third parties fork under the same name, the corporation never enforced the mark, and the mark's distinctiveness is diluted or lost. Trade-secret / IP-strategy interaction — see [chapter 04](./04-ip-strategy-trade-secrets-patents-trademarks.md).

## Concrete example: a Series-A SaaS company's OSS programme

Acme Robotics is a 40-person Series-A SaaS company (Delaware C-Corp; SaaS product delivered from AWS us-east-1). Its OSS programme:

**Approved licenses.**

- Permissive (default-approved, no review required): MIT, BSD 2-Clause, BSD 3-Clause, Apache License 2.0, ISC.
- Weak copyleft (approved with linkage / boundary constraint):
  - LGPL v2.1 and LGPL v3 — **dynamic linking only**; static linking requires engineering-lead + General Counsel sign-off.
  - MPL 2.0 — permitted; modifications to MPL files must be contributed back under MPL.
- Weak copyleft requiring review: EPL 2.0.

**Disapproved licenses (require CEO + GC sign-off with architectural review to override).**

- Strong copyleft: GPL v2, GPL v3, AGPL v3.
- "Source-available" non-OSI licenses: BUSL, SSPL, Elastic License v2, Confluent Community License, Redis Source Available License.
- Non-standard / hand-drafted licenses.

**Tooling.** FOSSA integrated into GitHub Actions CI. Every pull request runs a license scan; a policy violation (a disapproved license introduced as a direct or transitive dependency) fails the build. Monthly license-scan review by the Head of Engineering + GC covering: new components introduced in the month, licenses of any updated components, vulnerability status of components on the SBOM.

**SBOM.** Generated in CycloneDX JSON format on every production build. Stored as an artefact in the release pipeline (Amazon S3 with versioning and a 7-year retention policy — see [mod-106 records retention](../mod-106-compensation-architecture-and-total-rewards/) for the general retention framing). Shipped as a deliverable in the enterprise MSA order form ("Vendor will provide a CycloneDX SBOM for each production release; updated SBOMs will be provided within 30 days of a production release").

**Outbound-contribution policy.** Written policy in the engineering handbook. Employees may contribute to approved-license upstream projects; contributions are made from the corporate email address. The corporation has signed the Apache CCLA authorising named engineers to contribute to Apache Software Foundation projects. Contributions during work hours are on-the-clock. Substantive contributions (feature additions, non-trivial refactors) require engineering-lead approval; typo / small bug fixes are unrestricted.

**Released open source.** Acme has released two utility libraries under Apache License 2.0, with governance: benevolent-dictator (Acme's engineering-lead is maintainer), DCO (`Signed-off-by:` required on each commit), Contributor Covenant code of conduct, published trademark-use policy, security disclosure via `SECURITY.md`.

**MSA OSS warranty.** Acme's MSA includes a no-copyleft-contamination warranty, a license-compliance warranty, and an SBOM-delivery undertaking. The IP-indemnity clause covers patent, copyright, and trade-secret claims and does *not* carve out OSS — Acme's counsel took the position that the internal programme is strong enough that the residual indemnity risk is acceptable.

**Diligence readiness.** In a Series-B diligence workstream, Acme delivers on day one: the written OSS-approval policy, the current CycloneDX SBOM, a FOSSA export showing zero policy violations across the last six months of builds, the signed Apache CCLA, the outbound-contribution policy, and the two open-source project repositories with governance metadata. The OSS workstream closes in a week rather than becoming a diligence blocker.

## Summary

- OSS governance matters simultaneously for legal risk (copyleft compliance), investor diligence (Series-A / B license scans), enterprise procurement (SBOM in vendor questionnaires), and federal-agency sales (EO 14028 § 4(f) / 4(k), OMB M-22-18, CISA attestation).
- The OSI license taxonomy splits into permissive (MIT, BSD 2/3, Apache 2.0, ISC — safe with attribution; Apache 2.0 § 3 adds the patent grant and termination), weak copyleft (LGPL with dynamic linking, MPL 2.0 file-level, EPL module-level — workable with boundary discipline), and strong copyleft (GPL v2, GPL v3 § 5, AGPL v3 § 13 — disapproved for commercial SaaS by default).
- Beyond the OSI list, "source-available" non-OSI licenses (BUSL, SSPL, Elastic License v2) forbid the exact managed-service use most SaaS corporations intend and should be treated as commercial licenses, not open source.
- The SBOM programme delivers a machine-readable inventory in SPDX (ISO/IEC 5962:2021), CycloneDX (OWASP), or SWID (ISO/IEC 19770-2) format, covering the NTIA minimum elements — required for federal-agency sales under EO 14028 § 4(f) / OMB M-22-18 and increasingly required by Fortune-500 procurement.
- Tooling selection (FOSSA, Tidelift, Snyk, Black Duck, Mend, Sonatype Nexus IQ) is evaluated on language coverage, license-detection accuracy, false-positive rate, policy granularity, CI integration, SBOM output support, vulnerability data, and remediation guidance — see mod-112 SecReview and cto-curriculum for the engineering-side implementation.
- The outbound-contribution policy authorises employees to contribute upstream under the approved-license list, defines corporation copyright ownership and attribution, and identifies the CLA-signing authority; the Apache ICLA and CCLA are the practitioner-standard mechanisms, with DCO as a lighter-weight alternative.
- The decision to release the corporation's own open source is a separate architectural / strategic decision; the defaults are MIT or Apache 2.0 for the license, benevolent-dictator or foundation stewardship for governance, DCO or CLA for inbound contributions, and a registered trademark plus published trademark-use policy for the project name.
- The MSA's OSS warranty (no copyleft contamination, license compliance, SBOM availability) is the customer-facing mirror of the internal programme; where the IP-indemnity clause carves out OSS, the OSS warranty is the customer's substantive protection.
- Common failure modes: GPL v2/v3 linked into a distributed proprietary binary, AGPL v3 in a SaaS backend, missing attribution on permissive-license code, stripped copyright headers, static linking of LGPL without the § 4 relink mechanism, treating BUSL / SSPL as OSS, SBOM omissions revealed by customer questionnaires, and undocumented outbound contributions with no CLA chain.
