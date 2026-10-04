# Discovery Interview Notes

> **Revision note:** An earlier version of this file contained a draft set of plausible client answers, written before any actual discovery conversation took place, intended as a starting point for validation. That draft has been **discarded and replaced** below with the record of an actual simulated joint discovery session, which surfaced real (simulated) evidence — some of it contradicting the earlier guesses (e.g., the specific PMS vendors per property were invented in the draft; the real session confirms this is genuinely still unconfirmed). Keeping a disproven guess in the record alongside real evidence would undermine the traceability principle this project is built on, so it's been removed rather than marked up. See [`../CHANGELOG.md`](../CHANGELOG.md) for when this happened and why.

## Meeting 2 — Joint Discovery Session

**Attendees:** Khalid Rahman (Group Procurement Manager), Nadia Hassan (Group Finance Director), Omar Farouk (Group IT Manager), Mariam Al Mazrouei (Property GM), Daniel Thomas (Property GM)
**Format:** 45-minute joint session, followed by separate targeted Finance and IT sessions (not yet held)

### Confirmed client statements

- The initiative stems from group expansion and executive concern about obtaining a consolidated, comparable view of performance across the five properties — consistent with the original Procurement brief.
- **Properties operate with intentional, legitimate operational autonomy.** Khalid explicitly corrected the framing here: autonomy itself is not the problem. The issue is specifically where that flexibility affects information that needs to be compared or governed at group level.
- A concrete example was given: during the March reporting cycle, one property's occupancy figure appeared inconsistent with its own room-night figures. Investigation found the property excluded temporarily-unavailable rooms from its occupancy denominator, while corporate's comparison used total room inventory — **a definitional difference, not a data error.**
- Finance distinguishes three categories of issue, not currently tracked separately: **data correction** (the number was actually wrong), **definition clarification** (the number was reasonable, the basis wasn't clear), and **reconciliation** (two valid numbers needing context before comparison).
- **No formal group-wide KPI data dictionary or glossary exists today** — confirmed independently by both Finance (Nadia) and IT (Omar).
- The primary business impact identified so far is recurring Finance workload and delay in producing the monthly consolidated management pack — not, as far as currently known, a cancelled strategic decision or a materially wrong number reaching management undetected. Nadia was explicit that this distinction matters and declined to overstate the impact.
- Finance (Nadia) proposed itself as the appropriate owner of business/KPI definitions, with input from Operations and property teams, and IT as a consulted (not owning) stakeholder for reflecting definitions in systems. Tentatively agreed in the room; **not yet formally approved** by Executive Management.
- Both GMs support clearer group-level definitions in principle, **provided there is a proper process for agreeing them** and legitimate property-level differences are preserved rather than overridden for corporate convenience.

### Assumptions / still unverified

- **Current technology landscape per property** — which PMS/operations system each property runs, whether shared or different vendors, what reporting tools exist, whether integrations already exist. This remains the single highest-impact unknown (consistent with Q2.1 in the original [discovery questionnaire](discovery-questionnaire.md)). To be covered in the dedicated IT session.
- The exact data flow from property system → property report → corporate Finance → reconciliation → management report, and precisely where manual intervention occurs.
- Frequency/volume of clarification cases per month and the staff time this consumes. Nadia explicitly declined to give a figure "that would be treated as a requirement or business case figure" until it's actually measured — flagged as an evidence-gathering task for the Finance session, not assumed.
- How many KPIs beyond occupancy are affected by definitional inconsistency (revenue, ADR, and RevPAR were mentioned as plausible by Nadia, not confirmed).
- **Whether this pattern extends beyond Finance** into procurement or guest-service metrics. Both GMs raised this as a possibility but explicitly cautioned against assuming it's the same problem without investigation — this is a hypothesis, not a finding, and should not be treated as confirmed scope.

### Open questions / stakeholder dependencies

- Formal governance sign-off: who approves Finance as owner of KPI definitions — not yet escalated beyond this working group's informal agreement.
- Dedicated Finance session (not yet scheduled): Nadia to bring historical clarification case examples. She flagged these aren't cleanly categorized retroactively, so expect some cases to span more than one category.
- Dedicated IT session (not yet scheduled): Omar to walk through the current system landscape and data flow. He flagged that some of the reporting flow sits with Finance and property teams rather than IT, so IT alone may not have complete answers to every question.
- GMs asked to bring **concrete examples, not general impressions**, if anything comes to mind on procurement or guest-service inconsistency — not committed to proactively investigate.

### Decisions, risks, and next actions

**Decisions**
- Working problem statement adopted (below), with Khalid's correction applied.
- Proceed via separate targeted Finance and IT sessions rather than continuing to probe broader scope in the joint session — avoided speculation and respected participants' time.
- Finance tentatively proposed as owner of KPI/business definitions, IT as a consulted stakeholder — pending formal confirmation.

**Risks noted in-session**
- Risk of writing RFP requirements that ask a vendor to solve what is actually an internal governance problem (agreeing KPI definitions) through software alone.
- Risk of treating the single March occupancy example as representative of a systemic issue without further evidence across properties and KPIs.
- Risk of over-standardizing and removing legitimate property-level operational flexibility if group definitions are imposed without a proper agreement process — raised by both GMs.

**Next actions**
1. Share this written record with the group before scheduling the Finance and IT sessions.
2. Schedule a dedicated Finance session (historical cases, frequency, categorization).
3. Schedule a dedicated IT session (system landscape, data flow mapping).
4. Leave the broader-scope question (procurement/guest-service) open pending any concrete examples GMs bring forward — do not add to scope on a hypothesis.

### Working problem statement (provisional)

> Al Noor's five properties retain intentional operational flexibility, which is appropriate to their individual circumstances. However, this flexibility currently extends to how some KPIs are defined and reported, creating recurring reconciliation and clarification work for Group Finance and delaying a trusted, comparable portfolio-level view for management. The organization has not yet established how much of this is caused by process, governance (the absence of agreed definitions), or technology — most likely some combination of the three.

*Status: agreed in principle by session attendees. Not yet formally approved by Executive Management. Do not treat as a finalized problem statement until confirmed in a follow-up session.*

## Meeting 3 — Dedicated Finance Session

**Status: Open — not fully closed.** Nadia (correctly) flagged an unanswered question after the session appeared to wrap; see "Open questions" below. Treat Finance discovery as ongoing, not complete.

**Attendees:** Nadia Hassan (Group Finance Director)
**Caveat stated up front:** Finance's records aren't structured for this kind of analysis — what follows is built from real examples and team experience, not clean statistics. Treated accordingly below.

### Confirmed client statements

**Three concrete, categorized examples were provided** (one per issue type identified in Meeting 2):

| Example | Property | What happened | Category |
|---|---|---|---|
| 1 | Property B | Submitted room revenue didn't agree with its own supporting breakdown; a posting adjustment had been missed. The original figure was actually wrong. | **Data correction** |
| 2 | Property C | Occupancy excluded temporarily-unavailable rooms from the denominator, while corporate used total inventory. Both figures were defensible — the basis differed. | **Definition clarification** |
| 3 | Property D | A revenue figure didn't reconcile with a supporting report because the two were produced at different points in the adjustment process (one reflected the figure before a later adjustment had posted). Not a wrong number — a timing/state mismatch. | **Reconciliation / timing** |

**A sharper three-way framework emerged** (Nadia's own formulation, worth preserving verbatim in spirit):
- Property B asks: *"Is this number actually correct?"* — a **correctness** issue.
- Property C asks: *"What does this KPI mean?"* — a **definition/semantic** issue.
- Property D asks: *"At what point does this number represent the final position?"* — a **process-timing** issue.

All three surface identically from the outside ("the numbers don't match"), which is why treating this as one generic "reporting inconsistency" problem would be a mistake — each needs a different kind of fix. **Important caveat from Nadia: these categories are not necessarily mutually exclusive** — a reconciliation case could turn out to also involve a definition issue. Don't treat the taxonomy as a strict partition until more cases are reviewed.

**Relative effort, by category** (qualitative, not quantified):
- Data correction — usually low effort once confirmed.
- Definition clarification — potentially medium/high effort (requires understanding and agreeing a basis, not just fixing a number).
- Reconciliation/timing — unpredictable; some resolve quickly, others require tracing a number backward through several exchanges.

**Frequency:** "Closer to every monthly cycle" than "a few times a quarter" — multiple clarification exchanges typically occur across the five properties each cycle. Nadia explicitly declined to convert this into a numeric KPI without a proper log, and this should **not** be cited as a precise figure anywhere downstream.

**Other KPIs affected:** Revenue is the next clearest area (questions about which adjustments/categories are included). ADR and RevPAR are derived metrics and can inherit upstream differences, but **no systematic ADR/RevPAR problem has been established** — occupancy remains the best-evidenced example.

**Target-state process, in Nadia's own words:**
- Current: *Receive → investigate → ask property → clarify → reconcile → (investigate again if necessary) → consolidate → report*
- Target: *Receive → validate → consolidate → review → report*

**Success criteria, as described by Finance (not yet a requirement — Finance's own account of what "better" looks like):**
- Less back-and-forth with property teams
- Less time spent tracing why two figures differ
- More confidence that the five-property comparison is genuinely like-for-like where it's supposed to be
- A more predictable monthly reporting cycle
- Faster preparation of the management pack
- Clearer explanations when a property *legitimately* differs from the group basis (not everything should be standardized away)
- **Less dependence on individual Finance staff's informal, memorized knowledge** of how a specific property calculates something — explicitly flagged by Nadia as an easy-to-overlook risk (effectively a key-person/bus-factor risk in the current process)

**Explicit boundary Nadia maintained:** she described desired outcomes, not a system requirement — "I wouldn't want to jump from that statement directly to a technology requirement. We haven't established what mechanism would be appropriate." This boundary should be respected in `03-requirements/` — these are candidate **success/acceptance criteria**, not yet solution requirements.

### Open questions / stakeholder dependencies

- **What happens when an issue remains unresolved at the management-pack reporting deadline?** Flagged by Nadia as genuinely unanswered — not something to assume. Possible outcomes she named without confirming which applies: the pack proceeds using best-available information, Finance holds the report, or an exception gets flagged. **No assumption should be made about which of these is current practice until Finance confirms it directly.**

### Next actions
- Fold the three-category taxonomy and target-state process into `03-requirements/` once requirements drafting begins — strong candidate material for non-functional/process requirements and acceptance criteria.
- Return to Finance for the unresolved-issue-at-deadline question, and for anything the IT session raised that only Finance can answer (see Meeting 4 below).

## Meeting 4 — Dedicated IT Session

**Attendees:** Omar Farouk (Group IT Manager)
**Caveat stated up front:** some details still need verification with individual properties — Omar separated IT-confirmed facts from current-understanding-but-unverified throughout.

### Confirmed client statements

**System landscape, property by property:**

| Property | Current system | IT confidence |
|---|---|---|
| A | Opera PMS | High — centrally known, IT supports the environment |
| B | Opera PMS | High |
| C | Opera PMS | High (this is the property from the March occupancy example) |
| D | **Unknown / not yet confirmed** — a different PMS is suspected | Medium-low — internal records are inconsistent; product name deliberately withheld until verified |
| E | Opera PMS (per IT records) | Medium-high — not independently validated with the property team recently |

**Four of five properties are believed to run Opera; Property D is a genuine open item, not yet an assumption either way.** Omar explicitly cautioned that shared PMS across properties does **not** imply standardized configuration, reporting setup, process, or user practice — the same system can still be operated very differently.

**Property A reporting flow (used as baseline, highest confidence):**
`Front desk/reservations → Opera → month-end property report (reviewed locally) → submitted to Group Finance → Finance consolidation → Finance validation/comparison → (clarification with property if needed) → consolidated management report`
High confidence on the existence of Opera and the overall flow shape; medium confidence on the exact local reports/steps before Finance receives them (flagged as a Finance-side question, not IT's to answer).

**Property C flow:** structurally the same as Property A. The underlying occupancy data was available in Opera — the divergence happened in the **business logic applied to that data** (the occupancy calculation/denominator) before it became the KPI Finance compared, not in system/data capability. This independently corroborates Nadia's "definition clarification" category from the technical side.

**Property D:** genuinely unconfirmed. Omar explicitly declined to extrapolate a different reporting flow just because a different PMS is suspected — flagged as "possibilities, not findings." Five specific items committed for follow-up: which PMS, what reports it generates, how those reports are produced, whether data is manually transformed before submission, and how information reaches Corporate Finance.

**Corporate consolidation method:** confirmed **Excel/spreadsheet-based**, not a centralized BI consolidation process (High confidence). Omar flagged several details he does not have and recommended be asked directly to Finance: which workbook is authoritative, how many intermediate spreadsheets exist, whether formulas/macros are used, whether Finance manually re-enters or imports figures, and whether any BI layer sits downstream of consolidation.

**Integration status:** confirmed **no centralized, automated integration** consolidates the five Opera environments into one corporate dataset (High confidence on the *absence* of this). Current architecture is `Property PMS → Property reporting → File/report submission → Corporate Finance`, not `Five PMS instances → central data platform → automated group reporting`. Some property-level integrations exist for specific operational purposes, but Omar was explicit these shouldn't be assumed relevant to group consolidation without checking.

**Government/tourism authority reporting:** confirmed that external reporting obligations **do exist** for UAE hospitality operations — this corroborates the DET/DTCM-type requirement identified independently in [`../02-research/regulatory-considerations.md`](../02-research/regulatory-considerations.md). However, Omar was explicit this is **not yet a documented technical integration requirement**: handling may differ by emirate/property, may be manual or automated, and may or may not involve Opera directly. Medium confidence — he confirmed the obligation exists but declined to specify a mechanism without property-level verification. Seven items flagged for that verification: which authorities per hotel, what information is submitted, manual vs. automated, source system, whether Opera is directly involved, authority-specific portals/interfaces, and whether requirements differ by emirate.

**Key architectural insight (Omar's own synthesis, independently convergent with Finance's process-side account):** the current architecture has two distinct reporting layers —
- **Property layer:** `Opera → property calculation/reporting → property submission`
- **Corporate layer:** `Property submissions → Excel consolidation → Finance validation → management reporting`

Even a fully standardized PMS landscape across all five properties would **not** eliminate the corporate Excel consolidation layer, which sits entirely outside the PMS. This is why Omar — independently of Nadia — also resists framing this as a "PMS problem."

### Open questions / stakeholder dependencies

- Property D: system identity and full reporting flow (Omar to confirm directly with the property)
- Finance consolidation workbook detail: authoritative file, intermediate spreadsheets, macros/formulas, manual re-entry vs. import, any downstream BI layer — **direct these to Nadia, not IT**
- Government/tourism authority reporting: property-by-property verification of authority, data submitted, automation level, source system, Opera involvement, portals, and emirate-level variation
- Still outstanding from Meeting 3: what happens when a Finance issue remains unresolved at the management-pack deadline

### Next actions
1. Property D confirmation (Omar, owner)
2. Return to Nadia for: the consolidation-workbook detail Omar flagged, and the still-open unresolved-issue-at-deadline question
3. Schedule property-level verification of government/tourism reporting requirements once Property D is resolved
4. Begin drafting `03-requirements/` using the convergent Finance + IT evidence — both independently point to a **definition/governance + process (Excel consolidation) problem**, not a core PMS data-availability problem

## Meeting 5 — Follow-up on Open Items

**Attendees:** Nadia Hassan (Finance), Omar Farouk (IT), via written follow-up

### Confirmed client statements

**Deadline question — now fully resolved (not a gap, a finding):** there is **no formal, documented escalation or exception-handling policy** for an unresolved Finance issue at the management-pack deadline. Current practice is judgment-based: a minor clarification that doesn't materially affect the management view → pack proceeds on best-available information, resolved afterward. A potentially material issue → Finance would normally flag it rather than silently finalize the number; the relevant section *may* be held pending the property's response, but there is no defined rule for when holding applies versus flagging versus proceeding.

**This is itself a governance gap**, in the same family as the absent KPI data dictionary (Meeting 2/3) — worth carrying into `03-requirements/` as a candidate process/governance requirement (e.g., a defined severity-based escalation rule), not just a Finance quirk.

**Property D — partially confirmed:**
- Confirmed: **not** Opera. Exact product name still pending direct validation with the property — Omar deliberately declined to state it unconfirmed.
- Reporting flow structurally appears similar to the other properties (`Property operations → PMS → property-level reports/calculations → property submission → Corporate Finance`), but **medium confidence only** — any additional export/interface/manual-transformation steps specific to Property D are not yet confirmed.

**Government/tourism reporting — existence confirmed, detail still open:**
- Confirmed: property-level government/tourism authority reporting genuinely exists and requirements differ by emirate/authority.
- Still unconfirmed: which reports are automated vs. manual per property, and whether each property's PMS (Opera or otherwise) is the direct source for each regulatory submission.
- Omar's own framing: **do not yet treat this as a confirmed integration requirement** — it needs the full property-level inventory first.

### Decision on how to proceed

Rather than continue chasing Omar for information he's already said requires direct property-team confirmation, these two items are logged as **tracked dependencies with an owner**, not open-ended uncertainty:

| Item | Owner | Status |
|---|---|---|
| Property D — exact PMS and full reporting flow | Omar Farouk (IT), pending property confirmation | In progress |
| Government/tourism reporting — property-by-property inventory | Omar Farouk (IT), pending property-level engagement | Not yet started |

Both should be carried into the RFP/requirements process as **explicit dependencies to resolve before final scope or vendor selection is confirmed** — not as blockers to drafting requirements now.

### Next actions
1. Discovery phase findings are now sufficient to begin `03-requirements/` — proceed.
2. Carry the two tracked dependencies above forward explicitly; do not let them silently drop.
3. Carry the "no formal escalation policy" finding forward as a candidate governance/process requirement.
