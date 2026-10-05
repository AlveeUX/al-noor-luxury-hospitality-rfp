# Request for Proposal (Draft) — Group KPI Governance & Consolidation Capability

**Status: Draft.** This RFP is **deliberately not** the five-property "Hotel Management System" RFP named in the original brief ([`../01-discovery/client-brief-v0.1.md`](../01-discovery/client-brief-v0.1.md)). Discovery and the technology option analysis ([`../05-technology/system-context-and-options.md`](../05-technology/system-context-and-options.md)) found no evidence that a PMS replacement addresses the confirmed problem. Issuing the original RFP as-brief would have asked vendors to solve the wrong problem.

## 0. Procurement approach — read before scoping a vendor search

Per [`../05-technology/system-context-and-options.md`](../05-technology/system-context-and-options.md), governance (Option A) must precede any tooling. This document assumes governance work is underway or complete and that Procurement has decided a **build-vs-buy** question is still open:

- **Buy:** if a suitable off-the-shelf or configurable platform (e.g., a workflow/data-governance tool Al Noor already licenses) can satisfy [`../03-requirements/functional-requirements.md`](../03-requirements/functional-requirements.md) without disproportionate customization, a scoped vendor RFP (this document) is appropriate.
- **Build:** if no reasonable off-the-shelf fit exists at this scale (five properties, ~12 functional requirements), an internal build using existing group tooling may be more proportionate than running a vendor procurement at all. **This decision has not been made** — Khalid (Procurement) and Omar (IT) should make it before this RFP is issued, not after.

## 1. Background

Al Noor Luxury Hospitality Group operates five five-star properties across the UAE. A confirmed governance gap — no agreed KPI/business definitions, a manual Excel consolidation layer, and no formal escalation policy — creates recurring Finance reconciliation work and delays trusted, comparable group reporting. Full evidence trail: [`../01-discovery/interview-notes.md`](../01-discovery/interview-notes.md).

## 2. Scope of work

### In scope
- A KPI/business definition dictionary with version control and a governed change process (FR-01, FR-02)
- A consolidation workspace that validates property submissions against the dictionary before consolidating (FR-04, FR-05)
- Clarification-case logging and categorization (FR-06, FR-07)
- A severity-based escalation workflow (FR-08)
- A documented property-variance mechanism (FR-03, FR-11)
- Role-based access aligned to the RACI in [`../01-discovery/stakeholder-map.md`](../01-discovery/stakeholder-map.md) (NFR-07)

### Explicitly out of scope
- Replacement of any property's PMS
- Guest-facing functionality, booking engine, channel manager, POS/F&B, or guest CRM integration
- Government/tourism-authority reporting integration — **tracked dependency (US-09), to be scoped separately once the property-by-property inventory completes**
- Property D-specific integration — pending confirmation (US-10)

## 3. Objectives and success criteria

See [`../03-requirements/business-requirements-document.md`](../03-requirements/business-requirements-document.md) §4 and §8. Candidate acceptance criteria are explicitly labeled there as **not yet stakeholder-approved** — vendors should not expect these to be contractually final without a validation pass.

## 4. Requirements reference

Full functional and non-functional requirements: [`../03-requirements/functional-requirements.md`](../03-requirements/functional-requirements.md), [`../03-requirements/non-functional-requirements.md`](../03-requirements/non-functional-requirements.md). Vendors must complete the compliance matrix in [`vendor-response-template.md`](vendor-response-template.md) against every requirement ID — a narrative response without ID-level traceability will not be scored.

## 5. Vendor qualification

- Demonstrated experience with multi-entity data governance and/or financial consolidation workflows (hospitality experience is a plus, not a prerequisite — this is explicitly not a PMS procurement)
- Ability to comply with UAE Federal Decree-Law No. 45 of 2021 (PDPL) — see [`../02-research/regulatory-considerations.md`](../02-research/regulatory-considerations.md)
- Willingness to support a phased rollout (see [`../07-estimation-and-delivery/delivery-phases.md`](../07-estimation-and-delivery/delivery-phases.md)), starting with a single-KPI pilot (occupancy)

## 6. Timeline

**Not confirmed.** No go-live date or procurement deadline has been disclosed (BRD §7, A3). Any date inserted here before that confirmation would be invented.

## 7. Evaluation

Summarized here; full detail in [`evaluation-matrix.md`](evaluation-matrix.md). Proposals are scored on functional compliance, non-functional/compliance fit, implementation approach, vendor experience, and commercial terms.
