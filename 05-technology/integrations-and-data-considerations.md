# Integrations & Data Considerations — Al Noor Luxury Hospitality Group

**Status: Draft**, scoped to the recommended Option B (lightweight governance & consolidation tool) in [`system-context-and-options.md`](system-context-and-options.md). If that recommendation changes, this document must be revisited — it is not independent of it.

## 1. Core data entities

| Entity | Description | First appears in |
|---|---|---|
| KPI Definition | Name, formula, owner, effective date, version history | FR-01 |
| Property Submission | A property's monthly figures as received, pre-validation | FR-04 |
| Consolidation Record | Validated, consolidated group-level figures | FR-05 |
| Clarification Case | A logged discrepancy, categorized and tracked to resolution | FR-06, FR-07 |
| Escalation Record | An issue unresolved at the deadline, with action taken and rationale | FR-08, FR-09 |
| Property Variance | An approved, documented departure from a group definition | FR-03 |
| Regulatory Reporting Entry | Per-property government/tourism obligation record | FR-10 (Pending — US-09) |

## 2. Integration touchpoints

**No direct PMS integration is required to satisfy the confirmed requirements.** This is a direct consequence of Meeting 4's key finding: the problem is in business logic and the Excel consolidation layer, not in PMS data capture. Four of five properties' PMS (Opera) already reliably captures the underlying data (Meeting 4, "high confidence").

- **Property submission intake:** file/manual upload, matching the current process shape (Property → report → Corporate Finance). Automating this intake is a candidate future enhancement, not a day-one requirement — no evidence currently justifies the added integration cost.
- **Government/tourism-authority reporting:** **not yet a confirmed integration requirement** (Omar's own words, Meeting 4/5). Any integration design here must wait for the property-by-property inventory (US-09) to complete. Building against assumed authority/portal specifics now would risk building the wrong thing.
- **Property D:** once confirmed (US-10), assess whether its PMS/reporting flow differs enough from the other four to need separate handling. Not assumed either way currently.

## 3. Data residency and privacy

- UAE Federal Decree-Law No. 45 of 2021 (PDPL) applies — see [`../02-research/regulatory-considerations.md`](../02-research/regulatory-considerations.md) and NFR-02.
- The data entities in §1 are operational/financial (KPI figures, case logs), not guest personal data. **This distinction has not been explicitly confirmed with IT or Finance** — it is a reasonable inference from the discovery evidence, not a verified fact, and should be validated before any data residency decision is finalized.
- If a government/tourism-reporting integration is later built (contingent on US-09), that pathway is far more likely to involve guest-level data and would need its own privacy assessment — explicitly out of scope for this document.

## 4. Sequencing dependency (data quality)

A consolidation tool is only as good as the KPI dictionary behind it (US-01). Building Option B's data model before the dictionary is agreed would encode the current ambiguity rather than resolve it — this is the technical mirror of the governance-before-tooling sequencing argument in [`system-context-and-options.md`](system-context-and-options.md) §3.
