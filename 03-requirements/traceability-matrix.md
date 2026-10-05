# Requirements Traceability Matrix — Al Noor Luxury Hospitality Group

**Purpose:** every requirement in this folder must trace back to either a confirmed discovery finding or a sourced research finding — the standing rule in [`../DECISIONS.md`](../DECISIONS.md). This table is that trace, in one place.

**Status key:** **Confirmed** = directly evidenced by a stakeholder statement. **Candidate** = BA-derived from confirmed evidence, not yet itself validated with stakeholders. **Pending** = blocked on a tracked dependency.

| ID | Type | Requirement (short) | Source | Status |
|---|---|---|---|---|
| US-01 / FR-01 | User story / Functional | KPI/business definition dictionary | Meeting 2 (no dictionary exists — confirmed by Finance and IT independently) | Confirmed need; dictionary content itself is Candidate |
| US-02 / FR-02 | User story / Functional | Property-GM consultation before a definition is finalized | Meeting 2 (both GMs' caveat) | Confirmed need |
| US-03 | User story | Formal Executive approval of Finance as definition owner | Meeting 2; [`../DECISIONS.md`](../DECISIONS.md) "Pending approval" entry | Confirmed gap (approval itself is Pending) |
| US-04 / FR-04 | User story / Functional | Redesigned consolidation process (validate-first) | Meeting 3 (Nadia's current vs. target process) | Confirmed (Nadia's own account) |
| US-05 / FR-05 / NFR-01 | User story / Functional / Non-functional | Single authoritative, documented, auditable consolidation source | Meeting 3 (bus-factor risk); Meeting 4 (Excel-based, no centralized integration — confirmed) | Confirmed |
| US-06 / FR-06 / FR-07 | User story / Functional | Classified, logged, measured clarification cases | Meeting 3 (three-way framework: correctness / definition / process-timing; frequency not quantified) | Confirmed categories; measurement itself is Candidate |
| US-07 / FR-08 | User story / Functional | Documented escalation policy for unresolved deadline issues | Meeting 5 (confirmed: no formal policy exists today) | Confirmed gap |
| US-08 / FR-03 / FR-11 | User story / Functional | Property-level variance mechanism; preserved property autonomy | Meeting 2 (Khalid's autonomy correction; both GMs' caveat) | Confirmed |
| US-09 / FR-10 | User story / Functional | Government/tourism-authority reporting inventory | Meeting 4 (existence confirmed, mechanism not); Meeting 5 (still open); [`../02-research/regulatory-considerations.md`](../02-research/regulatory-considerations.md) | Pending — tracked dependency (owner: Omar Farouk) |
| US-10 / FR-12 | User story / Functional | Property D confirmation | Meeting 4; Meeting 5 | Pending — tracked dependency (owner: Omar Farouk) |
| NFR-02 | Non-functional | PDPL compliance | [`../02-research/regulatory-considerations.md`](../02-research/regulatory-considerations.md) | Confirmed (research-sourced) |
| NFR-03 | Non-functional | Usability for non-technical staff | Meeting 2 (GMs wary of corporate-imposed complexity) | Confirmed concern; requirement wording is Candidate |
| NFR-04 | Non-functional | Reporting-cycle timeliness target | Meeting 3 (Nadia declined to quantify) | Open / TBD — explicitly not to be invented |
| NFR-05 | Non-functional | Scalability beyond five properties | Not discovered either way | Candidate / soft assumption only (BRD §7, A4) |
| NFR-06 | Non-functional | Availability during reporting window | Inferred from criticality of monthly cycle (Meeting 3) | Candidate |
| NFR-07 | Non-functional | Role-based access aligned to RACI | [`../01-discovery/stakeholder-map.md`](../01-discovery/stakeholder-map.md) RACI (itself pending formal approval — see US-03) | Candidate, dependent on US-03 |
| NFR-08 | Non-functional | Localization (Arabic/English) | Discovery questionnaire Q4.4 — never asked in a session | Open — not investigated |
| NFR-09 | Non-functional | Vendor/solution neutrality | Meeting 2 (explicit risk: don't let software solve a governance problem) | Confirmed risk driving this constraint |

## Items explicitly NOT carried into requirements (and why)

| Item | Reason |
|---|---|
| Procurement / guest-service metrics inconsistency | Raised only as a GM hypothesis in Meeting 2; both GMs cautioned against assuming it without concrete evidence. Standing decision: do not add to scope on a hypothesis. |
| Revenue, ADR, RevPAR as *confirmed* problem KPIs | Nadia named these as "plausible," not confirmed (Meeting 3). Carried only as candidate dictionary entries (FR-01), not as confirmed findings. |
| Specific reporting-cycle time target | Explicitly declined by Finance pending measurement (Meeting 3). See NFR-04. |
| Original brief's module list (reservations, housekeeping, billing, etc.) | Never validated in discovery as in-scope pain points — remains an unconfirmed assumption from the original brief, not a requirement. |

## Open approvals blocking full sign-off

1. Executive Management approval of Finance as KPI/definition owner (US-03).
2. Stakeholder review of this entire requirements set with Khalid, Nadia, and Omar (BRD §11) — has not yet happened.
3. Resolution of the two tracked dependencies (US-09, US-10) before Epic E can move past "Pending."
