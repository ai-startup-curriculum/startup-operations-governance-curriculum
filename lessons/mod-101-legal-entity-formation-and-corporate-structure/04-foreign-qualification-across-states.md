# 4. Foreign qualification across states

> A Delaware corporation is only "at home" in Delaware. Every other state where it does business requires a Certificate of Authority — or imposes a penalty.

## Motivation

"Foreign qualification" is a term of art: from Delaware's perspective, the corporation is domestic; from every other state's perspective, it is foreign, and most states require a foreign corporation transacting business inside their borders to register with the state before doing so. The consequences of skipping the registration range from modest per-day penalties to loss of the ability to sue in the state's courts — a material problem the first time the corporation needs to enforce a contract or defend a claim. This chapter defines the trigger, walks the process, and quantifies the penalty exposure with reference to two states whose penalty statutes are frequently cited in diligence: California and New York.

## The "transacting business" trigger

Every state has its own statutory definition of what makes a foreign corporation "transacting business" (or "doing business," "carrying on business," or the state-specific term of art) inside the state and therefore subject to registration. The federal Constitution's Commerce Clause and the states' long-arm statutes converge on a rough operational definition — but the details vary by state, and startups routinely misjudge the boundary.

**A safe operational rule:** a corporation is transacting business in a state if it has one or more of the following:

- **Employees who work in the state** — remote-first startups create these constantly, and payroll registration in that state usually triggers the qualification requirement too.
- **A physical office, warehouse, retail location, or leased space** in the state.
- **Owned or leased property or equipment** located in the state on an ongoing basis.
- **A registered agent or "doing business" registration** already on file for tax or payroll purposes — many states cross-reference these.
- **Systematic and continuous solicitation and closing of business** inside the state, especially in-person sales, on-site services, or persistent trade-show presence.
- **Bank accounts, licences, or contracts** whose performance occurs materially within the state.

**A safe operational rule for the *other* direction (what generally does not require qualification):**

- Purely interstate commerce (shipping product from Delaware into a state, without a physical or personnel presence there).
- Holding meetings of directors, officers, or stockholders.
- Maintaining bank accounts.
- Isolated transactions completed within 30 days that are not part of a course of similar transactions.
- Owning securities of another corporation.

These "safe harbours" are statutorily enumerated in each state's foreign-qualification statute (for example, Cal. Corp. Code § 191(c) lists activities that do not constitute "doing intrastate business" for California; the Model Business Corporation Act contains an equivalent list in § 15.01(b) that many states have enacted). Read the specific state's list before relying on the safe harbour.

## The process

The mechanics of foreign qualification are consistent across states, with per-state variance in fees, forms, and processing times.

1. **Confirm name availability.** The corporation's Delaware name must be available in the target state — some states require the corporation to use an "assumed name" or add a corporate indicator if the exact name is taken.
2. **Order a Certificate of Good Standing from Delaware** dated within a short window (typically 30–90 days) of the state's application.
3. **Complete the state's application for Certificate of Authority** (California: Statement and Designation by Foreign Corporation, Form S&DC-S/N; New York: Application for Authority; Texas: Form 301; and so on). Each application requires the corporation's Delaware charter details, its principal-office address, its in-state registered agent, the names and addresses of directors and officers, and the type of business conducted.
4. **Designate an in-state registered agent** and file the appointment. Commercial registered agents (CSC, CT, Cogency, InCorp) handle this automatically as part of a national-agent engagement.
5. **Pay the state's initial filing fee** and any accompanying franchise-tax or entity-fee deposit.
6. **File the state's initial annual report / statement of information** within the state's grace period (California: within 90 days of qualification, then annually by the anniversary month).
7. **Register with the state's tax and employment authorities** — the department of revenue for income / sales / gross-receipts tax; the department of labor / employment for unemployment insurance and, where applicable, disability insurance and paid family leave withholdings.
8. **Add the state to the compliance calendar** (see [chapter 03](./03-corporate-record-and-compliance-calendar.md)) with the correct annual-report cadence, franchise-tax cadence, and registered-agent renewal.

## Penalty exposure — California and New York

Two states are worth internalising because they are the two most likely to matter for an early-stage US startup and because their statutes are commonly referenced in diligence.

### California — Cal. Corp. Code § 2203

A foreign corporation that transacts intrastate business in California without qualifying is exposed to:

- **A per-day monetary penalty** under Cal. Corp. Code § 2203(c). <!-- needs-research: verify the current $20 / day figure and the maximum aggregate at the California Corporations Code § 2203 statutory text; historically $250 per offense plus $20 per day. -->
- **Inability to maintain any action or proceeding** in California courts on any intrastate business until the corporation has qualified and paid all required fees, taxes, and penalties (Cal. Corp. Code § 2203(c)).
- **Voidability of contracts** in some fact patterns.
- **Franchise Tax Board exposure**: retroactive California franchise-tax liability, plus penalties and interest, for the full period of unqualified intrastate business. California's minimum franchise tax is $800 / year for corporations (FTB Form 100) — payable back to the year the corporation began transacting business, not the year it eventually registered.

### New York — N.Y. Bus. Corp. Law § 1312

A foreign corporation doing business in New York without a Certificate of Authority may not maintain any action or special proceeding in a New York court until it has obtained authority (N.Y. B.C.L. § 1312(a)). The corporation may still be sued, and any liability it incurs continues; only its ability to enforce its own claims is suspended. New York courts routinely dismiss or stay actions brought by non-qualified foreign corporations pending qualification. Franchise-tax and filing penalties accrue in parallel.

### Other states worth naming (representative)

- **Texas** — Tex. Bus. Orgs. Code § 9.051 and § 9.052 penalise transacting business without registration with late fees equal to the fees that would have been paid over the period of unregistered operation.
- **Massachusetts** — M.G.L. c. 156D § 15.02 imposes a per-year penalty and denies court access.
- **Illinois** — 805 ILCS 5/13.70 imposes penalties and denies court access.
- **Florida** — Fla. Stat. § 607.1502 imposes back-fees, a monetary civil penalty per year of unregistered operation, and denies court access.
- **Washington** — RCW 23.95.505 imposes similar penalties.

Read the specific statute the first time the corporation operates in a state; do not assume every state's penalty structure matches Delaware's or California's.

## The "employees make the state a foreign-qualification state" pattern

The single most common trigger for a startup's first foreign-qualification obligation is hiring the first employee in a new state. Payroll registration in the state's employment-tax system (California EDD, New York DOL, Texas Workforce Commission, etc.) usually requires the corporation to demonstrate it is a legally authorised entity in the state. Modern PEOs and HRIS platforms (Justworks, Rippling, Gusto, TriNet) either handle the qualification as part of onboarding a new state, or explicitly require the corporation to have qualified before payroll can be run. Missing the qualification often surfaces as a payroll-onboarding blocker rather than a diligence finding — but if payroll is being run for months without qualification, the diligence finding follows.

## The remote-first startup exposure

A startup with 12 fully-remote employees spread across 12 states plausibly needs to foreign-qualify in all 12 of those states, plus register in each state's payroll-tax system, plus (in many of them) register for sales tax if it sells taxable product, plus (in some of them) register for unemployment insurance, workers' compensation, paid family leave, and disability insurance. This is not a hypothetical — it is a modern operating reality. The cost per state ranges roughly from a few hundred dollars in filing fees plus a commercial registered agent to several thousand dollars in first-year franchise tax where a state's minimum tax is meaningful. The math typically favours qualifying in each state where the corporation has any employee, contractor being paid on a persistent basis, or physical asset, rather than betting on a "we're too small to notice" position that Series-A diligence will eventually surface.

## Concrete example: the "we just hired in New York" checklist

A Delaware corporation headquartered in San Francisco hires its first New York employee, working remotely from Brooklyn. Within 30 days of the hire date:

1. Order a Delaware Certificate of Good Standing.
2. File the New York **Application for Authority** with the NY Department of State, Division of Corporations. Pay the filing fee.
3. Designate the Secretary of State as the corporation's initial New York agent for service of process (standard New York mechanism) and engage a commercial registered agent to receive forwarded service.
4. Publish the "notice of qualification" as required by N.Y. B.C.L. § 1304(a)(9) in two newspapers in the county of the corporation's designated New York office for six weeks (New York's unique post-formation publication requirement). <!-- needs-research: confirm the current publication requirement and cost band, which has historically been material for NYC counties. -->
5. Register with the New York Department of Taxation and Finance for corporate income tax and, if applicable, sales tax.
6. Register with the New York Department of Labor for unemployment insurance.
7. Register with the New York Workers' Compensation Board.
8. Register with the New York State Insurance Fund or private carrier for statutory disability benefits and paid family leave.
9. Add New York to the corporation's compliance calendar: NY Biennial Statement due every two years, franchise tax annually, registered-agent renewal annually.
10. Confirm the corporation's D&O and Employment Practices Liability policies extend to New York exposures.

## Summary

- Foreign qualification is triggered by "transacting business" in a state — usually by employees, physical presence, or ongoing in-state operations. Purely interstate commerce and a short list of statutory safe-harbour activities do not trigger qualification.
- The process is consistent across states: Certificate of Good Standing from Delaware → application for Certificate of Authority → registered agent → tax and employment registrations → calendar entry.
- Penalty exposure is real: California can deny court access and impose per-day fines under Cal. Corp. Code § 2203; New York can deny court access under N.Y. B.C.L. § 1312; most other states have parallel penalty regimes.
- The single most common first trigger is the first employee in a new state. PEOs and HRIS platforms often surface the issue at payroll onboarding.
- Remote-first startups quickly accumulate multi-state qualification obligations. Model the cost, and qualify deliberately rather than reactively.
