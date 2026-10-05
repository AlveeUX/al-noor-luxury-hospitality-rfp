# Technology Risks & Dependencies — Al Noor Luxury Hospitality Group

**Status: Draft.**

## Risks

| # | Risk | Evidence / reasoning | Mitigation (candidate) |
|---|---|---|---|
| T1 | Building tooling before the KPI dictionary is agreed encodes current ambiguity rather than fixing it | Governance-before-tooling sequencing argument, [`system-context-and-options.md`](system-context-and-options.md) §3 | Gate any tooling build behind US-01/US-03 completion (see [`../07-estimation-and-delivery/delivery-phases.md`](../07-estimation-and-delivery/delivery-phases.md)) |
| T2 | Property D's unknown system may invalidate assumptions made about a uniform intake process | Meeting 4/5 — tracked dependency, still unconfirmed | Do not design Property D-specific integration until US-10 resolves; treat as a late-adding property, not a blocker to starting elsewhere |
| T3 | Government/tourism-reporting mechanism is unconfirmed per property | Meeting 4/5 — Omar explicit that this is "not yet a confirmed integration requirement" | Do not build against assumed authority/portal specifics; wait for US-09 inventory |
| T4 | No confirmed budget or IT resourcing for building or buying anything | Budget undisclosed (BRD §7, A2); no technology workshop held with Omar | Any estimate in [`../07-estimation-and-delivery/`](../07-estimation-and-delivery/) is explicitly indicative, not funded |
| T5 | Change-management/adoption risk from property GMs | Both GMs explicitly wary of corporate-imposed complexity (Meeting 2) | Variance mechanism (US-08) and mandatory consultation (US-02) built in from the start, not added later |
| T6 | Parallel-run risk if any part of the Excel process is formalized or replaced | Current process is the operational baseline (Meeting 3/4) — any change risks disrupting a working (if inefficient) monthly cycle | Phase 1 pilot on occupancy only (the single confirmed KPI-level finding) before expanding — see delivery phasing |
| T7 | Scope creep if the procurement/guest-service hypothesis (Meeting 2) is later confirmed | Both GMs raised it as a possibility, explicitly not yet evidenced | Treat as a separate future discovery exercise, not folded into this technology scope — consistent with standing decision not to expand scope on a hypothesis |

## Dependencies

| Dependency | Owner | Status | Blocks |
|---|---|---|---|
| Executive approval of Finance as KPI/definition owner (US-03) | Executive Management | Pending | Any tooling build (T1) |
| Property D — exact PMS and reporting flow (US-10) | Omar Farouk (IT) | In progress | Property D-specific integration design |
| Government/tourism reporting inventory (US-09) | Omar Farouk (IT) | Not yet started | Regulatory reporting integration design |
| Stakeholder validation of this technology recommendation | BA (this phase) | Not yet done | Proceeding past a draft recommendation into committed architecture |
| Budget and resourcing confirmation | Not yet owned by anyone — no session has addressed this | Not started | Any real (non-indicative) estimate |
