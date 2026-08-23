# 5. Subsidiary structure design

> Add a subsidiary only when the structure earns its complexity. Every additional entity is another compliance calendar, another minute book, another tax return.

## Motivation

Startups accumulate subsidiaries the way ships accumulate barnacles — a Delaware LLC set up for a joint venture that never launched, an offshore SPV to hold a piece of IP for a rejected licensing structure, a UK subsidiary that outlived the employee who was based there. Each of those subsidiaries is a real entity with real filings, real tax exposure, and a real diligence line-item. The rule for adding a subsidiary is: *do it only when the structure earns the complexity*, and design the structure with a clear exit path if the business rationale disappears.

This chapter walks the three common domestic subsidiary patterns and the boundary to international structures (which mod-113 owns in depth).

## The default structure

The default corporate structure of a US venture-backed startup is a single Delaware C-corporation, with all operations, all employees, all IP, and all contracts owned by that one entity. There are no subsidiaries. The single-entity structure minimises compliance, maximises optionality, and matches what Series-A diligence expects to find.

Adding a subsidiary trades away that simplicity for one of a small number of specific benefits. Below are the patterns worth learning.

## Pattern 1 — Delaware operating subsidiary of an IP-holding parent

Sometimes described as the "IP holdco / opco" structure. A Delaware parent corporation owns the IP; a wholly-owned Delaware operating subsidiary licenses the IP from the parent and conducts operations, holds employees, and signs commercial contracts. Rationales:

- **Ring-fencing operating liability from the IP.** A tort or contract claim against the operating entity does not automatically reach the IP asset.
- **Tax-planning opportunities in specific structures** — historically, licensing fees paid from the operating subsidiary to the IP-holding parent were used for state-tax planning (e.g., holding IP in a low-tax state). Many of those structures have been curtailed by state addback statutes; the CFO / tax advisor should validate whether the play still works in the states of operation before the structure is stood up.
- **Later transaction flexibility** — separating IP from operations can simplify a licensing transaction, a spinoff, or an asset sale that isolates a specific product line.

**Cost:** two sets of charters, bylaws, board consents, minute books, franchise taxes, and annual reports; an intercompany licensing agreement that must be genuine (arm's-length terms, actual license payments); potential intercompany transfer-pricing exposure; and a diligence explanation that the acquirer's counsel will read closely.

This structure is **rarely appropriate at seed or Series-A** for a normal SaaS or AI startup. It appears more often in later-stage companies with distinct product lines, in life-sciences companies isolating a specific asset for licensing, and in specific state-tax-planning contexts.

## Pattern 2 — Product-line ring-fencing

A parent operating company creates a wholly-owned Delaware subsidiary to hold a distinct product line — often when the product line is:

- **Materially more regulated** than the parent's core business (a payments product, a healthcare product with HIPAA exposure, a broker-dealer or money-transmitter licence holder).
- **Being prepared for a potential spinoff or sale** as a discrete unit.
- **A joint venture** with another company (see Pattern 3).
- **Carrying materially different liability profile** (e.g., a hardware line with product-liability exposure that the parent's software business does not have).

The ring-fenced subsidiary has its own board, its own officers (frequently overlapping with the parent), its own regulatory registrations, and its own commercial contracts. The parent typically retains all IP that is used across the family and licenses it to the subsidiary; the subsidiary owns IP specific to its product line.

**When it is not right:** if the product line is just a new SKU inside the same customer base, on the same infrastructure, sold by the same sales team, ring-fencing it into a subsidiary is compliance overhead without a real benefit. The default is to run new products inside the parent unless a specific reason forces separation.

## Pattern 3 — Joint venture structure

Two or more corporations form a jointly-owned entity (Delaware corporation, Delaware LLC, or occasionally a partnership) to pursue a specific business initiative together. Each parent owns a percentage of the JV; the JV has its own board (usually with directors appointed by each parent per a Stockholders' Agreement or LLC Agreement); the JV signs its own commercial contracts.

Governance considerations for a JV subsidiary:

- **The JV agreement is the governing document**, layered on top of the JV entity's charter / LLC agreement. Deadlock provisions, capital-call mechanics, buyout / put / call rights, IP ownership at wind-up, non-compete boundaries, and exit-triggering events are all authored in the JV agreement.
- **Board composition** reflects economic ownership, with veto rights on major decisions typically granted to each parent regardless of ownership percentage.
- **Employees, IP, and contracts** are typically contributed by each parent under contribution agreements, with clear ownership at wind-up.
- **Tax structure** is chosen deliberately — an LLC-JV taxed as a partnership pushes income to the parent members; a corporate JV pays entity-level tax and shields the parents from operational income.

JV structures are legal-heavy. Every material JV should have counsel drafting the JV agreement and setting up the entity, not a founder self-serving from a Delaware-incorporation kit.

## When to add an international subsidiary (handoff to mod-113)

An international subsidiary is warranted when the startup needs a legal presence in another country for one of the following:

- **Hiring employees in a country where the parent cannot legally employ them directly** (most countries — a US corporation cannot payroll a French employee out of Delaware without either a French entity or an Employer of Record).
- **Signing revenue-generating contracts in-country** where local customers require a local counterparty.
- **Registering IP** with a national IP office.
- **Establishing a regulated presence** (a banking licence, an insurance licence, a data-processing entity for GDPR purposes).

**When *not* to form an international subsidiary:** hiring a single individual contributor in a new country. That is what an Employer of Record (Deel, Remote, Oyster, Velocity Global, Papaya Global) is for. The EOR employs the individual under a local contract, invoices the parent, and eliminates the need for a subsidiary until the country's operations reach a scale that justifies one (typically 3–5 employees, meaningful in-country revenue, or a regulatory trigger).

**The full mechanics of international subsidiary formation** — statutory-form choice per country (Ltd, GmbH, SAS, Pty Ltd, KK, and equivalents), local director / statutory-agent requirements, local tax and social-insurance registrations, transfer-pricing documentation, permanent-establishment analysis, VAT / GST registrations, and the parent's disclosure and withholding obligations — are the subject of [mod-113 — International Expansion & Global Workforce](../mod-113-international-expansion-and-global-workforce/). This module flags the decision boundary; mod-113 owns the execution.

## Tax and governance consequences of adding any subsidiary

Every subsidiary — domestic or international — carries a standard consequence stack:

- **Compliance cost.** Formation fees, franchise / income tax filings in the jurisdiction, annual reports, registered-agent fees, minute-book maintenance, and separate audit or tax-return preparation.
- **Board and officer governance.** Each subsidiary needs at least one director and typically several officers. In an all-wholly-owned domestic structure, these can overlap with the parent's board and officers, but board consents authorising subsidiary actions must still be signed.
- **Intercompany agreements.** IP licenses, service agreements, cost-sharing agreements, and cash-management arrangements between parent and subsidiary must be documented at arm's length. Undocumented intercompany transfers create tax and audit exposure.
- **Consolidated financial statements.** A parent with subsidiaries prepares consolidated financials under US GAAP (or IFRS for international); this is a bookkeeping and audit-preparation lift that the CFO / controller function absorbs.
- **State and federal tax elections.** Consolidated federal returns require IRS Form 851; state consolidated / combined returns vary by state and can affect apportionment. Each new subsidiary is a new tax-planning conversation.
- **D&O insurance scope.** Confirm the D&O policy names the subsidiary as an insured; otherwise, subsidiary directors are exposed without cover.
- **Diligence footprint.** Every subsidiary produces its own diligence request list in the next financing or M&A transaction: charter, bylaws, minute book, cap table, contracts, franchise-tax filings, foreign-qualification history, insurance, tax returns.

## Concrete example: the "should we add a Delaware LLC for our new product?" decision

A Series-A startup with a SaaS product hires a small team to build a payments product. The team asks whether the payments product should be inside a new Delaware LLC or Delaware C-corporation subsidiary.

The relevant questions:

1. **Is the payments product going to hold a money-transmitter or payment-facilitator licence?** If yes → yes, a subsidiary. Regulatory registrations are far easier to obtain, maintain, and eventually transfer when they belong to a distinct legal entity.
2. **Is the product going to be spun off or sold within 24 months?** If yes → yes, a subsidiary. Separating it now reduces the transaction complexity later.
3. **Is the product materially higher-liability than the SaaS product (e.g., holding customer funds)?** If yes → probably yes, a subsidiary. Ring-fencing the SaaS balance sheet from a payments-product incident has real value.
4. **Otherwise** → default to running the new product inside the parent. Adding a subsidiary for internal-organisational reasons ("the payments team wants its own P&L") is not a legal reason; a business unit inside the parent has its own P&L just as well.

Whatever the answer, document it in a short memo signed by the CFO / GC / CEO before spending on formation.

## Summary

- The default is a single Delaware C-corporation. Every subsidiary you add is a compliance, tax, and diligence commitment.
- Domestic subsidiary patterns: IP-holdco / opco (rare at early stage), product-line ring-fencing (regulatory or liability-driven), joint ventures (a distinct governance discipline of their own).
- International subsidiaries: warranted for in-country hiring, in-country revenue counterparties, regulatory presence, and IP registration. For a single new-country hire, use an Employer of Record. Full mechanics live in mod-113.
- Every subsidiary carries a standard consequence stack: filings, boards, intercompany agreements, consolidated financials, tax elections, insurance, diligence footprint. Model the cost before adding the entity.
- Document the "why" of every subsidiary at the time of formation. It saves a future GC from writing the memo when a diligence request lands.
