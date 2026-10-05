# Functional Requirements — Al Noor Luxury Hospitality Group

**Status: Draft.** Derived from [`user-stories.md`](user-stories.md). **Framing note:** per the risk flagged in discovery (Meeting 2 — "risk of writing RFP requirements that ask a vendor to solve what is actually an internal governance problem through software alone"), these requirements are written against *capabilities needed*, not a named system. Each may be satisfied by a governance/process change, a configuration of existing tools, or new software — which approach is appropriate is a question for [`../05-technology/`](../05-technology/), not this document.

| ID | Requirement | Derived from |
|---|---|---|
| FR-01 | Maintain a version-controlled KPI/business definition dictionary capturing, per KPI: name, definition, calculation formula/denominator rules, owner, effective date, and revision history. Occupancy is the first entry; revenue, ADR, and RevPAR are candidate entries pending Finance validation. | US-01 |
| FR-02 | Provide a documented process for proposing, reviewing (including mandatory property-GM consultation), approving, and publishing KPI definition changes. | US-01, US-02 |
| FR-03 | Support recording an approved, documented property-level variance to a group KPI definition, distinct from — and visible separately to — an unapproved inconsistency. | US-08 |
| FR-04 | Validate property-submitted figures against the current, agreed KPI definitions *before* consolidation (a "validate" step preceding consolidation, replacing ad hoc investigation after the fact). | US-04 |
| FR-05 | Maintain a single authoritative source for group consolidation, with documented formulas, macros, and data sources — replacing undocumented reliance on individual staff knowledge. | US-05 |
| FR-06 | Classify and log each Finance clarification case by category (data correction / definition clarification / reconciliation-timing), supporting more than one category per case, with property, date, and resolution time captured. | US-06 |
| FR-07 | Produce volume and frequency reporting on logged clarification cases, by category and property, to establish a measured baseline in place of the current qualitative estimate. | US-06 |
| FR-08 | Enforce a documented, severity-based escalation/exception rule for cases unresolved at the reporting deadline (proceed on best-available information / hold pending response / flag as exception), applied consistently across properties. | US-07 |
| FR-09 | Maintain an auditable change history of who changed a KPI definition or a consolidation figure/formula, when, and why. | US-05, US-07 |
| FR-10 | Maintain a property-by-property register of government/tourism-authority reporting obligations (authority, data elements submitted, automation level, source system, portal/interface), with a per-property status field (Confirmed / Pending). | US-09 |
| FR-11 | Preserve each property's ability to operate its own day-to-day PMS/operations independently. Governance under FR-01–FR-09 applies only to the group-level comparable KPI layer, not to property operational configuration in general. | US-08, Meeting 2 (Khalid's correction) |
| FR-12 | Record Property D's confirmed PMS product and full reporting flow once validated, bringing it to parity with the documentation held for Properties A–C. | US-10 |

*Explicitly excluded from this list (not evidenced, or out of scope per BRD §5.2): guest-facing functionality, booking engine/channel manager integration, POS/F&B modules, and any requirement implying a specific new Hotel Management System purchase.*
