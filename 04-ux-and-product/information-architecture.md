# Information Architecture — Al Noor Luxury Hospitality Group

**Status: Draft — illustrative candidate, not a committed design.** This IA sketches one way the functional requirements in [`../03-requirements/functional-requirements.md`](../03-requirements/functional-requirements.md) could be organized **if** a supporting tool is the chosen delivery mechanism. Per NFR-09 (vendor/solution neutrality), nothing here commits the project to new software — [`../05-technology/`](../05-technology/) has not yet decided whether these capabilities are delivered by a new tool, a reconfiguration of existing tools, or process/governance change alone. Working name used purely for reference: **"Group KPI Governance & Consolidation Workspace."**

---

## Top-level structure

```
Group KPI Governance & Consolidation Workspace
│
├── 1. Dashboard
│   └── Consolidation cycle status · open cases · pending approvals · escalations this cycle
│
├── 2. KPI Dictionary                         → satisfies FR-01, FR-02
│   ├── Definitions list (by KPI)
│   ├── Definition detail (formula, owner, effective date)
│   ├── Version history
│   └── Propose a change (→ Workflow C)
│
├── 3. Consolidation Workspace                → satisfies FR-04, FR-05
│   ├── Property submissions (intake)
│   ├── Validation results (flagged against current dictionary)
│   ├── Consolidated report (draft)
│   └── Review & publish
│
├── 4. Case Log                               → satisfies FR-06, FR-07
│   ├── Clarification cases (list, filterable by category/property)
│   ├── Case detail (category tags, resolution time)
│   └── Volume/frequency reporting
│
├── 5. Escalation Queue                       → satisfies FR-08
│   ├── Issues approaching deadline
│   ├── Severity assessment
│   └── Escalation log (action taken + rationale)
│
├── 6. Property Variance Register             → satisfies FR-03, FR-11
│   ├── Variance requests (pending / approved / rejected)
│   └── Active variances by property
│
├── 7. Regulatory Reporting Register          → satisfies FR-10 (Pending — see US-09)
│   └── Property-by-property government/tourism obligations, status: Confirmed / Pending
│
└── 8. Admin & Access                         → satisfies NFR-07
    └── Roles: Finance (owner) · IT (consulted) · Property GM (consulted/viewer) · Executive (informed)
```

## Navigation and access notes

- Primary navigation reflects the five functional epics from [`../03-requirements/user-stories.md`](../03-requirements/user-stories.md): Governance (2), Process (3, 4), Exception handling (5), Autonomy (6), Regulatory (7).
- Section 7 (Regulatory Reporting Register) is populated incrementally as the tracked dependency (US-09) resolves — it should not imply completeness it doesn't have. Its per-entry status field (Confirmed/Pending) is load-bearing, not cosmetic.
- Role-based visibility (section 8) follows the RACI in [`../01-discovery/stakeholder-map.md`](../01-discovery/stakeholder-map.md), itself pending formal approval (US-03) — access rules here should be treated as provisional until that RACI is confirmed.
- No guest-facing, booking, or operational-module navigation (reservations, housekeeping, billing) is included — none of these were confirmed as in-scope pain points (see [`../03-requirements/business-requirements-document.md`](../03-requirements/business-requirements-document.md) §5.2).

## Open IA questions (not yet answerable from discovery evidence)

- Localization/navigation language (Arabic/English) — NFR-08, not yet investigated.
- Whether Property GMs need a dedicated "My Property" filtered view, or whether the Consolidation Workspace and Variance Register are sufficient — no session has tested this with a GM directly.
