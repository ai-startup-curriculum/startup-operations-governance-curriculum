# 2. Stand up the entity

> The formation-day package — Certificate of Incorporation, Bylaws, Initial Board Consent, Founders' Stock Purchase Agreements, 83(b), and the first stockholder consent.

## Motivation

"Stand up the entity" sounds like clerical work. It is not. Every choice made in the formation package — how many shares to authorize, what par value to set, which directors to name, what vesting to give the founders — either matches what the next investor and the IRS expect, or creates a defect that costs money to fix. This chapter walks the formation package end to end.

## The formation package (in filing order)

1. **Certificate of Incorporation (charter)** — filed with the Delaware Secretary of State under DGCL § 102. This is what creates the corporation.
2. **Action of Incorporator** — the incorporator (usually outside counsel) signs a one-page consent that (a) adopts the initial bylaws and (b) appoints the initial board of directors, then resigns.
3. **Bylaws** — adopted by the incorporator's action, then acknowledged by the initial board.
4. **Initial Board Consent** — the newly-appointed board's first written consent under DGCL § 141(f), covering officer appointments, adoption of the stock plan, and the initial stock issuances.
5. **Founders' Stock Purchase Agreements** — each founder buys their restricted stock, pays consideration (cash or IP contribution), and signs a vesting schedule.
6. **83(b) elections** — each founder mails an IRC § 83(b) election to the IRS within **30 days** of the stock purchase.
7. **Initial Stockholder Consent** — the founders, now stockholders, act by written consent under DGCL § 228 to ratify board actions where required (e.g., increases to authorized shares, stock-plan approval for later § 422 ISO purposes).
8. **EIN and state registrations** — the corporation obtains a federal EIN via IRS Form SS-4 and registers with the state tax authority.

## The Certificate of Incorporation

The charter is short — usually 2–4 pages at formation. The default clauses:

- **Name.** Must include a corporate indicator ("Inc.", "Corp.", "Corporation", etc.) and must be distinguishable on the Delaware Secretary of State records. Reserve the name via 8 Del. C. § 102(a)(1) filings if you need to lock it before formation.
- **Registered office and registered agent.** Required by 8 Del. C. § 132. This is a Delaware street address; the registered agent is a commercial provider (CSC, CT Corporation, Cogency Global, InCorp) or a Delaware resident.
- **Purpose.** "To engage in any lawful act or activity for which corporations may be organized under the Delaware General Corporation Law." This general-purpose clause is standard and preserves flexibility.
- **Authorized shares.** The total number of shares the corporation is authorized to issue. Common founder-formation practice is to authorize a large enough block to accommodate founder issuances plus an initial option pool plus headroom, without triggering a franchise-tax cliff (see the "authorized shares vs. franchise tax" trap below).
- **Par value.** A nominal per-share value assigned to each authorized share (commonly $0.00001 to $0.0001). Par value is not a market-value concept; it is a legal-capital concept that affects (a) the minimum consideration the corporation may accept for shares (DGCL § 153) and (b) the Delaware franchise-tax calculation under the Assumed Par Value Capital Method.
- **Board authority to issue preferred ("blank-check preferred").** A clause authorizing the board to designate one or more series of preferred stock, fix their rights and preferences, and issue them by board resolution (DGCL § 151). This is standard at formation so that a future priced-round Series Seed / A can be issued without a full charter restatement — the board can file a Certificate of Designations for the new series.
- **Director exculpation.** A clause under DGCL § 102(b)(7) limiting directors' personal liability for breach of fiduciary duty, subject to the statutory carve-outs (bad-faith, loyalty breaches, § 174 improper distributions, transactions where the director derived an improper personal benefit). Delaware amended § 102(b)(7) in 2022 to allow officer exculpation (with narrower scope than director exculpation); the modern form of the charter can include both.
- **Indemnification enabling clause.** A clause referencing DGCL § 145 and confirming the corporation will indemnify directors and officers to the fullest extent permitted by law. The mechanical detail lives in bylaws or a separate indemnification agreement; the charter clause is the enabling backstop.
- **Forum selection.** Optional but standard: an exclusive-forum clause designating the Delaware Court of Chancery as the sole forum for internal corporate-affairs disputes, plus a federal-forum clause for Securities Act claims (upheld by the Delaware Supreme Court in *Salzberg v. Sciabacucchi*, 227 A.3d 102 (Del. 2020)).

### The "authorized shares vs. franchise tax" trap

Delaware franchise tax has two calculation methods (see [chapter 03](./03-corporate-record-and-compliance-calendar.md)). Under the **Authorized Shares Method**, a corporation with millions of authorized shares can face an enormous initial franchise-tax bill. The **Assumed Par Value Capital Method** produces a much lower number for a startup with low par value and low gross assets — but the state's default invoice uses the Authorized Shares Method, and every startup should recompute using the Assumed Par Value method and pay the lower of the two. Authorizing 10,000,000 shares of common stock at $0.0001 par is a common formation default that keeps the Assumed Par Value calculation low while giving room for founder issuances and an initial option pool. Authorizing 100,000,000 shares of common at $0.00001 par is also common. Do the math before you file.

## The Bylaws

Bylaws are the operating manual for the board and the stockholders. They are adopted by the incorporator (and later, in practice, by the board) under DGCL § 109, and can be amended by the board unless the charter reserves that power to stockholders. Modern startup bylaws address:

- **Stockholder meetings.** Time and place of the annual meeting (required by DGCL § 211(b) — must be held annually), notice periods, quorum requirements (usually a majority of outstanding shares entitled to vote), and voting by proxy.
- **Action by written consent of stockholders.** Whether stockholders can act by less-than-unanimous written consent under DGCL § 228. Private-company bylaws almost always permit majority written consent; public-company bylaws typically prohibit it.
- **Number and election of directors.** A range (e.g., "one to nine") or a fixed number, and how vacancies are filled (usually by the remaining directors, per DGCL § 223). At formation the board is typically one or two directors — a single founder-director, or two co-founders.
- **Board meetings.** Notice, telephonic-meeting permission, quorum (usually a majority of directors), and action by unanimous written consent under DGCL § 141(f).
- **Officers.** The officer roles the corporation will maintain. Most startups elect at minimum a President and a Secretary at formation; a CEO, CFO, and General Counsel typically follow. DGCL § 142 permits any officer titles the bylaws provide.
- **Indemnification.** Mandatory indemnification of directors and officers to the fullest extent permitted by DGCL § 145, plus advancement of expenses. The bylaws are the workhorse for indemnification; a separate indemnification agreement layered on top (see [chapter 03](./03-corporate-record-and-compliance-calendar.md)) tightens the contract further.
- **Uncertificated shares.** Most modern startups elect uncertificated shares under DGCL § 158 so that stock issuance and transfer happen electronically (Carta, Pulley, Shareworks) rather than via paper certificates. The bylaws should authorize uncertificated shares explicitly.

## The Initial Board Consent

Once the incorporator has appointed the initial directors, those directors sign a written consent under DGCL § 141(f). At a minimum, the initial board consent:

1. **Ratifies the incorporator's actions** and adopts the charter as filed.
2. **Adopts the bylaws.**
3. **Appoints officers** (typically CEO, President, Secretary, Treasurer at formation; more roles added later).
4. **Designates the fiscal year** (most startups pick December 31 to align with individual founder tax returns; some pick a non-calendar year for a specific reason).
5. **Authorizes opening a bank account** and designates authorized signatories.
6. **Adopts the stock plan** (the equity incentive plan) and reserves shares for issuance under it. This is the moment the § 422 ISO clock starts; adopt the plan early.
7. **Approves the initial stock issuances** — the founders' shares — including the consideration, the vesting schedule, and the form of Stock Purchase Agreement.
8. **Approves the form of Indemnification Agreement** for directors and officers.
9. **Authorizes elections and filings** — the EIN application, state registrations, and initial insurance placement.
10. **Approves engagement of counsel and, if applicable, the initial accounting firm.**

Every action item on the consent should reference the specific document (charter, bylaws, stock plan, form of SPA, form of indemnification agreement) as an exhibit or by version-number reference. The consent is signed by every director; DGCL § 141(f) requires unanimity for board written consents, absent a bylaw provision permitting non-unanimous consents (which is not the modern default).

## Founders' Stock Purchase Agreements

Founders do not receive their stock — they **buy** it. The Stock Purchase Agreement documents:

- **Purchase price** — the price per share the founder pays, typically the par value or a nominal amount, paid in cash and/or in exchange for the founder's contribution of pre-existing IP.
- **Vesting schedule** — the market default is 4 years with a 1-year cliff. Some founders vest on a different schedule; whatever it is, it must be captured in writing on formation day, not later.
- **Right of repurchase** — the corporation's right to repurchase unvested shares at the original purchase price upon the founder's separation. Without this repurchase right, "vesting" is a fiction; the shares are already the founder's, and the corporation has no lever if the founder walks.
- **Acceleration** — typically none, or double-trigger acceleration on change-of-control, or a founder-specific negotiated single-trigger. The founder-CoC-accel conversation is deferred to [mod-102](../mod-102-founding-team-legal-architecture/).
- **Restrictions on transfer** — right of first refusal, co-sale, and market-standard transfer restrictions.
- **Consideration for pre-existing IP** — if the founder contributes IP (code, documents, designs) as part of the purchase price, the SPA (or a parallel IP-assignment) captures the assignment. The full mutual IP assignment (PIIA / CIIAA) is authored in [mod-102](../mod-102-founding-team-legal-architecture/); this chapter only flags that the entity must own the founder's pre-formation contributed IP.

**The mechanics of "purchase":** the founder writes a check (or transfers wired funds) to the corporation for the purchase price. This is not optional. Stock issued without consideration is a defective issuance and creates a Series-A diligence problem. Even a $10 check for 8,000,000 shares of common at $0.00000125 per share is a real transaction with a real transfer of consideration; the founder should keep a copy of the check or wire confirmation for the corporate record.

## The 83(b) election

The IRC § 83(b) election is the single most consequential piece of paper a founder signs. It is worth its own subsection.

**What it does.** Section 83(a) says that when property is transferred to you in connection with services, you have ordinary income equal to the fair-market-value minus the amount you paid — *at the time the property vests*. For restricted founders' stock that vests over four years, § 83(a) would produce ordinary income at each vesting event, calculated against the (usually much higher) fair-market value at that vesting date. Section 83(b) lets you elect, within 30 days of the *transfer* (not the vesting), to recognise the income up-front — usually zero income, because the founder paid par-value-equivalent for stock worth roughly par-value-equivalent on day one. After a valid § 83(b) election, all future appreciation is capital gain, taxed only on sale.

**The 30-day rule is absolute.** Treasury Regulation § 1.83-2(b) requires the election to be filed with the IRS Service Center where the taxpayer files their return within 30 days after the date of the property transfer. Late elections are void. There is no cure. This is the single most common Series-A diligence failure that founders inherit from themselves. The founder must (a) sign the election, (b) mail it certified-mail-return-receipt to the correct IRS Service Center, (c) keep the certified-mail receipt, (d) provide a copy to the corporation for the corporate record, and (e) attach a copy to the founder's federal tax return for that year.

**The form.** The IRS publishes model § 83(b) language in Rev. Proc. 2012-29. Every startup-formation counsel and every incorporation-service package includes an 83(b) form; none of them cure the 30-day deadline. Use the form counsel provides, or use Rev. Proc. 2012-29's model text.

**When 83(b) is not right.** If the founder pays a price equal to fair market value for the stock at issuance (which is almost always the case at formation), the § 83(b) election has essentially zero income to recognise — free option. If the stock has already appreciated between the corporation's formation and the founder's issuance (unusual, but possible if the founder joins after formation), the § 83(b) election locks in ordinary income today; the founder should still file, but understand the tax cost.

## The Initial Stockholder Consent

Immediately after the founders receive their stock, they act as the corporation's initial stockholders. A one-page consent under DGCL § 228 typically:

1. **Ratifies the board's actions** to date.
2. **Approves the stock plan** for IRC § 422 ISO purposes — § 422(b)(1) requires stockholder approval of the plan within 12 months before or after board adoption for any ISO grants to qualify.
3. **Elects any additional directors** if the initial board expands beyond the founders.
4. **Approves any charter amendments** that require stockholder approval (e.g., increasing authorized shares beyond what the initial charter provides).

Stockholder consents in a private company can be signed by holders of a majority of the outstanding voting shares unless the charter or bylaws require more (DGCL § 228). At formation, when the only stockholders are the founders, this is usually unanimous.

## Concrete formation-day timeline (a two-founder, no-outside-capital-yet startup)

- **Day 0.** Incorporator files the Certificate of Incorporation with the Delaware Secretary of State. Certificate is date-stamped and returned.
- **Day 0.** Incorporator signs Action of Incorporator: adopts bylaws, appoints two founders as initial directors, resigns.
- **Day 0.** Initial Board Consent signed by both founder-directors: appoints officers (CEO, President, Secretary, Treasurer as agreed), adopts stock plan, approves form SPA and IP assignment, approves initial issuances (e.g., 4,000,000 shares to each founder at $0.0001 per share).
- **Day 0.** Each founder signs a Stock Purchase Agreement and IP Assignment, writes a check to the corporation, and receives their shares (uncertificated, recorded in the share ledger).
- **Day 0.** Initial Stockholder Consent signed: approves stock plan for § 422 purposes; ratifies board actions.
- **Days 0–30.** Each founder mails their § 83(b) election, certified mail, to the IRS Service Center. Copy to corporation. Copy attached to that founder's Form 1040 for the year.
- **Days 0–14.** Corporation obtains EIN via IRS Form SS-4. Opens bank account. Registers with Delaware Division of Revenue if applicable, and with any home-state tax authority.

Every one of those actions creates a document. Every one of those documents goes into the minute book (see [chapter 03](./03-corporate-record-and-compliance-calendar.md)).

## Summary

- Formation is a package of interlocking documents that must all match: charter, bylaws, board consent, officer appointments, stock plan, founders' SPAs, 83(b)s, stockholder consent.
- The Certificate of Incorporation encodes the choices that are expensive to change later: authorized shares, par value, blank-check preferred, director exculpation, forum selection.
- The Initial Board Consent is the single document that "turns on" the corporation's operating machinery — officers, bank account, stock plan, and founders' issuances all trace back to it.
- Founders **buy** their stock, they do not receive it. The Stock Purchase Agreement, the vesting schedule, and the corporation's repurchase right make "vesting" real.
- **The § 83(b) 30-day deadline is absolute.** Set the calendar reminder before the founder signs anything else on formation day.
- Every document on formation day goes into the corporate record — indexed, dated, signed. Chapter 3 is the operating manual for that record.
