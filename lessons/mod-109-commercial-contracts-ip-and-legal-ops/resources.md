# Resources — mod-109 Commercial Contracts, IP & Legal Ops

Primary statutes, regulations, model clauses, agency guidance, standard-setting bodies, and vendor documentation cited across the chapters. Prefer these to secondary summaries. Where the underlying rule is in motion (EU AI Act phasing and delegated acts, Executive Order 14028 implementing standards, DPF adequacy, state auto-renewal statutes, enterprise AI-vendor terms, CLM-vendor feature coverage), the corresponding chapter carries a `<!-- needs-research: ... -->` marker; refresh the cite before treating the material as canonical.

## Uniform Commercial Code — Article 2 (sale of goods, warranty disclaimers)

- **UCC Article 2 — Sales.** The warranty and warranty-disclaimer discipline the MSA's implied-warranty disclaimer is drafted to satisfy. Whether Article 2 applies to a SaaS transaction is unsettled (Article 2 governs sales of goods; SaaS is arguably a service), but the practitioner default is to write the disclaimer so that if a court later applies Article 2 the disclaimer holds.
  - **§ 2-313** — express warranties.
  - **§ 2-314** — implied warranty of merchantability.
  - **§ 2-315** — implied warranty of fitness for a particular purpose.
  - **§ 2-316** — exclusion or modification of warranties. Disclaimers of merchantability must be conspicuous and must mention "merchantability" by name; disclaimers of fitness must be in writing and conspicuous. This is the drafting target for the MSA warranty-disclaimer paragraph.
  - **§ 2-719** — contractual modification or limitation of remedy. The "sole and exclusive remedy" language in the SLA runs through § 2-719.
- Primary text at the Uniform Law Commission: https://www.uniformlaws.org/committees/community-home?communitykey=be8e8dde-73c5-4c67-9d20-85ad42f1a93f and in each state's enactment (e.g., Delaware 6 Del. C. §§ 2-101 to 2-725; California Cal. Comm. Code §§ 2101–2725).
- **Restatement (Second) of Contracts** — American Law Institute. Background on contract formation, offer and acceptance, interpretation, and remedies that underlies the MSA.
- **CISG — United Nations Convention on Contracts for the International Sale of Goods.** The MSA's governing-law clause typically opts out of the CISG expressly; identify the clause and preserve the opt-out.

## Privacy and the DPA (structural anatomy only — regulatory depth in [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/))

- **Regulation (EU) 2016/679 (GDPR).** Consolidated text: https://eur-lex.europa.eu/eli/reg/2016/679/oj
  - **Article 4(7)–(8)** — controller / processor definitions.
  - **Article 28** — processor obligations and the mandatory DPA content list.
  - **Article 32** — security of processing (the TOMs clause in Annex II).
  - **Article 33** — breach notification by processor to controller "without undue delay."
  - **Article 44** — general principle for international transfers.
  - **Articles 45–49** — adequacy decisions, Standard Contractual Clauses, Binding Corporate Rules, derogations.
- **UK GDPR** — Data Protection Act 2018 and the UK General Data Protection Regulation.
- **Commission Implementing Decision (EU) 2021/914** of 4 June 2021 on standard contractual clauses for the transfer of personal data to third countries pursuant to Regulation (EU) 2016/679. The four-module SCC schedule. https://eur-lex.europa.eu/eli/dec_impl/2021/914/oj
- **UK International Data Transfer Addendum (IDTA)** and the **UK Addendum to the EU SCCs**. ICO guidance: https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/international-transfers/international-data-transfer-agreement-and-guidance/
- **Swiss addendum to the EU SCCs** — Swiss Federal Data Protection and Information Commissioner (FDPIC) guidance.
- **EU–US Data Privacy Framework.** **Commission Implementing Decision (EU) 2023/1795** of 10 July 2023 on the adequate level of protection of personal data under the EU-US Data Privacy Framework. https://eur-lex.europa.eu/eli/dec_impl/2023/1795/oj Framework self-certification register: https://www.dataprivacyframework.gov/
- **California Consumer Privacy Act (CCPA) / California Privacy Rights Act (CPRA).** Cal. Civ. Code § 1798.100 et seq.
  - **§ 1798.140(ag)** — "service provider" definition and the service-provider-contract-content list that the CCPA addendum to the DPA tracks.
  - **§ 1798.140(ah)** — "contractor" definition and the parallel contractor-contract content list.
  - **CPPA regulations** — California Privacy Protection Agency final regulations. https://cppa.ca.gov/regulations/
- **State comprehensive privacy statutes.** Colorado Privacy Act (Colo. Rev. Stat. § 6-1-1301 et seq.); Virginia Consumer Data Protection Act (Va. Code § 59.1-575 et seq.); Connecticut Data Privacy Act (Conn. Pub. Act 22-15); Utah Consumer Privacy Act (Utah Code § 13-61-101 et seq.). Full state-by-state map: [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/).
- **HIPAA Business Associate Agreement.** 45 C.F.R. §§ 164.502(e) and 164.504(e). Required-content list for the BAA, which supplements the general DPA when the Service processes PHI. HHS BAA sample: https://www.hhs.gov/hipaa/for-professionals/covered-entities/sample-business-associate-agreement-provisions/index.html
- **Shared Assessments SIG (Standardized Information Gathering).** Industry-standard third-party-security questionnaire — SIG, SIG Lite, SIG Core. https://sharedassessments.org/sig/ <!-- needs-research: confirm current SIG release year and the SIG-Core-vs-SIG-Lite coverage differential before quoting a specific module count. -->
- **AICPA SOC 2** — Trust Services Criteria and the SOC 2 Type I / Type II attestation. https://www.aicpa-cima.com/topic/audit-assurance/audit-and-assurance-greater-than-soc-2 Type II covers operating effectiveness over a defined period (typically 12 months); Type I is point-in-time design and is materially weaker.
- **ISO/IEC 27001:2022** — Information Security Management Systems. https://www.iso.org/standard/27001

## AI contracts and governance (chapter 06)

- **Regulation (EU) 2024/1689 — EU Artificial Intelligence Act.** Consolidated text: https://eur-lex.europa.eu/eli/reg/2024/1689/oj
  - **Chapter II (Articles 5)** — prohibited AI practices.
  - **Chapter III (Articles 6–49)** — high-risk AI systems.
  - **Chapter V (Articles 51–55)** — general-purpose AI models (GPAI) and GPAI with systemic risk; the GPAI addendum pattern in chapter 06 tracks these obligations.
  - **Chapter IV (Article 50)** — transparency obligations for providers and deployers of certain AI systems.
  - <!-- needs-research: confirm the current effective-date phasing (prohibited-practices provisions, GPAI provisions, high-risk-system provisions) and any delegated or implementing acts adopted after initial publication. -->
- **NIST AI Risk Management Framework 1.0** (January 2023). https://www.nist.gov/itl/ai-risk-management-framework
- **NIST AI RMF Generative AI Profile — NIST AI 600-1** (July 2024). https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf
- **NIST AI RMF Playbook.** https://airc.nist.gov/AI_RMF_Knowledge_Base/Playbook
- **ISO/IEC 42001:2023 — AI management system.** https://www.iso.org/standard/81230.html
- **OECD AI Principles** (2019; revised 2024). https://oecd.ai/en/ai-principles
- **White House — Blueprint for an AI Bill of Rights** (October 2022). https://www.whitehouse.gov/ostp/ai-bill-of-rights/ <!-- needs-research: confirm current status of the Blueprint and successor policy guidance after 2025 executive-branch changes; Executive Order 14110 has been revoked and successor policy should be verified before citing. -->
- **Enterprise AI-vendor documentation.** <!-- needs-research: confirm current enterprise-terms, zero-data-retention posture, training-opt-out mechanics, DPA availability, and IP-indemnity text for each provider before quoting as canonical. -->
  - **Anthropic — Claude for Work / Claude Enterprise.** https://www.anthropic.com/claude-for-work and the Anthropic Trust Center https://trust.anthropic.com/
  - **OpenAI — ChatGPT Enterprise, Azure OpenAI.** https://openai.com/chatgpt/enterprise and https://openai.com/policies
  - **Microsoft Copilot for Microsoft 365 / Copilot Enterprise.** https://www.microsoft.com/en-us/microsoft-365/copilot
  - **Google — Gemini for Google Workspace and Vertex AI.** https://workspace.google.com/solutions/ai/
  - **AWS Bedrock — Service Terms and Responsible AI.** https://aws.amazon.com/bedrock/
  - **GitHub Copilot — Business / Enterprise.** https://github.com/features/copilot
- **US Copyright Office — Policy Statement, Works Containing Material Generated by Artificial Intelligence** (March 2023). 88 Fed. Reg. 16190. https://www.copyrightoffice.gov/ai/
- **US Copyright Office — Report on Copyright and Artificial Intelligence** (serial publication, 2024–). https://www.copyright.gov/ai/ <!-- needs-research: confirm the current Report Parts (Digital Replicas, Copyrightability, Generative AI Training) status and successor parts. -->
- ***Thaler v. Perlmutter***, 687 F. Supp. 3d 140 (D.D.C. 2023), aff'd No. 23-5233 (D.C. Cir. 2025) — human-authorship requirement for copyright, applied to purely-AI-generated outputs. <!-- needs-research: confirm the current appellate posture. -->

## Intellectual property — patents (chapter 04)

- **Title 35 of the United States Code — Patents.**
  - **35 U.S.C. § 101** — patentable subject matter. https://www.law.cornell.edu/uscode/text/35/101
  - **35 U.S.C. § 102** — novelty; conditions for patentability. https://www.law.cornell.edu/uscode/text/35/102 (including the one-year grace period and the first-inventor-to-file mechanics under AIA).
  - **35 U.S.C. § 103** — non-obviousness. https://www.law.cornell.edu/uscode/text/35/103
  - **35 U.S.C. § 112** — specification, enablement, written description, means-plus-function. https://www.law.cornell.edu/uscode/text/35/112
  - **35 U.S.C. § 154** — term of patent (20 years from earliest effective filing date, subject to patent term adjustment and extension).
  - **35 U.S.C. § 287** — marking requirement.
- **Leahy-Smith America Invents Act (AIA), Pub. L. 112-29** (16 September 2011; most provisions effective 16 March 2013). https://www.congress.gov/bill/112th-congress/house-bill/1249 Shifted US from first-to-invent to first-inventor-to-file.
- **USPTO — Manual of Patent Examining Procedure (MPEP).** https://www.uspto.gov/web/offices/pac/mpep/
- **USPTO — General Information.** https://www.uspto.gov/patents
- **USPTO — Patent fees.** https://www.uspto.gov/learning-and-resources/fees-and-payment/uspto-fee-schedule <!-- needs-research: confirm current fee schedule and any small-entity / micro-entity fee discounts applicable. -->
- **Patent Cooperation Treaty (PCT).** Administered by the World Intellectual Property Organization (WIPO). https://www.wipo.int/pct/en/
- **European Patent Convention (EPC)** and the **Unitary Patent system / Unified Patent Court (UPC)**. https://www.epo.org/
- **Key subject-matter case law.**
  - ***Alice Corp. Pty. Ltd. v. CLS Bank Int'l***, 573 U.S. 208 (2014) — two-step framework for abstract-idea subject matter.
  - ***Mayo Collaborative Services v. Prometheus Laboratories***, 566 U.S. 66 (2012) — law-of-nature carve-out.
  - ***Bilski v. Kappos***, 561 U.S. 593 (2010) — machine-or-transformation test rejected as sole test for process patents.
- **Obviousness.** ***KSR Int'l Co. v. Teleflex Inc.***, 550 U.S. 398 (2007).
- **Defensive patent aggregators.**
  - **LOT Network** — Licence on Transfer agreement. https://lotnet.com/
  - **Open Invention Network (OIN).** https://openinventionnetwork.com/
  - **Unified Patents.** https://www.unifiedpatents.com/
- **Patent Trial and Appeal Board (PTAB)** — inter partes review and post-grant review. 35 U.S.C. §§ 311–329. https://www.uspto.gov/patents/ptab

## Intellectual property — trademarks (chapter 04)

- **Lanham Act — 15 U.S.C. §§ 1051–1141n.**
  - **§ 1051** — application for registration; use-in-commerce and intent-to-use filings.
  - **§ 1052** — refusal of registration (functionality, descriptiveness, deceptive matter, confusing similarity under § 2(d)).
  - **§ 1057** — certificates of registration and principal-register benefits.
  - **§ 1065** — incontestability after five years of continuous use (if the registrant files a § 15 declaration).
  - **§ 1114** — infringement of registered marks and remedies.
  - **§ 1125(a)** — unfair competition and false designation of origin; false endorsement; trade-dress protection.
  - **§ 1125(c)** — dilution of famous marks under the Trademark Dilution Revision Act of 2006.
- **USPTO — Trademark Manual of Examining Procedure (TMEP).** https://tmep.uspto.gov/
- **USPTO — Trademark Electronic Search System (TESS).** https://www.uspto.gov/trademarks/search
- **USPTO — Trademark fees.** https://www.uspto.gov/trademarks/fees-payment-information <!-- needs-research: confirm current fee schedule and any TEAS Standard vs. TEAS Plus differentials. -->
- **Trademark Trial and Appeal Board (TTAB).** https://www.uspto.gov/trademarks/ttab
- **Madrid Protocol.** International trademark registration administered by WIPO. https://www.wipo.int/madrid/en/
- **European Union Intellectual Property Office (EUIPO).** EU trade mark (EUTM) and Registered Community Design. https://euipo.europa.eu/
- **UK Intellectual Property Office (UKIPO).** https://www.gov.uk/government/organisations/intellectual-property-office
- **Canadian Intellectual Property Office (CIPO).** https://ised-isde.canada.ca/site/canadian-intellectual-property-office/
- **IP Australia.** https://www.ipaustralia.gov.au/

## Intellectual property — copyright (chapter 04)

- **Title 17 of the United States Code — Copyrights.**
  - **17 U.S.C. § 102** — subject matter of copyright (original works of authorship fixed in a tangible medium of expression).
  - **17 U.S.C. § 106** — exclusive rights.
  - **17 U.S.C. § 107** — fair use.
  - **17 U.S.C. § 201** — ownership (including works made for hire).
  - **17 U.S.C. § 408** — registration (permissive, but prerequisite to § 411 infringement suit for US works).
  - **17 U.S.C. § 411** — registration as precondition to suit for US works.
  - **17 U.S.C. § 504** — remedies; statutory damages available only for pre-infringement-registered works per § 412.
  - **17 U.S.C. § 512 — DMCA safe harbour** for online service providers (notice-and-takedown; counter-notification; registered DMCA agent). https://www.copyright.gov/dmca-directory/
- **US Copyright Office.** https://www.copyright.gov/
- **Berne Convention for the Protection of Literary and Artistic Works** and the **WIPO Copyright Treaty**.
- **CC licences — Creative Commons.** Reference set for licensed-work attribution and reuse. https://creativecommons.org/

## Intellectual property — trade secrets (chapter 04)

- **Defend Trade Secrets Act (DTSA), 18 U.S.C. §§ 1836–1839.** Federal civil cause of action for trade-secret misappropriation (added 2016 by Pub. L. 114-153). Includes:
  - **§ 1836(b)** — civil action.
  - **§ 1836(b)(3)(D)** — ex parte seizure.
  - **§ 1833(b)** — immunity for whistleblowers; required notice in employee / contractor agreements that contain confidentiality / trade-secret obligations (the "DTSA notice"). Cross-reference the PIIA and NDA templates in [mod-103](../mod-103-employment-law-and-contract-design/).
- **Uniform Trade Secrets Act (UTSA).** Enacted in some form in nearly every US state. Primary text: https://www.uniformlaws.org/committees/community-home?CommunityKey=3a2538fb-e030-4e2d-a9e2-90373dc05792
- **Economic Espionage Act (EEA), 18 U.S.C. §§ 1831–1839.** Federal criminal trade-secret statute.
- **California Civil Code § 3426 et seq.** — California UTSA.
- **New York** — common-law trade-secret doctrine (New York has not enacted UTSA; practitioner analysis under *Faiveley Transport Malmö AB v. Wabtec Corp.*, 559 F.3d 110 (2d Cir. 2009) and successor cases).
- **American Bar Association — Section of Intellectual Property Law, Trade Secrets Committee.** https://www.americanbar.org/groups/intellectual_property_law/committees/trade_secrets/

## Chain of title and PIIAs (cross-references)

- **Work-for-hire doctrine.** 17 U.S.C. §§ 101 and 201(b); the two-prong test for "work made for hire" (employee in scope of employment; or one of nine categories of specially commissioned works for which the parties expressly agree in writing).
- **Pre-formation IP assignment and founder PIIA mechanics** — [mod-102 — Founding-Team Legal Architecture](../mod-102-founding-team-legal-architecture/).
- **Employee PIIA with DTSA whistleblower notice and the state-law variance (California § 2870 carve-out, Washington RCW 49.44.140, Illinois 765 ILCS 1060/2, Minnesota Minn. Stat. § 181.78)** — [mod-103 — Employment Law, Worker Classification & Contract Design](../mod-103-employment-law-and-contract-design/).

## Open-source hygiene and the SBOM programme (chapter 05)

- **Open Source Initiative — OSI-approved licence list.** https://opensource.org/licenses
  - **MIT License.** https://opensource.org/license/mit
  - **BSD 2-Clause ("Simplified").** https://opensource.org/license/bsd-2-clause and **BSD 3-Clause ("New").** https://opensource.org/license/bsd-3-clause
  - **Apache License, Version 2.0.** https://www.apache.org/licenses/LICENSE-2.0 (patent-licence grant at § 3; NOTICE-file propagation at § 4; patent-litigation termination at § 3).
  - **GNU General Public License v2.0** https://www.gnu.org/licenses/old-licenses/gpl-2.0.html and **v3.0** https://www.gnu.org/licenses/gpl-3.0.html
  - **GNU Lesser General Public License v2.1 / v3.** https://www.gnu.org/licenses/lgpl-3.0.html
  - **GNU Affero General Public License v3** (AGPL-3.0). https://www.gnu.org/licenses/agpl-3.0.html (§ 13 network-use trigger).
  - **Mozilla Public License 2.0.** https://www.mozilla.org/en-US/MPL/2.0/
  - **Eclipse Public License 2.0.** https://www.eclipse.org/legal/epl-2.0/
  - **ISC License.** https://opensource.org/license/isc-license-txt
- **FSF — Free Software Foundation.** License list and compatibility matrix. https://www.gnu.org/licenses/license-list.html
- **SPDX — Software Package Data Exchange** (ISO/IEC 5962:2021). The Linux Foundation SPDX specification and licence list. https://spdx.dev/
- **CycloneDX** — OWASP SBOM specification. https://cyclonedx.org/
- **NTIA — "The Minimum Elements for a Software Bill of Materials"** (July 2021). https://www.ntia.gov/report/2021/minimum-elements-software-bill-materials-sbom
- **Executive Order 14028** — *Improving the Nation's Cybersecurity* (May 12, 2021). https://www.whitehouse.gov/briefing-room/presidential-actions/2021/05/12/executive-order-on-improving-the-nations-cybersecurity/ § 4(e), § 4(f), § 4(k) on software-supply-chain security and SBOM.
- **OMB Memorandum M-22-18** — *Enhancing the Security of the Software Supply Chain through Secure Software Development Practices* (September 14, 2022). https://www.whitehouse.gov/wp-content/uploads/2022/09/M-22-18.pdf
- **OMB Memorandum M-23-16** — update to M-22-18 (June 9, 2023). https://www.whitehouse.gov/wp-content/uploads/2023/06/M-23-16-Update-to-M-22-18-Enhancing-Software-Security.pdf
- **NIST — Secure Software Development Framework (SSDF), SP 800-218.** https://csrc.nist.gov/publications/detail/sp/800-218/final
- **CISA — Securing the Software Supply Chain and SBOM resource page.** https://www.cisa.gov/sbom
- **License-compliance tooling.** <!-- needs-research: confirm current product tiers, hosted-vs-self-hosted posture, SBOM-format support, and pricing before quoting as canonical in a selection memo. -->
  - **FOSSA.** https://fossa.com/
  - **Black Duck (Synopsys / Black Duck Software).** https://www.synopsys.com/software-integrity/security-testing/software-composition-analysis.html
  - **Snyk Open Source and Snyk License Compliance.** https://snyk.io/
  - **Tidelift.** https://tidelift.com/
  - **GitHub Advanced Security — Dependency Review, CodeQL, Dependabot.** https://docs.github.com/en/code-security
- **Software Freedom Law Center (SFLC).** Legal services and OSS-compliance guidance. https://softwarefreedom.law.columbia.edu/
- **Software Package Data Exchange SPDX License List.** https://spdx.org/licenses/

## CLM — contract lifecycle management (chapter 07)

<!-- needs-research: confirm current product tiers, native-vs-add-in editor posture, e-signature-vendor coupling, HRIS / Salesforce integration coverage, AI-feature set, and pricing before quoting as canonical in a selection memo. -->

- **Ironclad.** https://ironcladapp.com/
- **LinkSquares.** https://linksquares.com/
- **DocuSign CLM** (DocuSign Agreement Cloud). https://www.docusign.com/products/clm
- **Concord.** https://www.concord.app/
- **Contract Logix.** https://www.contractlogix.com/
- **Agiloft.** https://www.agiloft.com/
- **Juro.** https://juro.com/
- **PandaDoc.** https://www.pandadoc.com/
- **Icertis.** https://www.icertis.com/
- **Conga Contracts (and Conga CLM).** https://conga.com/products/conga-contracts
- **SpotDraft.** https://www.spotdraft.com/
- **Lexion** (acquired by Docusign; integration status may be relevant). https://www.docusign.com/products/clm
- **E-signature.** DocuSign (https://www.docusign.com/), Adobe Acrobat Sign (https://www.adobe.com/sign.html), Dropbox Sign (formerly HelloSign; https://sign.dropbox.com/).
- **ESIGN Act (Electronic Signatures in Global and National Commerce Act), 15 U.S.C. §§ 7001–7006** and the **Uniform Electronic Transactions Act (UETA)**. Federal and state frameworks for enforceability of electronic signatures.
- **Legal-ops professional communities and benchmarks.**
  - **Corporate Legal Operations Consortium (CLOC).** https://cloc.org/
  - **Association of Corporate Counsel (ACC).** https://www.acc.com/
  - <!-- needs-research: confirm current CLOC Core Competencies, ACC Chief Legal Officers Survey, and the ACC/EY Law Firm Hourly Rate Survey editions and specific figures before quoting as canonical. -->

## In-house vs. outside-counsel references (chapter 08)

<!-- needs-research: confirm current firm-level startup-practice coverage, deferred-fee arrangement terms, partner rate ranges, and panel-firm management vendors (Simple Legal, Mitratech TyMetrix, Brightflag, etc.) before quoting specific figures. -->

- **Big Law startup practices.**
  - **Cooley LLP.** https://www.cooley.com/
  - **Wilson Sonsini Goodrich & Rosati (WSGR).** https://www.wsgr.com/
  - **Orrick, Herrington & Sutcliffe LLP.** https://www.orrick.com/
  - **Fenwick & West LLP.** https://www.fenwick.com/
  - **Latham & Watkins LLP.** https://www.lw.com/
  - **Gunderson Dettmer Stough Villeneuve Franklin & Hachigian, LLP.** https://www.gunder.com/
  - **Goodwin Procter LLP.** https://www.goodwinlaw.com/
  - **Perkins Coie LLP.** https://www.perkinscoie.com/
  - **DLA Piper LLP.** https://www.dlapiper.com/
  - **Morrison & Foerster LLP.** https://www.mofo.com/
  - **Kirkland & Ellis LLP.** https://www.kirkland.com/
- **IP boutiques (prosecution and litigation).** Fish & Richardson (https://www.fr.com/), Finnegan Henderson (https://www.finnegan.com/), Knobbe Martens (https://www.knobbe.com/), Sterne Kessler Goldstein & Fox (https://www.sternekessler.com/), Perkins Coie IP (https://www.perkinscoie.com/en/practices/intellectual-property.html).
- **Alternative Legal Service Providers (ALSPs).** Axiom (https://www.axiomlaw.com/), Elevate (https://www.elevateservices.com/), UnitedLex (https://unitedlex.com/).
- **NVCA — National Venture Capital Association model legal documents.** The NVCA-derived venture-financing documents (COIP, IRA, VA, ROFR, MRL) that outside counsel will draft on priced rounds. https://nvca.org/model-legal-documents/
- **Delaware General Corporation Law (DGCL), 8 Del. C. § 101 et seq.** The entity-law substrate for the officer-authority and board-resolution mechanics the signature discipline runs on.

## Deal-desk, playbook, and SaaS-contract market precedent (chapter 02)

- **Bloom, Lee & Spencer / Vinson & Elkins / Perkins Coie / Fenwick public MSA templates** — several Big Law firms and academic clinics publish redacted or template MSAs that illustrate the drafting norms the playbook calibrates against. <!-- needs-research: locate currently-published template sets and confirm the version in reference. -->
- **TechGC.** Peer-benchmarked legal-ops and playbook community. https://techgc.co/
- **Bonterms.** Public reference set of common commercial contract clauses. https://bonterms.com/
- **CommonPaper.** Open contract templates for enterprise software. https://commonpaper.com/
- **oneNDA.** Public standard-form NDA. https://onenda.org/
- **TLDRLegal.** Plain-English summaries of common software licences (reference, not authority). https://tldrlegal.com/

## Industry questionnaires and third-party-risk standards

- **Shared Assessments SIG / SIG Lite / SIG Core.** https://sharedassessments.org/sig/
- **CAIQ (Cloud Security Alliance — Consensus Assessments Initiative Questionnaire).** https://cloudsecurityalliance.org/research/caiq/
- **CSA STAR Registry.** https://cloudsecurityalliance.org/star/
- **TPRM (Third-Party Risk Management) frameworks.** ISO/IEC 27036 (information security for supplier relationships); NIST SP 800-161r1 (Cybersecurity Supply Chain Risk Management).
- **Vendor risk-management platforms** — OneTrust, Vanta, Drata, Secureframe, Prevalent, Whistic. <!-- needs-research: confirm current product coverage and tiers before quoting as canonical. -->

## State auto-renewal and consumer-contract statutes (chapter 02, chapter 07)

Consumer-focused but influential on enterprise auto-renewal practice:

- **California Automatic Renewal Law (ARL), Cal. Bus. & Prof. Code § 17600 et seq.** As amended by AB 390, SB 313, and successor amendments.
- **New York General Obligations Law § 5-903.** Automatic renewal; required written notice to residents.
- **Illinois Automatic Contract Renewal Act, 815 ILCS 601/.**
- **FTC — "Click-to-Cancel" rule (16 C.F.R. § 425).** <!-- needs-research: confirm current rulemaking status, effective date, and any litigation stays. -->
- Primary agency resources: FTC https://www.ftc.gov/

## M&A and IPO diligence (hand-off to `startup-exit-curriculum`)

- **ABA Model Stock Purchase Agreement and Model Asset Purchase Agreement.** American Bar Association, Section of Business Law. Reference models for the diligence rep-and-warranty schedules the mod-109 contract manifest and IP schedule feed.
- **SEC — Regulation S-K.** 17 C.F.R. § 229.
- **SEC — Regulation S-X.** 17 C.F.R. § 210.
- **SEC — EDGAR filings and S-1 corpus.** https://www.sec.gov/edgar
- **R&W insurance.** AIG, Chubb, Beazley, Liberty, QBE, Berkshire Hathaway Specialty Insurance. <!-- needs-research: confirm current carrier panel for middle-market tech R&W placements. -->

## Insurance and risk (cross-reference to [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/))

- **Cyber liability and tech E&O.** Beazley, Chubb, Travelers, AIG, Coalition, At-Bay. The cyber tower sets the practical ceiling on the data-breach super-cap in the MSA.
- **D&O and EPLI.** Chubb, AIG, Travelers, Hiscox.
- **Commercial General Liability (CGL) and umbrella.** The Hartford, Chubb, Travelers.
- <!-- needs-research: confirm current carrier appetite, limit availability, and retentions for the Series-A / B / C profile before quoting a tower structure. -->

---

*Where a resource above cannot be verified at time of publication (current effective-date phasing of the EU AI Act and delegated acts, current status of federal AI executive orders after 2025 changes, current enterprise terms and training-opt-out posture for the enterprise LLM offerings, current USPTO and TMEP fee schedules and small-entity thresholds, current CLM-vendor feature coverage and pricing, current CLOC / ACC survey editions and benchmark figures, current FTC "Click-to-Cancel" rulemaking status, current state auto-renewal and consumer-contract statute amendments, current cyber-liability carrier appetite and limit availability), a `<!-- needs-research: ... -->` marker is inline in the corresponding chapter or in this resources index and should be resolved before that material is treated as canonical.*
