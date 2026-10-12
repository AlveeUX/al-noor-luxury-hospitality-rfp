# Proposed Solution and Approach

## What we'd build

A **Group KPI Governance & Consolidation Workspace** — a single place where KPI definitions are agreed and versioned, property submissions are validated against those definitions before they're consolidated, clarification cases are logged and tracked, unresolved issues are escalated by a documented rule, and legitimate property-level variances are recorded rather than treated as errors.

At a structural level, the workspace has eight areas:

| Area | What it does | Which requirement it satisfies |
|---|---|---|
| Dashboard | Cycle status, open cases, pending approvals, escalations this cycle | — |
| KPI Dictionary | Definitions, formulas, owners, version history, change proposals | FR-01, FR-02 |
| Consolidation Workspace | Property submission intake, pre-consolidation validation, draft and published consolidated report | FR-04, FR-05 |
| Case Log | Clarification cases, categorized, with resolution time | FR-06, FR-07 |
| Escalation Queue | Deadline-driven alerts, severity assessment, logged decisions | FR-08 |
| Property Variance Register | Approved/pending/rejected variances, visible to corporate Finance | FR-03, FR-11 |
| Regulatory Reporting Register | Populated once the property-by-property inventory is confirmed | FR-10 (future phase) |
| Admin & Access | Role-based access aligned to the governance RACI | NFR-07 |

## Our approach: governance before interface

We agree with the RFP's own framing — building a tool before the KPI dictionary is agreed just automates today's ambiguity faster. So our delivery sequence deliberately puts governance work *before* any screen gets designed:

1. **Validate the dictionary and process with the people who'll use it** — Finance, IT, and Property GMs — before UX work starts. Mandatory property consultation isn't a feature we bolt on later; it's step one.
2. **Design and build against one confirmed KPI first.** Occupancy is the only KPI with a confirmed definitional dispute today. We would not build dictionary entries for revenue, ADR, or RevPAR speculatively — each gets added only once independently confirmed as affected, same discipline the RFP itself applies.
3. **Pilot before rollout.** One or two properties run a full monthly cycle on the new validate-then-consolidate process before we touch the other three. This is a deliberate parallel-run safeguard — Al Noor's current process, however manual, is the operational baseline, and we're not willing to put that at risk group-wide on an unproven pilot.
4. **Preserve property autonomy by design, not by caveat.** The variance register isn't an edge case we handle later — it's in the core workspace from day one, because without it, any governance process risks becoming exactly the "corporate imposing definitions" outcome both Property GMs in your evidence were wary of.

## Build vs. buy

The RFP (§0) leaves this open, and so do we — but we want to be direct about what each path means for this proposal:

- **If build:** this response's scope, timeline, team, and estimate apply as written.
- **If buy:** we can instead lead vendor evaluation, configuration, and integration of a selected platform against the same requirements set — a materially different (and likely smaller) engagement. We'd want this decided before Phase 1 starts, not during it, because it changes almost everything downstream.

## What we are explicitly not proposing

- No replacement of any property's PMS, reservations, or front-desk system.
- No guest-facing functionality — booking engine, channel manager, POS/F&B, or guest CRM.
- No government/tourism-authority reporting integration in this phase — that's scoped separately, once Al Noor's property-by-property inventory is complete (see Assumptions, Risks & Dependencies).
- No assumption that the fifth property is ready to onboard — we've scoped for four properties now, with the fifth added once its system is confirmed.
