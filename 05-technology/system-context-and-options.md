# System Context & Solution Options — Al Noor Luxury Hospitality Group

**Status: Draft — BA/technology analysis, not a stakeholder-validated decision.** No dedicated technology workshop has been run with Omar Farouk or Executive Management. This is where the project's central open question — raised but deliberately left unanswered since Meeting 2 — gets a recommendation: **should this be solved by governance/process change, lightweight supporting tooling, or a new system?**

---

## 1. Current-state system context (confirmed, Meeting 4)

```
Property layer (×5):
  Property PMS (4 confirmed Opera; Property D confirmed NOT Opera, exact product pending — US-10)
        │
        ▼
  Property-level calculation & reporting (business logic lives here — this is
  where the March occupancy divergence actually happened, not in the PMS data)
        │
        ▼
  Property submission (file/report) ──────────────┐
                                                    ▼
Corporate layer:                     Excel-based consolidation (no centralized
                                      integration across the 5 PMS environments — confirmed absence, Meeting 4)
                                                    │
                                                    ▼
                                      Finance validation / reconciliation
                                                    │
                                                    ▼
                                      Consolidated management report

Separately (not integrated with the above):
  Government/tourism-authority reporting — property-by-property, mechanism
  not yet confirmed (tracked dependency, US-09)
```

**Key architectural fact driving everything below** (Omar's own synthesis, Meeting 4): even a fully standardized PMS landscape across all five properties would **not** eliminate the corporate Excel consolidation layer, because it sits entirely outside the PMS. This is why "replace the PMS" and "fix the consolidation problem" are two different projects, not one.

## 2. Solution options considered

| | Option A — Process & governance only | Option B — Lightweight governance & consolidation tool | Option C — Full Hotel Management System replacement (5 properties) |
|---|---|---|---|
| **What it is** | Formalize the KPI dictionary, escalation policy, and a single authoritative consolidation workbook as documented, versioned artifacts — no new software | A purpose-built or configured capability (the candidate scoped in [`../04-ux-and-product/`](../04-ux-and-product/)) layered on top of the existing property/PMS landscape | Replace PMS across all five properties with a single standardized system (the original brief's request) |
| **Addresses the confirmed problem?** | Yes — directly targets the governance gap (Meeting 2/3/5) | Yes — same governance fix, plus removes manual/undocumented steps (bus-factor risk, Meeting 3) | **No** — the confirmed problem lives in business logic and the Excel consolidation layer, not PMS data availability (Meeting 4) |
| **Cost/risk/disruption** | Lowest | Low-medium — scoped to the confirmed problem only | Highest — five-property migration, retraining, contract/termination exposure (discovery Q2.4, never answered) |
| **Time to value** | Fastest | Medium | Slowest |
| **Preserves property autonomy (Epic D)** | Yes, by design | Yes, if the variance mechanism (US-08) is built in | At risk — standardizing a PMS invites standardizing configuration too, which both GMs explicitly cautioned against (Meeting 2) |
| **Dependent on open items** | No | Low — can start before Property D / regulatory inventory resolve | High — Property D's unknown system and undisclosed budget/timeline (BRD §7) make this materially harder to scope at all |

## 3. Recommendation (draft, pending validation)

**Sequence Option A into Option B — do not pursue Option C on current evidence.**

Rationale:
- Governance (Option A) must exist before any tool (Option B) is built — a tool encoding an undefined KPI dictionary just automates the current ambiguity faster. This sequencing dependency is reflected in [`../07-estimation-and-delivery/delivery-phases.md`](../07-estimation-and-delivery/delivery-phases.md).
- Option C directly contradicts two standing project decisions: treating "Hotel Management System" as the client's *requested* solution rather than a confirmed need ([`../DECISIONS.md`](../DECISIONS.md)), and the explicit Meeting 2 risk against writing requirements that ask a vendor to solve a governance problem through software alone.
- This recommendation is **reversible** — if, during Option A, new evidence emerges that the problem is broader (e.g., the procurement/guest-service hypothesis from Meeting 2 gets concrete examples), the option analysis should be redone, not assumed to still hold.

**This recommendation has not been reviewed with Khalid, Nadia, or Omar.** Per [`../03-requirements/business-requirements-document.md`](../03-requirements/business-requirements-document.md) §11, it should be validated alongside the BRD, not decided unilaterally by this document.
