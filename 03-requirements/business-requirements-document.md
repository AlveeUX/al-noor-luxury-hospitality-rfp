# Business Requirements Document (BRD) — Al Noor Luxury Hospitality Group

**Status: Draft.** Authored by the BA from discovery evidence in [`../01-discovery/interview-notes.md`](../01-discovery/interview-notes.md) and [`../02-research/`](../02-research/). **Not yet circulated for stakeholder sign-off.** Every statement below is either a confirmed discovery finding (cited) or an explicitly labeled BA-derived candidate requiring validation. Nothing here should be read as agreed scope until reviewed with Khalid Rahman, Nadia Hassan, and Omar Farouk, and formally approved by Executive Management where noted.

---

## 1. Document control

| | |
|---|---|
| Prepared by | BA (Absar Alvee), practice case study |
| Based on | Discovery Meetings 2–5 ([`interview-notes.md`](../01-discovery/interview-notes.md)), original brief ([`client-brief-v0.1.md`](../01-discovery/client-brief-v0.1.md)), regulatory research ([`regulatory-considerations.md`](../02-research/regulatory-considerations.md)) |
| Status | Draft — pending stakeholder validation |
| Version | 0.1 |

## 2. Background

The engagement originated from a one-paragraph Procurement brief requesting a "Hotel Management System" for five five-star properties across the UAE (see [`client-brief-v0.1.md`](../01-discovery/client-brief-v0.1.md)). Per the project's standing decision to treat a named solution as a *requested* solution rather than a confirmed need (see [`../DECISIONS.md`](../DECISIONS.md)), discovery was run before any requirement was drafted.

Discovery (a joint session plus dedicated Finance and IT sessions) did **not** confirm a PMS data-availability problem. Instead, two independent stakeholders converged on the same underlying issue from different angles:

- **Finance (process view):** recurring reconciliation and clarification work caused by undefined KPI/business definitions and a manual Excel consolidation layer (Meeting 3).
- **IT (technical view):** the PMS layer (Opera, for 4 of 5 properties) reliably captures the underlying data; the divergence happens in *business logic applied to that data* before it reaches Finance, and in a corporate Excel consolidation layer that sits entirely outside any PMS (Meeting 4).

This is why the requirements below are deliberately **solution-agnostic where possible** — they describe what must be true of the governance, process, and (where applicable) supporting tooling, not a predetermined piece of software. A risk was explicitly raised in discovery against writing RFP requirements that ask a vendor to solve what is actually an internal governance problem through software alone (Meeting 2, Risks).

## 3. Problem statement

> Al Noor's five properties retain intentional operational flexibility, which is appropriate to their individual circumstances. However, this flexibility currently extends to how some KPIs are defined and reported, creating recurring reconciliation and clarification work for Group Finance and delaying a trusted, comparable portfolio-level view for management. No formal KPI/business definition dictionary exists, group consolidation runs through a manual Excel layer outside any PMS, and no formal escalation policy exists for issues unresolved at the reporting deadline.

*Carried forward, word-for-word in substance, from the provisional problem statement agreed in Meeting 2 and corroborated by Meetings 3–5. Still described there as "agreed in principle... not yet formally approved by Executive Management" — that approval status has not changed during requirements drafting and should be sought before this BRD is finalized.*

## 4. Business objectives

Derived from Finance's own description of what "better" looks like (Meeting 3, explicitly framed by Nadia as outcomes, not yet requirements) and Khalid's framing in Meeting 2:

1. A trusted, comparable, group-level view of property performance for management — without overriding legitimate property-level operating differences.
2. Reduced Finance reconciliation and clarification workload.
3. A more predictable, faster monthly reporting cycle.
4. Reduced dependence on individual staff's undocumented knowledge of how a given property's figures are built (the "bus-factor" risk Nadia flagged).
5. A consistent, documented way to handle issues that are unresolved when the reporting deadline arrives.

These are BA-synthesized from Finance's account and **not yet validated as formal success criteria** — see §8.

## 5. Scope

### 5.1 In scope for this phase of requirements

- Governance process and ownership for KPI/business definitions (Epic A, see [`user-stories.md`](user-stories.md))
- The group consolidation and reporting process, including its current manual Excel layer (Epic B)
- A formal escalation/exception policy for unresolved issues at the reporting deadline (Epic C)
- Preservation of legitimate property-level flexibility within a governed definition process (Epic D)
- A property-by-property inventory of government/tourism-authority reporting obligations — tracked as a dependency, not yet a confirmed integration requirement (Epic E)

### 5.2 Explicitly out of scope / deferred

- **Procurement and guest-service metrics.** Both property GMs raised this as a *possible* parallel issue in Meeting 2 but explicitly cautioned against assuming it's the same problem without concrete evidence. Per standing decision in [`../DECISIONS.md`](../DECISIONS.md), this is not added to scope on a hypothesis.
- **Technology/vendor selection.** Whether any new system is needed at all — versus governance and process change alone — is an open question this BRD does not presuppose. Vendor and architecture evaluation is deferred to [`../05-technology/`](../05-technology/) and [`../06-rfp-and-commercial/`](../06-rfp-and-commercial/).
- **UX/product design** of any supporting tooling — deferred to [`../04-ux-and-product/`](../04-ux-and-product/).
- **Original brief's full module list** (reservations, front desk, housekeeping, billing — see [`client-brief-v0.1.md`](../01-discovery/client-brief-v0.1.md)) — none of these were confirmed as in-scope pain points during discovery; they remain unvalidated assumptions from the original brief, not requirements.

## 6. Stakeholders

See [`../01-discovery/stakeholder-map.md`](../01-discovery/stakeholder-map.md) for the full map and RACI. Summary of confirmed participants: Khalid Rahman (Procurement, process owner), Nadia Hassan (Finance, tentative accountable owner of KPI definitions — pending formal approval), Omar Farouk (IT, consulted), Mariam Al Mazrouei and Daniel Thomas (Property GMs, consulted). Three of five property GMs have not yet been engaged — any requirement below describing "property-level" impact should be read as evidenced by two of five properties unless stated otherwise.

## 7. Assumptions and constraints

| # | Assumption / constraint | Status |
|---|---|---|
| A1 | Four of five properties run Opera PMS; Property E is medium-high confidence (not independently re-validated recently) | From Meeting 4 — not a requirement input, context only |
| A2 | No budget range has been disclosed | Confirmed absence, per original brief — estimation work in later phases must flag this |
| A3 | No go-live date or procurement deadline has been disclosed | Confirmed absence |
| A4 | The group may expand beyond five properties in future | Not confirmed either way — treated as a soft scalability consideration only (see NFR-05), not a scope commitment |
| A5 | Finance's frequency estimate ("closer to every monthly cycle" than quarterly) is qualitative, not measured | Nadia explicitly declined to give a number for this purpose (Meeting 3) — do not cite as a business-case figure |

## 8. Success / acceptance criteria (candidate — not yet approved)

Finance's own account of what "better" looks like (Meeting 3), explicitly described by Nadia as *outcomes*, not requirements: "I wouldn't want to jump from that statement directly to a technology requirement." Carried here as **candidate acceptance criteria** pending a formal validation session:

- Less back-and-forth with property teams during consolidation
- Less time spent tracing why two figures differ
- Confidence that the five-property comparison is genuinely like-for-like where it's supposed to be
- A more predictable monthly reporting cycle; faster management-pack preparation
- Clear, documented explanations when a property *legitimately* differs from the group basis
- Reduced dependence on individual staff's informal/memorized knowledge of property-specific calculations

## 9. Dependencies (tracked, not blockers)

Per [`../DECISIONS.md`](../DECISIONS.md), these are carried forward explicitly rather than re-chased or assumed:

| Dependency | Owner | Status |
|---|---|---|
| Property D — exact PMS and full reporting flow | Omar Farouk (IT), pending property confirmation | In progress |
| Government/tourism-authority reporting — property-by-property inventory | Omar Farouk (IT), pending property-level engagement | Not yet started |

## 10. Risks carried into requirements

- Writing requirements that implicitly ask a future vendor to solve an internal governance problem (agreeing KPI definitions) through software alone (Meeting 2).
- Treating the single March occupancy example as representative of a systemic issue without further evidence across properties and KPIs (Meeting 2) — mitigated here by scoping occupancy as the only *confirmed* KPI-level finding; revenue/ADR/RevPAR remain candidate, not confirmed (Meeting 3).
- Over-standardizing and removing legitimate property-level flexibility if group definitions are imposed without a proper agreement process (Meeting 2) — addressed directly in Epic D.

## 11. Open governance items

- Formal Executive Management approval of Finance as accountable owner of KPI/business definitions has not yet been obtained (Meeting 2) — see US-03.
- This BRD itself has not been reviewed with stakeholders. Recommended next step: circulate this document and [`user-stories.md`](user-stories.md) to Khalid, Nadia, and Omar for validation before any RFP or technology-scoping work proceeds.

## 12. Related documents

[`user-stories.md`](user-stories.md) · [`functional-requirements.md`](functional-requirements.md) · [`non-functional-requirements.md`](non-functional-requirements.md) · [`traceability-matrix.md`](traceability-matrix.md)
