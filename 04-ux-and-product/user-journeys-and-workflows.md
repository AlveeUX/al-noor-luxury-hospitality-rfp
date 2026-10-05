# User Journeys & Workflows — Al Noor Luxury Hospitality Group

**Status: Draft.** Two of the journeys below (A, B) are taken directly from confirmed discovery statements. The remaining three (C, D, E) are BA-derived workflows that would be needed to deliver the user stories in [`../03-requirements/user-stories.md`](../03-requirements/user-stories.md) — they describe a process, not necessarily new software, and are marked **Candidate** accordingly.

---

## A. Current-state: Monthly Consolidation (Confirmed — Meeting 3)

| Step | Actor | Pain point (if any) |
|---|---|---|
| 1. Receive | Finance | Property submissions arrive with no upfront validation against an agreed definition |
| 2. Investigate | Finance | Manual tracing of discrepancies; relies on individual staff's undocumented knowledge (bus-factor risk) |
| 3. Ask property | Finance → Property | Round trip, adds cycle time |
| 4. Clarify | Property → Finance | No shared vocabulary for *why* figures differ (data error vs. definition vs. timing) |
| 5. Reconcile | Finance | Unpredictable effort — "some resolve quickly, others require tracing a number backward through several exchanges" |
| 6. (Investigate again, if necessary) | Finance | Loop back to step 2 for unresolved cases |
| 7. Consolidate | Finance | Performed in Excel, no centralized integration (Meeting 4) |
| 8. Report | Finance | Delivered to management; deadline handling is judgment-based, no formal escalation rule (Meeting 5) |

## B. Target-state: Monthly Consolidation (Confirmed — Nadia's own account, Meeting 3)

`Receive → validate → consolidate → review → report`

The compression from 8 steps to 5 is Nadia's own framing of what "better" looks like — explicitly stated as a desired outcome, not yet a system requirement. The **validate** step is the structural change: checking submissions against an agreed KPI dictionary (US-01) *before* consolidation, rather than discovering mismatches during it. See [`../03-requirements/user-stories.md`](../03-requirements/user-stories.md) US-04.

---

## C. Candidate workflow: Propose & Approve a KPI Definition Change

Derived from US-01 / US-02 / US-03 / FR-01 / FR-02 — no equivalent process exists today (confirmed absence, Meeting 2).

1. **Propose** — Finance (or IT, consulted) drafts a new or revised KPI definition (name, formula, denominator rules).
2. **Property consultation** — Each affected property GM is notified and has a documented opportunity to object or request a variance (US-02). Consultation is mandatory; unanimous consent is not.
3. **Finance review** — Definitions owner (Nadia, pending US-03) reviews GM input and either finalizes or revises the proposal.
4. **Executive approval (first-time/ownership-level changes only)** — Required while Finance's ownership role itself remains "pending approval" (see US-03); once formally approved, routine definition updates may not need to reach this step every time — **this escalation threshold is itself undecided and should be confirmed with stakeholders, not assumed.**
5. **Publish** — Definition enters the dictionary with a version number and effective date (FR-01).
6. **Notify** — All consulted stakeholders are informed of the published definition.

## D. Candidate workflow: Escalate an Unresolved Issue at the Reporting Deadline

Derived from US-07 / FR-08 — addresses the confirmed governance gap in Meeting 5 (no formal policy exists today).

1. **Detect** — A clarification case (see Epic B) remains open as the management-pack deadline approaches.
2. **Assess severity** — Finance determines whether the issue materially affects the management view. *(The specific severity criteria are not yet defined — this is the policy Epic C's user story (US-07) calls for, not something this project can assume on Finance's behalf.)*
3. **Act per policy** — One of three documented actions: proceed on best-available information; hold the affected section pending the property's response; or flag as an exception in the management pack.
4. **Log** — The decision and its rationale are recorded (supports FR-09, auditability).
5. **Resolve post-hoc** — If held or flagged, the case is tracked to resolution in the next cycle.

## E. Candidate workflow: Submit & Approve a Property-Level Variance

Derived from US-08 / FR-03 — addresses the over-standardization risk both GMs raised in Meeting 2.

1. **Identify** — A property GM identifies a group definition that doesn't fit a legitimate local circumstance.
2. **Submit** — GM documents the requested variance and its operational justification.
3. **Review** — Finance (definitions owner) and the requesting property jointly review.
4. **Decide** — Approved variances are recorded and made visible to corporate Finance (not silently applied); rejected requests return to the standard definition, with the GM's objection still logged per US-02.
5. **Distinguish from inconsistency** — An approved variance is explicitly not the same as an unapproved inconsistency (Epic B's clarification-case log) — the two must not be conflated in reporting.

---

*Journeys C–E are not yet validated with Khalid, Nadia, or Omar — see [`../03-requirements/business-requirements-document.md`](../03-requirements/business-requirements-document.md) §11. Treat step sequencing and the escalation-threshold question in Workflow C, step 4, as draft until confirmed.*
