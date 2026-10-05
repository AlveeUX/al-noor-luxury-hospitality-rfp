# User Stories — Al Noor Luxury Hospitality Group

**Status: Draft.** BA-authored from discovery evidence (see [`business-requirements-document.md`](business-requirements-document.md) §2 for why these are deliberately solution-agnostic). Priorities below are BA-suggested for the purpose of sequencing a draft, not a stakeholder-agreed backlog order — no prioritization workshop has been run yet. Every story cites its discovery source; see [`traceability-matrix.md`](traceability-matrix.md) for the full mapping.

---

## Epic A — KPI & Business Definition Governance

### US-01: Documented KPI/business definition dictionary
**As** Group Finance Director, **I want** a version-controlled KPI/business definition dictionary, **so that** property and corporate figures are calculated on an agreed, auditable basis.

**Acceptance criteria:**
- Dictionary records, per KPI: name, definition, calculation formula/denominator rules, owner, effective date, and version history.
- Occupancy is documented first (the only KPI with a confirmed definitional dispute — Meeting 2/3). Revenue, ADR, and RevPAR are added as candidate entries, explicitly marked unconfirmed until Finance validates them.
- Accessible to Finance, IT, and property GMs.

**Source:** Meeting 2 (no dictionary exists, confirmed by both Finance and IT), Meeting 3 (definition/semantic issue category). **Priority (suggested):** High.

### US-02: Property consultation before a definition is finalized
**As** a Property GM, **I want** to be consulted before a group-wide KPI definition is finalized, **so that** legitimate property-level operating differences aren't overridden without my input.

**Acceptance criteria:**
- A documented consultation step exists in the definition governance process.
- GM sign-off or a documented objection is captured before a definition is marked "agreed."
- Consultation does not require unanimous consent, but every property's input must be recorded.

**Source:** Meeting 2 — both GMs supported clearer definitions "provided there is a proper process for agreeing them." **Priority (suggested):** High.

### US-03: Formal approval of Finance as definition owner
**As** Group Finance Director, **I want** Executive Management to formally approve Finance as accountable owner of KPI/business definitions (IT consulted, not owning), **so that** governance authority is unambiguous rather than an informal working-group agreement.

**Acceptance criteria:**
- Executive Management sign-off recorded and dated.
- [`../01-discovery/stakeholder-map.md`](../01-discovery/stakeholder-map.md) RACI updated from "tentative" to "approved."

**Source:** Meeting 2; [`../DECISIONS.md`](../DECISIONS.md) ("Pending approval" entry). **Priority (suggested):** High — blocks formal legitimacy of Epic A.

---

## Epic B — Group Consolidation & Reporting Process

### US-04: Redesigned consolidation process
**As** Group Finance Director, **I want** the monthly consolidation process to move from *receive → investigate → ask property → clarify → reconcile → (investigate again if necessary) → consolidate → report* to *receive → validate → consolidate → review → report*, **so that** reconciliation effort and reporting cycle time are reduced.

**Acceptance criteria:**
- An upfront validation step checks property-submitted figures against the current agreed KPI dictionary (US-01) before consolidation.
- The process is documented as a standard operating procedure (SOP).
- A before/after cycle-time comparison is possible once a baseline is measured (see US-06) — not claimed here, since no baseline currently exists.

**Source:** Meeting 3 (Nadia's own current vs. target process). **Priority (suggested):** High.

### US-05: Single authoritative, documented consolidation source
**As** Group Finance Director, **I want** a single authoritative consolidation source with documented formulas and data sources, **so that** the process isn't dependent on individual staff's undocumented knowledge of how each property's figures are built.

**Acceptance criteria:**
- One workbook/process is designated authoritative; intermediate spreadsheets, if retained, are documented as feeding it.
- Formulas/macros are documented, not tribal knowledge.
- Addresses the "bus-factor" risk Nadia named explicitly.

**Source:** Meeting 3 (bus-factor risk), Meeting 4 (Excel-based consolidation confirmed, no centralized integration). **Priority (suggested):** Medium-High.

### US-06: Classified, logged clarification cases
**As** Group Finance Director, **I want** each clarification case classified by type (data correction / definition clarification / reconciliation-timing) and logged, **so that** recurring issues can be measured and reduced over time instead of handled ad hoc.

**Acceptance criteria:**
- Logging captures category (or categories — a case may span more than one, per Nadia's caveat), property, and resolution time.
- Produces a measured monthly volume, replacing the current qualitative estimate ("closer to every monthly cycle").
- Categories are **not** treated as a strict partition.

**Source:** Meeting 3 (three-way framework: correctness / definition / process-timing). **Priority (suggested):** Medium.

---

## Epic C — Exception & Escalation Handling

### US-07: Documented escalation policy for unresolved deadline issues
**As** Group Finance Director, **I want** a documented, severity-based escalation/exception policy for issues unresolved at the reporting deadline, **so that** handling (proceed on best-available information / hold pending response / flag as exception) is consistent rather than purely judgment-based.

**Acceptance criteria:**
- Policy defines severity tiers and the required action for each tier.
- Approved by Finance leadership (and Executive Management if the policy requires it).
- Referenced from the SOP in US-04.

**Source:** Meeting 5 — confirmed as a genuine governance gap, not an assumption ("no formal, documented escalation or exception-handling policy" exists today). **Priority (suggested):** Medium-High — same governance family as the missing data dictionary.

---

## Epic D — Preserving Property-Level Flexibility

### US-08: Documented property-level variance mechanism
**As** a Property GM, **I want** the ability to flag where a group-wide definition doesn't fit my property's legitimate operating circumstances, **so that** standardization doesn't remove necessary local flexibility.

**Acceptance criteria:**
- A variance/exception mechanism exists within the governance process from Epic A.
- Approved variances are visible to corporate Finance, not silently applied or hidden.
- Variances are distinguished from unapproved inconsistency (the latter remains a clarification case per Epic B).

**Source:** Meeting 2 — Khalid's framing that autonomy itself isn't the problem; both GMs' caveat that legitimate differences must be preserved. **Priority (suggested):** High — without this, Epic A risks the over-standardization risk named in discovery.

---

## Epic E — Regulatory / Government Reporting (tracked dependency)

### US-09 (provisional — blocked): Government/tourism-authority reporting inventory
**As** Group IT Manager, **I want** a verified, property-by-property inventory of government/tourism-authority reporting obligations (authority, data submitted, automation level, source system, portal/interface), **so that** any future process or system change correctly accounts for these obligations.

**Acceptance criteria:**
- Inventory completed for all five properties.
- Cross-checked against [`../02-research/regulatory-considerations.md`](../02-research/regulatory-considerations.md) (the DET/DTCM-type finding).
- Marked complete only after direct property-level confirmation — not before.

**Source:** Meeting 4 (existence confirmed, mechanism not), Meeting 5 (still open), [`../02-research/regulatory-considerations.md`](../02-research/regulatory-considerations.md). **Status:** Blocked — tracked dependency, owner Omar Farouk. **Priority:** Not yet prioritized against the backlog; sequencing depends on when the dependency resolves.

### US-10 (provisional — blocked): Property D confirmation
**As** Group IT Manager, **I want** Property D's PMS and full reporting flow fully confirmed and documented, **so that** Property D can be included in group governance and consolidation processes on the same basis as the other four properties.

**Acceptance criteria:**
- PMS product name confirmed (currently known only to **not** be Opera).
- Full reporting flow documented with the same confidence level as Properties A–C.

**Source:** Meeting 4, Meeting 5 (tracked dependency). **Status:** Blocked — in progress, owner Omar Farouk.

---

*Not included as stories: procurement/guest-service metrics (explicitly out of scope — see BRD §5.2), any new-system/vendor capability (deferred to [`../05-technology/`](../05-technology/) and [`../06-rfp-and-commercial/`](../06-rfp-and-commercial/)).*
