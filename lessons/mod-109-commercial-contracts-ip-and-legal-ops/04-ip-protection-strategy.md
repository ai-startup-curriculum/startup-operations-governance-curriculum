# 4. IP protection strategy: patents, trademarks, copyrights, and trade secrets

> Intellectual property at a Series-A corporation is not a litigation programme; it is a diligence artefact, a defensive shield, a commercial-negotiation lever, and the substrate that makes the customer-facing IP indemnity in the MSA defensible. What matters at this stage is not how much IP the corporation *owns*, but how cleanly it can *prove* what it owns, on demand, to an investor's counsel or a buyer's diligence team.

## Motivation

A Series-A or Series-B corporation has no meaningful litigation capacity. It does not have the balance sheet to fund a multi-year patent infringement suit against a well-capitalised competitor, does not have in-house IP counsel, and cannot in practice enforce most of the rights it holds. Even so, IP protection matters at this stage for four independent reasons, each of which is enough on its own to justify a written programme:

1. **IP is a diligence artefact.** Every institutional financing round after seed — and every M&A transaction — runs an IP diligence workstream. The buy-side counsel (Wilson Sonsini, Cooley, Latham, Gunderson, Fenwick, or the equivalent) requests a schedule of patents and applications, a schedule of trademarks and registrations, a schedule of registered copyrights, a description of the trade-secret programme, chain-of-title evidence for every material IP asset, and evidence that every past employee and contractor executed a PIIA that assigned their work to the corporation. Missing artefacts at diligence become either a purchase-price adjustment, a rep-and-warranty carve-out, an escrow, or (occasionally) a deal delay. The corporation whose IP paperwork is clean on day one of diligence closes faster and at better terms.

2. **IP is a defensive shield.** Even a small filed patent portfolio, a registered mark, and a documented trade-secret programme change the arithmetic when a competitor considers a claim against the corporation and when a non-practising entity (NPE, "patent troll") screens the corporation for suit. A corporation with zero IP filings and no documented trade-secret programme looks like a plaintiff's opportunity; a corporation with a modest defensive portfolio, membership in a defensive-patent aggregator (LOT Network, Open Invention Network), and a documented trade-secret programme looks like more work than it is worth.

3. **IP is an offensive lever in commercial negotiations.** Trademarks and patents in the corporation's name change how a strategic partner, licensor, or acquirer models the relationship. A partnership discussion in which the corporation can point to a filed provisional or a registered mark on the hero product is a different negotiation from one in which the corporation has only common-law rights and unfiled ideas.

4. **IP is the substrate for the customer-facing indemnity.** The MSA's IP indemnity ([chapter 01](./01-customer-contract-suite-msa-sla-dpa-security-aup.md)) commits the corporation to defend the customer against third-party claims that the Service infringes a third party's IP. That commitment is only credible if the corporation actually owns what it is licensing to the customer — every material contribution to the Service must trace back to a properly assigned author (employee under a PIIA, contractor under an IP-assignment SOW), and every third-party component must be under a licence that permits the corporation's use. IP hygiene inside the corporation is what makes the outbound indemnity underwritable.

This chapter covers the *strategic* IP layer — what to file, what to keep as trade secret, how to think about the patent-vs-trade-secret decision, and how to prepare for diligence. It defers to other chapters and modules for the mechanics:

- **Founder-era pre-formation IP and PIIA** — [mod-102](../mod-102-founding-team-legal-architecture/).
- **Employee PIIA and DTSA whistleblower notices in employment contracts** — [mod-103](../mod-103-employment-law-and-contract-design/).
- **Contractor / consultant IP assignment in vendor SOWs** — [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md).
- **Open-source licence hygiene and the SBOM programme** — [chapter 05](./05-open-source-hygiene-and-sbom-programme.md).
- **Privacy and data-governance overlap with trade-secret protection for personal data** — [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/).
- **Entity structuring for IP holding subsidiaries** — [mod-101](../mod-101-legal-entity-formation-and-corporate-structure/).

The strategy that follows is stage-appropriate for a Series-A → growth-stage US C-corporation. Mature-corporation IP work — active portfolio prosecution, cross-licensing, standards-essential-patent commitments, formal FTO opinions on every product launch — is beyond this chapter's scope; the aim here is a defensible programme sized to the corporation's stage.

## The patent decision framework

Patents are the most expensive and most visible IP asset and often the one founders ask about first. The right answer for most Series-A corporations is "not yet, or one narrowly-targeted provisional," and understanding why requires walking through the statutory framework and the cost curve.

### Statutory anatomy

United States utility patents are governed by Title 35 of the U.S. Code. The four core requirements a claim must satisfy to be patentable are:

- **Patentable subject matter** ([35 U.S.C. § 101](https://www.law.cornell.edu/uscode/text/35/101)) — "any new and useful process, machine, manufacture, or composition of matter, or any new and useful improvement thereof." The statutory categories are broad; the doctrinal limits (abstract ideas, laws of nature, natural phenomena) come from case law and are the current active battleground for software patents (see the *Alice* / *Mayo* / *Bilski* trilogy below).
- **Novelty** ([35 U.S.C. § 102](https://www.law.cornell.edu/uscode/text/35/102)) — the invention was not previously patented, described in a printed publication, publicly used, on sale, or otherwise available to the public before the effective filing date. § 102(b)(1) provides a one-year grace period for the inventor's own disclosures — a filing must be made within one year of the inventor's first public disclosure, sale, or offer for sale, or the invention is barred (the "on-sale bar" and "public-disclosure bar"). Under the Leahy-Smith America Invents Act ([Pub. L. 112-29](https://www.congress.gov/bill/112th-congress/house-bill/1249), effective 16 March 2013), the US moved from a first-to-invent to a **first-inventor-to-file** system; the inventor's own grace-period disclosures still preserve their priority against later third-party disclosures within the one-year window, but a third party's independent filing that predates the inventor's own filing (even if the inventor conceived first) defeats the inventor's application. In practical terms: get on file before public disclosure, and if that is not possible, file within twelve months.
- **Non-obviousness** ([35 U.S.C. § 103](https://www.law.cornell.edu/uscode/text/35/103)) — the differences between the claimed invention and the prior art must not have been obvious to a person having ordinary skill in the art at the effective filing date. Obviousness is where most rejections and most invalidity attacks live; the *KSR Int'l Co. v. Teleflex Inc.*, 550 U.S. 398 (2007) framework relaxed the earlier "teaching-suggestion-motivation" test and made obviousness a more flexible (and, from the applicant's perspective, more dangerous) doctrine.
- **Specification and enablement** ([35 U.S.C. § 112](https://www.law.cornell.edu/uscode/text/35/112)) — the specification must describe the invention in sufficient detail to enable a person skilled in the art to make and use it, and the claims must particularly point out and distinctly claim the subject matter. § 112(f) additionally governs means-plus-function claiming, which is a specialised drafting mode and largely a claim-drafting concern for counsel.

The patent term is **20 years from the earliest non-provisional filing date** ([35 U.S.C. § 154](https://www.law.cornell.edu/uscode/text/35/154)), with possible term adjustments for USPTO delay under § 154(b) and term extensions in specific regulatory contexts (Hatch-Waxman for pharmaceuticals). The 20-year clock runs from filing, not from issuance — which means every year in prosecution is a year off the effective monopoly.

### The on-sale bar and its interaction with launch strategy

The on-sale bar under § 102(b)(1) is the single most common trap for founder-era inventions. If the corporation publicly discloses, demonstrates, offers for sale, or actually sells a product embodying the invention *before* the filing date, and the sale is not covered by an experimental-use exception, the one-year grace period begins running. Under AIA first-inventor-to-file, that grace period only protects against the inventor's *own* prior disclosures — third-party filings during the grace period can still defeat the inventor. The Supreme Court's ruling in *Helsinn Healthcare S.A. v. Teva Pharmaceuticals USA, Inc.*, 586 U.S. 123 (2019), confirmed that the AIA preserves the pre-AIA understanding of "on sale" — a confidential sale to a third party can trigger the bar even if the sale did not disclose the invention publicly. The practical implication: any commercial engagement (a pilot with a design partner, a beta customer under NDA, a demo to an investor under NDA) that involves an offer for sale of a product embodying a patentable invention starts the twelve-month clock. If patent protection is contemplated, file — at minimum a provisional — before or contemporaneously with the first commercial engagement.

### Provisional applications: the twelve-month priority preserve

A provisional patent application under [35 U.S.C. § 111(b)](https://www.law.cornell.edu/uscode/text/35/111) is a lightweight filing that:

- Establishes a priority date (the provisional's filing date) that a subsequent non-provisional filed within twelve months can claim benefit of under § 119(e).
- Is not examined by the USPTO. It does not need claims in patentable form; it needs a written description that meets § 112's enablement requirement for the subject matter that the later non-provisional will claim.
- Is inexpensive relative to a non-provisional (USPTO fees are low; the substantive cost is attorney time drafting the specification — <!-- needs-research: verify current USPTO provisional filing fee for small entity, micro entity, and large entity; the small-entity fee has historically been in the low-hundreds-of-dollars range but should not be quoted without checking -->).
- Automatically abandons at twelve months if a non-provisional is not filed claiming its priority. There is no examination, no publication, and no continuing prosecution — the provisional either matures into a non-provisional within twelve months or lapses.

The stage-appropriate use of a provisional at Series-A is narrow: file a provisional on a *genuinely differentiating technique* the corporation has invented in-house, where the twelve-month window buys time to (a) validate that the technique is core to the product, (b) decide whether the technique should ultimately be patent-protected or trade-secret-protected, and (c) budget the non-provisional prosecution cost. Filing provisional after provisional on every idea the engineering team has is a pattern that produces a filing bill without producing patents; the discipline is to file few and file well.

Where a provisional is *not* appropriate: the invention is a straightforward application of well-known techniques (obviousness under § 103 will kill it), the corporation has already publicly disclosed the invention more than twelve months ago (§ 102 bars it), the invention is an abstract idea in the software / business-method space with no technical improvement over prior art (subject-matter eligibility under *Alice* will kill it), or the corporation's economics do not support the eventual non-provisional prosecution cost (a provisional that lapses is not a defensive asset).

### The software subject-matter problem: Alice, Mayo, Bilski

Software-implemented inventions occupy the most contested corner of patentable-subject-matter doctrine. The Supreme Court trilogy that governs the current framework:

- ***Bilski v. Kappos***, [561 U.S. 593 (2010)](https://supreme.justia.com/cases/federal/us/561/593/) — held that a business-method claim (a method of hedging risk in commodities trading) was an unpatentable abstract idea. Rejected the Federal Circuit's "machine-or-transformation" test as the sole test but left it as a useful clue.
- ***Mayo Collaborative Servs. v. Prometheus Labs., Inc.***, [566 U.S. 66 (2012)](https://supreme.justia.com/cases/federal/us/566/66/) — held that a diagnostic-method claim adding conventional steps to a natural correlation was unpatentable. Established the two-step framework: (i) is the claim directed to a judicial exception (abstract idea, natural phenomenon, law of nature)? (ii) if so, do the claim's other elements transform the claim into a patent-eligible application, adding "significantly more" than the exception itself?
- ***Alice Corp. Pty. Ltd. v. CLS Bank Int'l***, [573 U.S. 208 (2014)](https://supreme.justia.com/cases/federal/us/573/208/) — applied the *Mayo* framework to software claims. Held that a computer-implemented method of intermediated settlement was directed to an abstract idea and that generic computer implementation did not supply the "inventive concept" required at *Mayo* step two. *Alice* is the case that produced the current era of § 101 rejections for software and business-method claims.

The post-*Alice* practice, refined through Federal Circuit case law (*Enfish, LLC v. Microsoft Corp.*, 822 F.3d 1327 (Fed. Cir. 2016); *McRO, Inc. v. Bandai Namco Games America, Inc.*, 837 F.3d 1299 (Fed. Cir. 2016); *Berkheimer v. HP Inc.*, 881 F.3d 1360 (Fed. Cir. 2018)) and the USPTO's 2019 Revised Patent Subject Matter Eligibility Guidance, is that software claims can survive § 101 if they claim a specific technical improvement to computer functionality (a new data structure, a new caching approach, a new distributed-computing coordination mechanism) rather than an abstract idea implemented on generic hardware. The drafting response is to write claims that recite the technical improvement in structural terms rather than in "do X on a computer" terms.

For a Series-A software corporation, this doctrinal instability is a strong reason to be selective about patent filings on software algorithms. Many algorithms are better protected as trade secrets (see the patent-vs-trade-secret matrix below), and the ones that are worth filing on need drafting that clears *Alice* — which is skilled work and part of what the drafting cost reflects.

### The cost curve

A US utility patent from initial drafting through issuance runs roughly $15,000 – $25,000 in professional fees for a corporation of Series-A size and typical software / hardware complexity, with additional cost if prosecution involves multiple rounds of office actions or if the application is contested at appeal. <!-- needs-research: verify current market rates for utility-patent drafting through issuance for a US software patent at a Series-A software corporation; rates vary substantially by firm, complexity, and prosecution difficulty --> A provisional-only filing (drafted well) is typically a fraction of that — the substantive cost is the specification, which is largely reusable when the non-provisional is later drafted. Continuation applications, foreign filings, and post-grant proceedings add cost on top.

The material implication for stage planning: a corporation that files ten patents a year at Series-A is committing $150K – $250K annually to a portfolio it cannot enforce and that will not mature to issuance for three to five years. A corporation that files one carefully-selected provisional per year, converts the ones that still matter at the twelve-month mark, and re-evaluates the portfolio at each financing round, spends materially less and ends up with a better-selected portfolio.

### International filing: the PCT route

Patents are territorial. A US patent gives rights only in the United States; European rights require European filings, Japanese rights require Japanese filings, and so on. The **Patent Cooperation Treaty (PCT)** administered by [WIPO](https://www.wipo.int/pct/en/) is the mechanism most Series-A / B corporations use to preserve international priority without committing to the cost of national-phase filings up front.

The PCT sequence: file a US non-provisional (or a US provisional followed by a US non-provisional within twelve months, or a PCT application directly), then within twelve months of the earliest priority date file a **PCT international application** claiming that priority. The PCT application then has a **30-month priority preservation** window (from the earliest priority date) during which the applicant must enter the **national phase** in each jurisdiction where protection is sought — the [European Patent Office (EPO)](https://www.epo.org/), the [Japan Patent Office (JPO)](https://www.jpo.go.jp/e/), the [Canadian Intellectual Property Office (CIPO)](https://www.ic.gc.ca/eic/site/cipointernet-internetopic.nsf/eng/home), [IP Australia](https://www.ipaustralia.gov.au/), the [China National Intellectual Property Administration (CNIPA)](https://english.cnipa.gov.cn/), and so on.

The PCT is a priority-preservation mechanism, not an examination mechanism — the PCT international search and preliminary examination produce a searchable report but do not confer any actual patent. Every jurisdiction that ultimately grants a patent does so through its own national examination.

Practical Series-A / B posture: file domestically first, use the twelve-month convention-priority window (or the twelve-month PCT window from a US non-provisional) to file PCT for anything with plausible international commercial value, and then defer national-phase decisions to the thirty-month mark when the corporation has better information about which markets matter. The national-phase filings are the expensive step — translation costs, local counsel, jurisdiction-specific claim amendments — so deferring them is the primary point of the PCT.

### Stage-appropriate patent posture

The patent posture should track the corporation's stage:

- **Seed → early Series-A.** Typically no utility filings. At most, one provisional on a genuinely differentiating invention that the corporation is confident will remain core to the product and that has a plausible path through § 101 (i.e., a technical improvement, not an abstract-idea implementation). The paperwork cost of an over-broad early portfolio consistently outweighs its diligence value.
- **Series-A → Series-B.** Selective filings — perhaps one to three provisionals per year on genuinely-differentiating techniques, converted to non-provisionals at the twelve-month mark when the corporation is still confident of their commercial relevance. Begin building a defensive portfolio, and evaluate membership in a defensive-patent aggregator.
- **Series-B → Series-C.** Move toward a defensive portfolio with sufficient breadth that a competitor or NPE runs an infringement analysis before initiating suit. Selectively file abroad via PCT for inventions with international commercial value.
- **Growth stage.** Strategic filings supporting product-launch programmes and commercial-negotiation leverage; possibly cross-licensing discussions with strategic partners; formal FTO opinions on major product launches.

### Defensive-patent aggregators

Two established defensive-patent programmes are relevant to venture-backed corporations:

- **[LOT Network](https://lotnet.com/).** A cross-licensing network in which members agree that if any member's patent is transferred to a non-practising entity, that transfer triggers an automatic licence to all other members. The corporation retains the ability to enforce its own patents against competitors; the licence only triggers on transfer to an NPE. Membership is inexpensive (a tiered fee by revenue) and is a low-cost way to reduce troll exposure. <!-- needs-research: verify current LOT Network membership fee tiers; historically fees for revenue-under-$25M members have been low but should not be quoted without checking -->
- **[Open Invention Network (OIN)](https://openinventionnetwork.com/).** A patent-non-aggression community focused on Linux and open-source software. Members grant royalty-free licences to the "OIN Linux System" patents in exchange for reciprocal non-aggression from other members. Free to join and is a strong signal to the open-source community.

Both programmes are essentially free option value for a Series-A / B corporation with any software exposure and are commonly joined in the same year the corporation files its first patents.

## Trademark portfolio design

Trademarks are the highest-return IP filings at Series-A. They are inexpensive, quick to obtain relative to patents, and directly protect assets the corporation is actively investing in — the corporate name, the product name, and the associated goodwill. The Lanham Act ([15 U.S.C. § 1051 et seq.](https://www.law.cornell.edu/uscode/text/15/1051)) governs federal trademark registration; state trademark law and federal / state unfair-competition law provide the common-law substrate.

### Federal registration on the Principal Register

The [USPTO Principal Register](https://www.uspto.gov/trademarks) is the primary federal trademark register. Registration on the Principal Register carries four substantive benefits over unregistered (common-law) use:

- **Constructive notice** ([15 U.S.C. § 1072](https://www.law.cornell.edu/uscode/text/15/1072)) — nationwide notice to third parties of the registrant's claim of ownership, defeating good-faith later adopters in remote geographic areas.
- **Presumption of validity** ([15 U.S.C. § 1057(b)](https://www.law.cornell.edu/uscode/text/15/1057)) — the registration is prima facie evidence of the validity of the mark, of the registrant's ownership, and of the registrant's exclusive right to use the mark in commerce for the goods or services listed.
- **Incontestability after five years** ([15 U.S.C. § 1065](https://www.law.cornell.edu/uscode/text/15/1065)) — after five years of continuous post-registration use and a § 15 affidavit, the registration becomes largely immune to many challenges (including descriptiveness challenges) and is conclusive evidence of the registrant's exclusive right to use the mark in commerce.
- **Statutory damages, treble damages, and attorney fees** in counterfeiting cases ([15 U.S.C. § 1117](https://www.law.cornell.edu/uscode/text/15/1117)) — significantly stronger remedies than common-law relief.

Common-law rights (arising from actual use of a mark in commerce) exist and can be enforced, but are geographically limited to the areas of actual use and lack the presumptions and statutory damages of federal registration. For any Series-A corporation with more than local geographic ambition, federal registration is the standard.

### Intent-to-use filings

Section 1(b) of the Lanham Act ([15 U.S.C. § 1051(b)](https://www.law.cornell.edu/uscode/text/15/1051)) permits filing based on **bona fide intent to use** the mark in commerce, before actual use has begun. The intent-to-use filing preserves the priority date as of the filing date, but the registration does not actually issue until the applicant files either an Amendment to Allege Use (before publication) or a Statement of Use (after the Notice of Allowance) demonstrating actual use in commerce. Extensions of time to file the Statement of Use are available in six-month increments up to a total of thirty-six months from the Notice of Allowance.

This mechanism is what allows a corporation to secure a mark's priority date before the product has publicly launched — the corporation can file intent-to-use as soon as the naming decision is made, giving it a defensible priority date months or years before the public launch triggers common-law rights.

### TEAS Plus vs. TEAS Standard

The USPTO's electronic filing system offers two application tracks:

- **TEAS Plus** — lower filing fee per class of goods/services, but the applicant must select goods and services from the USPTO's pre-approved Trademark Identification (ID) Manual, must pay all fees up front, and must maintain compliance with a set of additional requirements (correspondence with USPTO must be electronic, applicant must have an email address on file, etc.).
- **TEAS Standard** — higher filing fee per class, more flexibility on goods-and-services identification (the applicant may write a custom description or draw from outside the ID Manual). Preferable when the corporation's goods or services do not fit cleanly into a pre-approved ID.

<!-- needs-research: verify current TEAS Plus and TEAS Standard per-class filing fees; the USPTO adjusts these periodically and the exact numbers should not be quoted without checking uspto.gov --> The practical guidance: file TEAS Plus when the goods/services fit a pre-approved ID cleanly; file TEAS Standard when a bespoke description is needed to accurately capture what the mark covers. Do not force an inaccurate ID selection just to qualify for TEAS Plus — an inaccurate description can create later problems if the actual use in commerce does not match.

### The Nice Classification and the temptation to over-file

The [Nice Classification](https://www.wipo.int/classifications/nice/en/) (International Classification of Goods and Services) organises goods and services into 45 international classes (34 goods classes and 11 services classes). US applications must specify one or more classes, and USPTO filing fees are per class. The relevant classes for most software / SaaS corporations:

- **Class 9** — downloadable software, computer programs.
- **Class 42** — computer / SaaS services, including "software as a service" and "platform as a service."
- **Class 35** — advertising, business management, business analytics services (sometimes appropriate for analytics-adjacent products).
- **Class 41** — educational and training services (relevant if the corporation ships training content).

The temptation is to file across many classes to "protect the mark broadly." This is often a mistake for two reasons: (i) each class has its own filing fee, so a five-class filing costs materially more than a two-class filing, and (ii) US law requires actual use in commerce of the mark for each class listed, and post-registration filings ([§ 8 declaration of use](https://www.law.cornell.edu/uscode/text/15/1058) at years 5–6 and every ten years thereafter) require re-attesting to that use. Registering in classes the corporation does not actually use exposes the registration to a fraud-on-the-USPTO challenge (see *In re Bose Corp.*, 580 F.3d 1240 (Fed. Cir. 2009), which raised the intent standard for fraud but did not eliminate the risk). The discipline is to file in the classes where the corporation actually offers goods or services, and add classes as the corporation actually expands.

### Trademark clearance discipline

Adopting a mark is a two-step search:

- **Knockout search.** A quick search of the USPTO TESS database (and equivalent state databases and common-law sources — Google, industry-specific directories, domain-name registrations) to eliminate marks that are obvious blockers. The knockout is cheap and should be done as soon as a naming candidate emerges. A well-run knockout narrows a set of five candidate names down to one or two viable ones in a day.
- **Full clearance search.** Once a candidate survives knockout, a professional full clearance search (often through a search vendor like Corsearch, Compumark, or Thomson CompuMark, with counsel review of the results) covers federal registrations, state registrations, common-law use, domain-name registrations, business-name registrations, phonetic equivalents, foreign registrations in relevant markets, and industry-specific databases. The full clearance produces an opinion letter (or informal counsel view) on the risk of adopting the mark. A full clearance search runs roughly $2,000 – $5,000 <!-- needs-research: verify current market rates for a full trademark clearance search including counsel opinion --> and is the standard due-diligence step before public launch and before intent-to-use filing.

The parallel workstream is **domain and social-handle acquisition** — the corporation should acquire the .com (and often the .io, .ai, .co, and country-code TLDs relevant to its international footprint), the primary social-media handles (Twitter/X, LinkedIn, GitHub, Instagram, YouTube, and whichever platforms are relevant to its go-to-market), and the app-store identifiers (if a mobile product is contemplated) *before* the public launch. Waiting until after launch gives cybersquatters and lookalikes a window to grab the corollary assets, and recovering them (via UDRP or purchase) is materially more expensive than acquiring them clean.

### International trademark: Madrid Protocol and direct filings

International trademark protection follows a broadly similar territorial pattern to patents but with a more usable central-filing mechanism. The [**Madrid Protocol**](https://www.wipo.int/madrid/en/) — implemented in the US under [15 U.S.C. § 1141](https://www.law.cornell.edu/uscode/text/15/1141) et seq. — allows a US registrant (or applicant) to file a single international application through WIPO designating multiple member jurisdictions. Each designated jurisdiction then examines the application under its own local law and either grants or refuses protection.

The Madrid Protocol's principal advantages are cost efficiency and centralised administration — a single filing designating twelve jurisdictions is substantially cheaper than twelve national filings, and the renewal and assignment mechanics are administered through WIPO. Its principal disadvantage is the **central-attack** vulnerability: for the first five years, the international registration depends on the underlying US "basic" application or registration, so a successful challenge to the US mark within that window collapses the entire international registration. For marks with any risk of US challenge, direct national filings — [EUIPO](https://euipo.europa.eu/ohimportal/en/) for the European Union, CIPO for Canada, IP Australia for Australia, JPO for Japan — avoid the central-attack risk at the cost of higher aggregate filing expense.

Stage-appropriate posture: Series-A corporations typically defer international trademark filings unless the go-to-market plan includes near-term international expansion. Series-B is the common inflection point for filing Madrid designations covering the major English-speaking markets and the European Union. Growth-stage corporations typically maintain a broader Madrid portfolio and direct filings in markets with material presence.

### Trademark policing

A registered mark is only as strong as its owner's willingness to police it. The core policing infrastructure:

- **Watch service.** A commercial trademark-watch service (Corsearch, Compumark, MarkMonitor, and similar) monitors USPTO and international registers for new applications for similar marks and issues periodic alerts. Cost is modest and the watch flags the applications the corporation should oppose *before* they publish for opposition, when opposition is procedurally straightforward.
- **Cease-and-desist workflow.** When infringing use is identified (whether by watch service, by internal detection, or by customer report), the corporation issues a cease-and-desist letter with the intent that the infringing user stop use, transfer any related domains, and (in some cases) agree to a coexistence arrangement. The C&D process is a graduated escalation — polite first letter, formal counsel-drafted second letter, filing suit if the response is inadequate.
- **UDRP and URS for domain disputes.** The Uniform Domain-Name Dispute-Resolution Policy ([UDRP](https://www.icann.org/resources/pages/help/dndr/udrp-en)) and the Uniform Rapid Suspension System ([URS](https://www.icann.org/resources/pages/urs-2014-01-09-en)) — both administered under ICANN — are administrative procedures for resolving disputes over domain names that are confusingly similar to a registered mark, registered in bad faith, and being used in bad faith. UDRP is the older and more thorough mechanism; URS is a faster and cheaper route for clear cases and produces suspension rather than transfer of the domain. A trademark policing programme should include UDRP / URS as the standard remedy for cybersquatting.

### Failure modes

- **Trademark loss through non-enforcement.** A registered mark that the owner does not police can become **generic** — the name of the good or service rather than a source identifier — and lose protection entirely. The canonical examples (Aspirin, Escalator, Thermos, Kleenex before rehabilitation) are cautionary. The corporation's marketing programme should always use the mark as an adjective ("the Acme product," not "the Acme"), with the appropriate registration symbol (® for registered marks, ™ for unregistered marks in trademark use, ℠ for unregistered service marks), and the trademark-use policy should be enforced against internal and external misuse.
- **Adopting a merely-descriptive mark.** Under [15 U.S.C. § 1052(e)](https://www.law.cornell.edu/uscode/text/15/1052), marks that are "merely descriptive" of the goods or services are not registrable on the Principal Register absent proof of acquired distinctiveness (secondary meaning) under § 2(f). A mark like "Best Analytics Software" is merely descriptive and will not register; a suggestive, arbitrary, or fanciful mark ("Snowflake" for a data warehouse, "Kodak" for photographic film) is registrable on first use. Founder-favourite descriptive names are a common failure mode; the clearance discipline should catch this before intent-to-use filing.
- **Failing to conduct full clearance before public launch.** Launching a product under a name that later turns out to conflict with a senior mark forces a rebrand — expensive, brand-diluting, and (if the senior mark holder is aggressive) potentially litigation-triggering. The full clearance search before public launch is inexpensive relative to a rebrand.
- **Filing across unused classes.** The Nice-class over-filing pattern discussed above; exposes registration to abandonment or fraud challenges.

## Copyright registration for high-value creative works

Copyright is the least intentional of the four IP regimes at a Series-A corporation — it vests automatically on fixation and requires no filing or registration to exist. What *registration* provides is procedural and remedial standing that meaningfully changes the enforcement calculus for a handful of high-value creative works.

### Copyright vests on fixation

Under [17 U.S.C. § 102](https://www.law.cornell.edu/uscode/text/17/102), copyright protection subsists "in original works of authorship fixed in any tangible medium of expression" — the moment a work is written down, saved to disk, or otherwise fixed, copyright exists. No registration is required for the copyright to exist. The categories of copyrightable works include literary works (which under the statute includes computer software), musical works, dramatic works, pictorial / graphic / sculptural works, motion pictures and audiovisual works, sound recordings, and architectural works.

For a software / SaaS corporation, the practical scope of copyrightable material is broad: source code, compiled binaries, product documentation, marketing copy, whitepapers and technical publications, blog posts, product screenshots and UI illustrations, marketing videos, sales-deck imagery, and (with some doctrinal complexity) UI designs where sufficiently original. All of this is protected by copyright the moment it is authored.

### Registration as a precondition to suit

Even though copyright vests on fixation, [17 U.S.C. § 411(a)](https://www.law.cornell.edu/uscode/text/17/411) requires that a US work be **registered** (or the registration application at minimum acted on by the Copyright Office) before the copyright owner can file an infringement suit in federal court. The Supreme Court in ***Fourth Estate Public Benefit Corp. v. Wall-Street.com, LLC***, [586 U.S. 296 (2019)](https://supreme.justia.com/cases/federal/us/586/296/), resolved a long-running circuit split by holding that "registration has been made" within the meaning of § 411(a) when the Copyright Office actually *acts on* the application (grants or refuses registration), not when the application is merely filed. In practical terms: for a US work, the corporation cannot sue for infringement until the Copyright Office has processed the registration application, which takes months in the ordinary course (and can be accelerated via special-handling fees for expedited processing).

The practical implication: waiting until infringement occurs to register is too late — the corporation faces months of delay before it can file suit, during which the infringement may be doing material damage.

### Statutory damages and attorney fees under § 412

The remedial advantage of pre-infringement registration is even more consequential. [17 U.S.C. § 412](https://www.law.cornell.edu/uscode/text/17/412) bars an award of **statutory damages** under § 504(c) and **attorney fees** under § 505 for any infringement of an *unpublished* work that occurred before registration, and for any infringement of a *published* work that occurred more than three months after first publication and before the effective date of registration.

Statutory damages under [17 U.S.C. § 504(c)](https://www.law.cornell.edu/uscode/text/17/504) range from $750 to $30,000 per work infringed at the court's discretion, increased to up to $150,000 for wilful infringement and reduced to as low as $200 for innocent infringement. Statutory damages matter because they allow the copyright owner to recover without proving actual damages — which for many software / content-piracy scenarios are hard to quantify — and to recover attorney fees under § 505 as prevailing party, which changes the economics of enforcement.

The **three-month post-publication window** is the operational anchor: for any published work the corporation cares about, register within three months of publication and pre-infringement statutory damages / attorney fee eligibility is preserved. Missing that window forfeits the enhanced remedies for prior infringement.

### Work-made-for-hire doctrine

Under [17 U.S.C. § 201(a)](https://www.law.cornell.edu/uscode/text/17/201), copyright vests initially in the author. Section 201(b) provides the **work-made-for-hire** exception: where a work is a work made for hire, the employer or party for whom the work was prepared is considered the author for copyright purposes. Section 101 defines "work made for hire" in two mutually-exclusive ways:

- A work prepared by an **employee** within the scope of their employment; **or**
- A work specially ordered or commissioned for use as one of **nine specifically enumerated categories** (contribution to a collective work, part of a motion picture or other audiovisual work, translation, supplementary work, compilation, instructional text, test, answer material for a test, or atlas), **if** the parties expressly agree in a written instrument signed by them that the work is a work made for hire.

For **employee** authorship the analysis is scope-of-employment (see *Community for Creative Non-Violence v. Reid*, 490 U.S. 730 (1989) for the multi-factor employee-vs-independent-contractor test that governs). Copyright vests in the corporation automatically, provided the work is within the scope of employment. The employee's PIIA belt-and-suspenders assigns any copyright that does not vest via § 201(b) directly to the corporation.

For **non-employee (independent contractor)** authorship, the nine-category test is narrow. Most software work does not fit any of the nine categories cleanly (software is not "contribution to a collective work" or "part of a motion picture" in the statutory sense), which means work-made-for-hire status frequently does not apply to contractor-authored software even if the SOW recites the incantation. The remedy is the **belt-and-suspenders assignment** — the contractor SOW recites work-made-for-hire *and*, in the alternative if work-made-for-hire does not apply, includes a present-tense written assignment of all right, title, and interest in the work to the corporation. See [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md) on vendor SOWs for the drafting pattern.

### Which works to register

Copyright registration costs roughly $65 per work online through the [Copyright Office eCO system](https://www.copyright.gov/registration/), with higher fees for paper filings and expedited processing. <!-- needs-research: verify current Copyright Office online single-application filing fee; historically has been $45 – $65 for single-application single-author works but the fee schedule is periodically updated --> The universe of copyrightable works the corporation produces is far broader than what warrants registration; the discipline is to register the material creative works where enforcement is plausibly worth the effort.

The typical Series-A registration slate:

- **Core marketing collateral** — the company's flagship whitepaper, its published research reports, its widely-distributed content pieces. These are the works most likely to be scraped, republished, or plagiarised by competitors.
- **Technical documentation** — the corporation's published API documentation, developer guides, and technical books (if the corporation has published a book-length technical work).
- **Product documentation** where verbatim copying by competitors is a realistic concern.
- **Published open-source projects** — if the corporation has released its own open-source project (see [chapter 05](./05-open-source-hygiene-and-sbom-programme.md)), the copyright registration in the codebase enables the corporation to enforce license terms against a violator.
- **Marketing videos and imagery** with meaningful production value.

Source code registration is possible but less common in practice — the Copyright Office's software registration procedures permit registering the first and last 25 pages of source code (with trade-secret redactions) to establish a registration record without publicly disclosing the code. Whether to register source code copyright is a stage-appropriate decision — most Series-A corporations rely on trade-secret protection for source code and register only if enforcement against a specific infringer is contemplated.

## Trade-secret protection programme

Trade secrets are the workhorse IP regime for most software corporations. The scope of what a trade secret can cover — customer lists, business plans, unpublished algorithms, source code, product roadmaps, pricing structures, financial models, technical know-how — is broader than any of the registration-based regimes, the duration is indefinite (or, at least, until public disclosure, independent invention, or reverse engineering), and the cost of establishing protection is the cost of running a competent security-and-confidentiality programme (which the corporation should be running anyway).

### The DTSA and its federal cause of action

The **Defend Trade Secrets Act of 2016** ([18 U.S.C. § 1836](https://www.law.cornell.edu/uscode/text/18/1836) et seq.) established a federal civil cause of action for trade-secret misappropriation. Before the DTSA, trade-secret enforcement was almost entirely a state-law matter under state adoptions of the Uniform Trade Secrets Act. The DTSA now provides federal-court jurisdiction, uniform national procedural rules, and remedies including injunctive relief, damages (actual damages plus unjust enrichment), reasonable royalty in lieu of damages, exemplary (double) damages for wilful and malicious misappropriation, and attorney fees for wilful and malicious misappropriation.

The DTSA also includes an **ex parte seizure** provision ([§ 1836(b)(2)](https://www.law.cornell.edu/uscode/text/18/1836)) allowing a court, in extraordinary circumstances, to order seizure of property necessary to prevent the propagation of a misappropriated trade secret — a powerful remedy that has been used sparingly.

### The "reasonable measures" requirement

The DTSA's definition of trade secret ([18 U.S.C. § 1839(3)](https://www.law.cornell.edu/uscode/text/18/1839)) has three elements:

- (A) the owner has taken **reasonable measures** to keep the information secret;
- (B) the information derives independent economic value, actual or potential, from not being generally known to, and not being readily ascertainable by, another person who can obtain economic value from the disclosure or use of the information; and
- (C) the information is not generally known to, or readily ascertainable through proper means by, another person who can obtain economic value from the disclosure or use of the information.

The **reasonable-measures** element is the operational one — if the corporation cannot demonstrate that it took reasonable steps to keep the information secret, the information is not a trade secret regardless of its actual economic value. What counts as "reasonable" is fact-specific and scaled to the corporation's size and sophistication; courts do not require a Fortune-500 security programme from a twenty-person startup but do require *some* documented, operational programme.

### The DTSA whistleblower-immunity notice

[18 U.S.C. § 1833(b)(3)](https://www.law.cornell.edu/uscode/text/18/1833) requires that any contract or agreement with an employee (a term the statute defines broadly to include contractors and consultants) that governs the use of a trade secret or other confidential information include **notice of the immunity** provided under § 1833(b)(1) and (2) — the immunity from criminal or civil liability under any federal or state trade-secret law for disclosure of a trade secret (a) in confidence to a federal, state, or local government official or to an attorney, solely for the purpose of reporting or investigating a suspected violation of law; or (b) in a complaint or other document filed in a lawsuit or other proceeding, if filed under seal.

The consequence of failing to include this notice is codified in § 1833(b)(3)(C): the corporation may not recover exemplary damages or attorney fees against an employee to whom notice was not provided. That is a materially worse enforcement posture and is one of the most easily-avoided drafting failures.

The notice can be given directly in the confidentiality / PIIA / NDA agreement, or the agreement can cross-reference a separate policy document containing the notice. See [mod-102 chapter 05](../mod-102-founding-team-legal-architecture/05-dtsa-whistleblower-and-trade-secret-baseline.md) for the founder-level DTSA baseline, [mod-103 chapter 04](../mod-103-employment-law-and-contract-design/04-employee-piia.md) for the employee-PIIA implementation, and [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md) for the vendor / contractor NDA implementation. All three should include the DTSA notice; if any one omits it, the corresponding population is not covered for exemplary damages.

### UTSA and state trade-secret law

The **Uniform Trade Secrets Act** (UTSA), promulgated by the Uniform Law Commission, has been adopted (with variations) by 48 states and the District of Columbia. **New York** is the notable non-adopter and continues to apply common-law trade-secret doctrine (which produces broadly similar outcomes with idiosyncratic proof requirements). Massachusetts historically was also a non-adopter but adopted a modified UTSA in 2018.

State law and federal DTSA claims can be — and typically are — pleaded together. The DTSA does not preempt state trade-secret law, and the plaintiff selects among available theories at pleading. The state-federal overlap generally works in the plaintiff's favour: the DTSA supplies federal jurisdiction and uniform procedure, while state law supplies additional theories, sometimes different damages calculations, and (in a few states) statutory attorney-fee provisions.

### The operational programme

The reasonable-measures requirement is satisfied by an operational trade-secret programme with the following components. Each is table stakes at Series-A / B:

- **Identification and classification.** A written data-classification policy identifies categories of information the corporation treats as confidential and trade-secret. A common four-tier structure: **Public** (marketing materials, public documentation), **Internal** (routine internal communications, non-sensitive operational data), **Confidential** (customer data, employee data, financial data, business plans), **Trade Secret** / **Restricted** (source code, unpublished algorithms, customer-specific pricing, unfiled inventions, M&A pipeline). The policy specifies handling requirements for each tier.
- **Access controls.** Least-privilege access with role-based access controls, multi-factor authentication for all systems that hold Confidential or Trade Secret information, and periodic (typically quarterly) access reviews. Repositories containing trade-secret material (source code repositories, model repositories, sensitive data lakes) should require MFA and, ideally, hardware-key second factors for engineers with production access.
- **Physical and digital marking.** Documents and data assets classified as Confidential or Trade Secret should be marked as such — a footer or watermark on documents, a header comment or metadata tag on code, a classification label in the data catalogue. Marking is procedurally useful evidence that the corporation identified the information as confidential; it also makes downstream mishandling easier to spot.
- **Personnel controls (PIIA).** Every employee signs a PIIA on hire assigning all IP and imposing continuing confidentiality obligations, with the DTSA whistleblower notice ([mod-103 chapter 04](../mod-103-employment-law-and-contract-design/04-employee-piia.md)). The PIIA should specifically identify categories of confidential information and specify handling obligations that continue post-termination.
- **Vendor and contractor controls (NDA / PIIA).** Every contractor, consultant, professional-services vendor, and adviser signs an NDA (or an SOW with confidentiality obligations) with equivalent obligations and the DTSA notice ([chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md)).
- **Exit interviews and IP-return protocol.** Every departing employee is exited through a standard checklist that (i) reminds them of continuing confidentiality obligations, (ii) requires return of all corporation devices and materials, (iii) requires certification that no confidential information has been retained, and (iv) documents any invention or work-product ownership questions. The exit interview creates an evidentiary record that the corporation reasserted its trade-secret rights at departure — a fact that materially strengthens later enforcement against a departed employee.
- **Audit trail.** Logging of access to trade-secret repositories, of document downloads and exports, of privileged-account use. In the event of misappropriation, the audit trail is the evidentiary foundation for both the pleading (specific documents accessed on specific dates by specific users) and the eventual damages case. Retention of audit logs is a records-retention policy question — see [mod-101 chapter 03](../mod-101-legal-entity-formation-and-corporate-structure/03-corporate-record-and-compliance-calendar.md) for the corporate records framing.

The programme should be **documented** — a written trade-secret policy, a data-classification policy, an access-review procedure, an offboarding procedure — so that in litigation the corporation can produce the policies as evidence that reasonable measures existed. Actual behaviour and written policy should match; a documented programme that is not followed in practice is worse than no policy at all.

## The patent-vs-trade-secret decision matrix

For any given invention, the corporation faces a choice: file a patent (public disclosure in exchange for a defined-term monopoly), keep it as a trade secret (indefinite protection but only against improper disclosure and use), or defensively publish (create prior art to block competitors without patenting yourself). The matrix that governs the decision:

| Dimension | Patent | Trade secret |
|---|---|---|
| Duration | 20 years from filing (35 U.S.C. § 154) | Indefinite while secret |
| Public disclosure required | Yes — the specification is published (§ 122) | No — protection depends on secrecy |
| Protects against independent invention | Yes | No |
| Protects against reverse engineering | Yes | No |
| Requires ongoing investment | Prosecution, maintenance fees | Ongoing security programme |
| Enforcement remedy | Injunction, damages, treble for wilful | Injunction, damages, DTSA exemplary damages |
| Subject-matter limits | § 101 abstract-idea limits post-*Alice* | Broad — no subject-matter limits |
| Effective against copying | Yes (if valid and infringed) | Yes (if misappropriation proven) |

### Software algorithms typically go trade-secret

For most software algorithms, trade-secret protection is the better economic choice. The reasoning:

- **Patent-subject-matter uncertainty.** Post-*Alice*, software claims face a materially higher rejection rate under § 101 and materially higher invalidation risk in post-grant proceedings. Filing a patent that is later invalidated is worse than not filing — the invention is now publicly disclosed *and* unprotected.
- **Detection difficulty.** Enforcing a patent requires detecting infringement. Server-side software algorithms are usually not observable from the outside; a competitor implementing the same algorithm on its own servers is functionally undetectable unless a former employee documents the copying. If detection is unlikely, the patent's exclusionary force is limited.
- **Independent development is likely.** Well-known algorithmic patterns are frequently reinvented; a patent that is easily worked-around or independently developed provides limited exclusivity.
- **Reverse-engineering resistance.** Server-side algorithms cannot be reverse-engineered by customers (unlike an on-premises binary), so the trade-secret alternative provides essentially the same protection against improper acquisition.

For these reasons, the practitioner canon for most SaaS-backend algorithmic work is trade-secret protection through a documented internal programme, with a defensive-publication mechanism (see below) for algorithms that need to be kept out of competitors' patent portfolios but that the corporation does not want to patent itself.

### Hardware innovations more often go patent

For hardware inventions, the calculus reverses. Hardware is often observable — a competitor's device can be purchased, torn down, and studied. Reverse engineering of hardware is a well-established discipline and is a "proper means" of acquiring information that defeats trade-secret protection. Independent development of a differentiated hardware architecture is often unlikely without access to the original design. Detection of infringement is straightforward — a competitor's product embodying the invention can be examined.

For a corporation with any hardware component to its product, the default posture is patent-protect the hardware innovations and trade-secret-protect the software and know-how. Combination inventions with both hardware and software elements typically get filed on the hardware aspects with claims constructed to capture the technical improvement.

### The defensive-publication route

A third option, distinct from patenting or trade-secret protection, is **defensive publication** — publishing a description of the invention in a form that qualifies as prior art under § 102, defeating any later third-party patent application on the same invention without the corporation itself patenting.

The historical mechanism was the IBM Technical Disclosure Bulletin, published from 1958 to 1998, in which IBM engineers published invention disclosures precisely to establish prior art without the cost of patenting. The modern practitioner-canon substitutes:

- **[arXiv](https://arxiv.org/) preprint posts.** For algorithms with academic-adjacent content, a preprint on arXiv establishes a public disclosure with a timestamp and is regularly cited as prior art in patent office rejections.
- **[IP.com](https://ip.com/) defensive publications.** IP.com maintains a searchable defensive-publications database explicitly designed for this purpose; a publication there is a low-cost, USPTO-searchable prior-art creation. <!-- needs-research: verify current IP.com defensive publication fee schedule; historically has been in the low-hundreds-of-dollars range but should not be quoted without checking -->
- **[Research Disclosure journal](https://www.researchdisclosure.com/).** A commercial journal published for defensive-publication purposes; USPTO examiners search its indexes as part of patent-examination prior-art searches.
- **Corporation-hosted blog posts and technical publications.** With appropriate timestamping and searchable indexing (Google indexes the corporation's website, and archive.org's Wayback Machine provides independent timestamp evidence), a corporation-hosted publication can serve as prior art. Less procedurally clean than IP.com or Research Disclosure but usable.

The defensive-publication decision is orthogonal to the trade-secret decision — the corporation cannot defensively publish *and* keep an invention as a trade secret (publication destroys the secret). The three-way choice is:

- **Trade secret** — keep it internal, protect via the programme.
- **Patent** — disclose in exchange for exclusivity.
- **Defensive publication** — disclose to block others without patenting.

The rare corporation gets to all three modes for different inventions; the discipline is to make the decision consciously per invention rather than by default.

## The IP-holding-company structure

Some corporations elect to house their IP in a separate Delaware or Nevada holding subsidiary that licenses back to operating subsidiaries. The structural logic:

- **Bankruptcy remoteness of IP.** If the operating subsidiary encounters financial distress, the IP owned by a separate holding entity is (in theory) not part of the operating entity's bankruptcy estate — potentially preserving the asset for reorganisation or sale outside the operating entity's insolvency.
- **Licensing income and tax structuring.** In the historical structuring, IP-holding subsidiaries in low-tax jurisdictions (Delaware, Nevada, and internationally the double-Irish and Dutch-sandwich structures) generated licensing income at low or zero effective tax rates. Most of these structures have been substantially curtailed by the 2017 Tax Cuts and Jobs Act (GILTI, FDII, BEAT provisions) and the OECD BEPS framework, but domestic Delaware / Nevada holding structures still have some tax advantages in specific state-tax scenarios.
- **Facilitates future licensing programmes.** If the corporation intends to build a licensing programme (patent licensing, brand licensing, technology-transfer licensing), the holding-company structure separates the licensing business from the operating business cleanly.

The trade-offs:

- **Complexity and administrative cost.** Two entities to maintain, two sets of corporate records, two annual reports, transfer-pricing documentation for the intercompany license, transfer-pricing risk if the licensing rates cannot be defended as arm's-length.
- **Tax analysis is genuinely complex.** State-tax treatment (some states have addressed IP-holding structures with income-adjustment or throwback rules), transfer-pricing compliance under Treas. Reg. § 1.482, GILTI implications if any structure is international. **This chapter does not own the tax analysis** — the tax structuring should be run by qualified tax counsel and, for material structures, a corporate tax adviser.
- **Diligence complexity.** Buy-side counsel in an M&A transaction will diligence the IP-holding structure and the intercompany license carefully; a poorly-structured intercompany license can create diligence friction.

For a Series-A corporation, the default is *not* to implement an IP-holding structure — the operating C-corp owns its own IP directly, and the cost / benefit does not justify the complexity. The question typically reopens at Series-C / growth stage, at pre-IPO restructuring, or in connection with an international-expansion programme. See [mod-101](../mod-101-legal-entity-formation-and-corporate-structure/) for the general entity-structuring framing.

## IP-diligence readiness

A Series-A, B, or C financing round and an M&A transaction each produce an IP diligence workstream. The buy-side counsel — Wilson Sonsini, Cooley, Latham, Gunderson, Fenwick, or the equivalent — will request a defined set of artefacts. The corporation that can deliver them on day one of diligence closes faster and at better terms than the corporation that has to reconstruct them under time pressure.

The standard IP-diligence request list:

- **Patent schedule.** All patents (issued and pending), including patent applications and provisionals, with filing dates, issuance dates, inventors, and assignee. If any inventor is not an employee (or was not at the time of invention), the assignment chain from the inventor to the corporation.
- **Trademark schedule.** All registered and pending trademark registrations, with jurisdictions, classes, first-use dates, and registration numbers. Any common-law marks the corporation asserts.
- **Copyright registration schedule.** All registered copyrights, with registration numbers and dates. (Unregistered copyrights are not typically scheduled because they are not distinctively identified.)
- **Chain-of-title evidence for each material IP asset.** For each patent, trademark, or registered copyright material to the corporation's business, evidence that the corporation actually owns it — inventor assignments, contractor IP assignments, founder pre-formation IP transfers ([mod-102](../mod-102-founding-team-legal-architecture/)), employment PIIAs.
- **PIIA coverage of every past and current employee and contractor.** The single most common diligence finding is a former employee or contractor without a signed PIIA — a gap in chain of title. The corporation should be able to produce, on request, a schedule showing that every past and current employee, founder, contractor, consultant, and adviser executed either a PIIA or an IP-assignment SOW. See [mod-103](../mod-103-employment-law-and-contract-design/) and [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md).
- **Open-source scan and SBOM.** A current CycloneDX or SPDX SBOM and evidence that the OSS-approval policy has been enforced ([chapter 05](./05-open-source-hygiene-and-sbom-programme.md)). Discovering a GPL or AGPL dependency shipped into a proprietary product mid-diligence is a common deal-slowing surprise.
- **Trade-secret programme documentation.** The data-classification policy, the confidentiality policy, evidence of access controls and access reviews, the standard PIIA / NDA templates with DTSA notice, the offboarding checklist.
- **Third-party IP licences.** All inbound licences (open-source in the SBOM plus any commercial third-party IP the corporation depends on); any outbound licences the corporation has granted.
- **IP-litigation and dispute schedule.** Any pending or threatened IP litigation, cease-and-desist letters sent or received, opposition proceedings, and post-grant proceedings.
- **The "IP indemnity we're giving customers is defensible" trail.** A representative MSA showing the IP indemnity, together with evidence that the internal chain-of-title, PIIA coverage, and OSS hygiene support the corporation's ability to honour the indemnity.

The diligence goal is not zero findings — some findings are expected and are addressed through reps-and-warranties, disclosure schedules, or specific covenants. The goal is *no surprises* — the corporation has flagged every issue itself, has an explanation for each, and is not caught out by the buy-side counsel finding something the corporation did not know about. Diligence-readiness is a continuous discipline, not a pre-transaction sprint; the corporation that runs its IP paperwork cleanly year-round arrives at the diligence conversation prepared.

## Ownership boundary

This chapter covers the corporation's strategic IP layer — what to file, what to keep as trade secret, how to structure the portfolio, and how to prepare for diligence. It defers:

- **Founder-era pre-formation IP transfers and founder PIIAs** — [mod-102](../mod-102-founding-team-legal-architecture/), particularly [mod-102 chapter 04](../mod-102-founding-team-legal-architecture/04-piia-mutual-ip-assignment.md) and [chapter 05](../mod-102-founding-team-legal-architecture/05-dtsa-whistleblower-and-trade-secret-baseline.md).
- **Employee PIIA and DTSA whistleblower notices in employment contracts** — [mod-103](../mod-103-employment-law-and-contract-design/), particularly [chapter 04](../mod-103-employment-law-and-contract-design/04-employee-piia.md) and [chapter 05](../mod-103-employment-law-and-contract-design/05-nda-and-mnda-layer.md).
- **Contractor / consultant IP-assignment mechanics in vendor SOWs** — [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md).
- **Open-source licence hygiene and SBOM programme** — [chapter 05](./05-open-source-hygiene-and-sbom-programme.md).
- **Privacy and data-governance overlap with trade-secret protection for personal data** — [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/).
- **Entity structuring for any IP-holding subsidiary** — [mod-101](../mod-101-legal-entity-formation-and-corporate-structure/).
- **The tax analysis of IP-holding structures** — outside this chapter's scope; requires qualified tax counsel.

## Concrete example: a Series-A B2B SaaS corporation authors its IP programme

Acme Analytics is a ~30-engineer Series-A B2B SaaS corporation (Delaware C-corp, SaaS platform delivered from AWS). It has just closed its Series-A ($18M led by a top-tier venture firm) and its General Counsel — either a fractional GC or the first-legal-hire — is authoring the corporation's IP programme.

**Patents.** Acme files **no utility patents** in the Series-A year. Its core technology is a set of software algorithms in the analytics-platform space — subject-matter risk under *Alice* is meaningful, detection of infringement server-side is essentially impossible, and independent development by competitors is likely. Trade-secret protection is the better economic choice for the algorithmic work. The corporation does file **one defensive provisional** on a genuinely differentiating technique — a novel approach to incremental materialisation of query results that the CTO believes is materially better than published prior art and that has plausible § 101 claim structure (specific technical improvement to computer functionality, not an abstract-idea implementation). The provisional buys twelve months to decide whether to convert to a non-provisional. Acme joins **LOT Network** at Series-A ($1K – $2K annual fee for a corporation of its size, <!-- needs-research: verify current LOT Network fee tier for Acme's revenue band -->) as inexpensive troll-defence.

**Trademarks.** Acme files a **USPTO Principal Register application** for its company name in **Nice class 42** (SaaS / computer services) and **class 9** (downloadable software). Founder-favourite descriptive names had been evaluated at naming time; the actual name is arbitrary and cleared through a **full clearance search** performed by counsel via a search vendor before public launch. A **knockout search** had already eliminated three competing candidates. The filing is **TEAS Standard** because the corporation's actual services description is bespoke enough that the pre-approved TEAS Plus IDs do not fit cleanly. Filing is intent-to-use under § 1(b), converted to actual use six months later when public launch triggers the Amendment to Allege Use. **Domain acquisition** — the .com, .io, .ai, and the country-code TLDs for the corporation's identified target markets — was completed before the naming decision was public. **Social handles** — Twitter/X, LinkedIn, GitHub, YouTube — were secured on the same day. **Madrid Protocol** international filings are **deferred to Series-B**, when the go-to-market plan will include material international expansion. Acme subscribes to a **trademark watch service** and has a written **cease-and-desist workflow** that routes infringing-use reports through the General Counsel.

**Copyright.** Acme identifies a defined **registration slate**: (i) the corporation's flagship whitepaper (published at Series-A launch), (ii) two published technical blog posts that saw high external distribution, (iii) the developer-facing API documentation, (iv) the corporation's marketing launch video, and (v) the source code and documentation for its one released open-source utility library. Each is registered within the **three-month post-publication window** to preserve statutory-damages and attorney-fee eligibility under § 412. Source code for the proprietary platform is not registered — trade-secret protection is the primary regime; registration will be considered if an enforcement action is contemplated. Every employee's PIIA and every contractor's SOW contains the **work-made-for-hire recital plus present-tense assignment** (the belt-and-suspenders construction), so that for both employee and non-employee-authored works, copyright is either automatically the corporation's or has been assigned to it.

**Trade-secret programme.** Acme's programme has the components required for reasonable-measures compliance:

- **Data-classification policy.** Four tiers (Public, Internal, Confidential, Trade Secret), with handling requirements for each. Owned by the Head of Security.
- **Access controls.** MFA required for all corporate accounts (Google Workspace, GitHub, AWS, HRIS, CRM). Hardware-key second factors required for engineers with production access. Source code repositories are private and access-audited. Quarterly access reviews signed off by the Head of Engineering.
- **Marking.** Confidential documents footer-marked; source code repositories tagged Trade Secret in the data catalogue; NDA-covered materials watermarked.
- **PIIA templates.** All employees on hire sign a PIIA with (i) IP assignment, (ii) confidentiality obligations continuing post-termination, (iii) DTSA whistleblower notice under § 1833(b), (iv) return of materials obligation on termination. See [mod-103 chapter 04](../mod-103-employment-law-and-contract-design/04-employee-piia.md).
- **NDA / SOW templates.** All contractors and consultants sign NDAs with the DTSA notice; SOWs include the belt-and-suspenders IP-assignment construction. See [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md).
- **Offboarding protocol.** Every departing employee is exited through the checklist — remind of continuing obligations, collect devices, certify no-retention, document any IP-ownership questions. The exit interview is documented in the HRIS and preserved as evidence.
- **Audit trail.** GitHub, AWS CloudTrail, Google Workspace audit logs, and HRIS logs are ingested into a central log store with 7-year retention. Access to trade-secret repositories is logged and reviewable.

**Defensive publication.** For algorithmic work Acme has decided *not* to patent but wants to keep out of competitors' portfolios, Acme uses a lightweight defensive-publication mechanism: internal engineering blog posts describing the technique are re-published, with lightly-redacted implementation detail, either on the corporation's public engineering blog (indexed by Google, timestamped) or as arXiv preprints (for work with academic-adjacent content). Two publications per year is the working pace.

**Diligence readiness.** In the Series-B round eighteen months later, Acme delivers to the buy-side counsel on day one of the IP diligence workstream: the patent schedule (one provisional, now converted to a non-provisional under prosecution, with the assignment from the CTO on file); the trademark schedule (US registration issued, with class 9 and 42 coverage, and the § 8 declaration of use filing calendar noted); the copyright schedule (five registered works); the PIIA / SOW coverage schedule (100% of employees, 100% of active contractors, 100% of past employees back to the founding date, with the DTSA notice in all templates); the current CycloneDX SBOM ([chapter 05](./05-open-source-hygiene-and-sbom-programme.md)) with zero disapproved licences; the trade-secret programme documentation. The IP diligence workstream closes in five business days rather than becoming a deal-timing constraint.

## Summary

- IP strategy at Series-A is not a litigation programme — it is a diligence artefact, a defensive shield, a commercial-negotiation lever, and the substrate that makes the customer MSA's IP indemnity ([chapter 01](./01-customer-contract-suite-msa-sla-dpa-security-aup.md)) defensible.
- Patents (35 U.S.C. §§ 101, 102, 103, 112, 154) impose a first-inventor-to-file regime with a one-year on-sale / public-disclosure grace period, a 20-year term from filing, and — for software — the post-*Alice* / *Mayo* / *Bilski* subject-matter constraints that require claiming a specific technical improvement rather than an abstract idea. Cost per US utility patent runs roughly $15K – $25K from drafting through issuance.
- The stage-appropriate patent posture at Series-A is typically no utility filings or at most one defensive provisional under 35 U.S.C. § 111(b) on a genuinely differentiating invention. International priority preservation is via the Patent Cooperation Treaty (PCT) with 30-month national-phase deferral. Membership in a defensive-patent aggregator (LOT Network, Open Invention Network) is inexpensive troll-defence.
- Trademark registration on the USPTO Principal Register (Lanham Act, 15 U.S.C. § 1051 et seq.) provides constructive notice, presumption of validity, incontestability after five years, and statutory damages that materially exceed common-law rights. Intent-to-use filings under § 1(b) preserve priority before actual use; TEAS Plus / TEAS Standard choose based on ID fit; Nice-class discipline avoids over-filing fraud risk; full clearance search precedes public launch; Madrid Protocol under 15 U.S.C. § 1141 handles international coverage with the central-attack trade-off vs. direct EUIPO / CIPO / JPO / IP Australia filings.
- Copyright vests on fixation (17 U.S.C. § 102) but registration is a precondition to a US infringement suit under *Fourth Estate*, 586 U.S. 296 (2019), and pre-infringement (or within three months of first publication) registration is required to unlock statutory damages under § 504(c) and attorney fees under § 505. Work-made-for-hire (§ 201(b)) plus belt-and-suspenders present-tense assignment covers both employee and contractor authorship. The registration slate is targeted at high-value creative works: flagship whitepapers, technical documentation, published open source, marketing videos.
- Trade-secret protection under the DTSA (18 U.S.C. § 1836 et seq.) and UTSA is the workhorse regime for software algorithms and confidential business information. It requires demonstrable reasonable measures under § 1839(3)(A) — the operational programme (identification, access controls, marking, PIIA / NDA coverage, offboarding, audit trail). The DTSA whistleblower-immunity notice under § 1833(b) is required in every employee and contractor confidentiality agreement to preserve exemplary damages and attorney fees.
- The patent-vs-trade-secret decision follows the observability and detectability of the invention: software algorithms typically go trade-secret (Alice-era subject-matter uncertainty, undetectable server-side implementation, reverse-engineering-resistant); hardware innovations more often go patent (observable, reverse-engineerable, detectable in a competitor's product). The defensive-publication route (arXiv, IP.com, Research Disclosure, corporation-hosted publication) is the third-path option for inventions that need to be kept out of competitors' portfolios without being patented or held as trade secret.
- The IP-holding-company structure — parking IP in a Delaware or Nevada holding subsidiary that licenses back to the operating entity — is advanced structural work with material complexity, transfer-pricing exposure, and diligence friction. It is not a Series-A default; it reopens at Series-C or growth stage. Entity structuring belongs to [mod-101](../mod-101-legal-entity-formation-and-corporate-structure/); tax analysis is out of scope for this chapter and requires qualified tax counsel.
- IP-diligence readiness is a continuous discipline. Buy-side counsel in a financing or M&A transaction will request patent, trademark, and copyright schedules; chain-of-title evidence for material assets; complete PIIA / SOW coverage of every past and current employee and contractor; the OSS SBOM ([chapter 05](./05-open-source-hygiene-and-sbom-programme.md)); trade-secret programme documentation; third-party inbound and outbound licences; and the trail supporting the customer-facing IP indemnity. The goal is not zero findings but no surprises.
- This chapter defers to [mod-102](../mod-102-founding-team-legal-architecture/) for founder-era pre-formation IP and PIIA, to [mod-103](../mod-103-employment-law-and-contract-design/) for employee PIIA and DTSA notices, to [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md) for contractor IP-assignment mechanics, to [chapter 05](./05-open-source-hygiene-and-sbom-programme.md) for OSS licence hygiene, and to [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) for the privacy / data-governance layer that intersects with trade-secret protection for personal data.
