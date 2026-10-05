# Non-Functional Requirements — Al Noor Luxury Hospitality Group

**Status: Draft.** Several entries below are marked **TBD** rather than given an invented figure, consistent with the project's traceability principle — Finance explicitly declined to supply numbers that would be "treated as a requirement or business case figure" before they're actually measured (Meeting 3).

| ID | Requirement | Note |
|---|---|---|
| NFR-01 | **Auditability.** Every change to a KPI definition or a consolidation formula/figure must be attributable to a person, timestamped, and reversible. | Directly addresses the "bus-factor"/key-person risk named in Meeting 3. |
| NFR-02 | **Regulatory compliance.** Any process or system handling guest or property data must comply with UAE Federal Decree-Law No. 45 of 2021 (PDPL). | See [`../02-research/regulatory-considerations.md`](../02-research/regulatory-considerations.md). |
| NFR-03 | **Usability for non-technical staff.** KPI definitions and governance workflows must be usable by Finance and property GM staff without specialist technical training — both GMs were wary of corporate-imposed complexity (Meeting 2). | Plain-language definitions, not purely technical specs. |
| NFR-04 | **Reporting-cycle timeliness.** Monthly consolidation and reporting must complete within an agreed cycle time. | **TBD** — no current cycle-time baseline exists; Nadia explicitly declined to estimate one (Meeting 3). To be measured via FR-07 before a target is set. |
| NFR-05 | **Scalability.** The governance model and any supporting tooling should reasonably accommodate the current five properties and foreseeable near-term growth without a redesign. | Soft consideration only — group expansion beyond five properties is not confirmed (BRD §7, A4). |
| NFR-06 | **Availability during the reporting window.** Whatever supports monthly consolidation must be reliably available from property submission through management-pack finalization. | Derived from the criticality of the monthly cycle (Meeting 3); no specific uptime figure has been requested or evidenced. |
| NFR-07 | **Role-based access control.** Access must distinguish who may propose, approve, and simply view KPI definitions and consolidation data — aligned to the RACI in [`../01-discovery/stakeholder-map.md`](../01-discovery/stakeholder-map.md) (Finance: owner: IT: consulted; property GMs: consulted/viewer; Executive: informed). | Pending the RACI's own formal approval (US-03). |
| NFR-08 | **Localization.** Arabic/English language support and end-user technology comfort level (discovery questionnaire Q4.4) have not been investigated. | **Open — not yet confirmed as in scope.** Not assumed either way. |
| NFR-09 | **Vendor/solution neutrality.** No requirement in this set may presuppose a new Hotel Management System purchase; every requirement must remain satisfiable by process/governance change, reconfiguration of existing tools, or new software. | Directly mitigates the risk named in Meeting 2. |

*Performance, security architecture, and integration-specific non-functionals are deferred to [`../05-technology/`](../05-technology/), once a solution approach (process-only, tooling change, or new system) is actually chosen.*
