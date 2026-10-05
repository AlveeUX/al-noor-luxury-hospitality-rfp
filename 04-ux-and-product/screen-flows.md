# Screen Flows — Al Noor Luxury Hospitality Group

**Status: Draft — illustrative candidate, not a committed design.** Described at a wireframe level (purpose, key elements, primary actions) rather than as visual mockups, consistent with this repository's markdown-only format so far. Each flow implements one workflow from [`user-journeys-and-workflows.md`](user-journeys-and-workflows.md) within the candidate IA in [`information-architecture.md`](information-architecture.md). No usability testing has been conducted — these are BA/product-drafted screens pending review, same status as the rest of this phase.

---

## Flow 1 — Propose & Approve a KPI Definition Change

*Implements Workflow C. Primary actor: Finance (Nadia persona). Secondary: Property GM, Executive.*

| Screen | Purpose | Key elements | Primary action(s) |
|---|---|---|---|
| 1. Dictionary List | Browse existing KPI definitions | Table: KPI name, current version, owner, last updated | "Propose new definition" / "Edit existing" |
| 2. Definition Form | Draft a proposed definition | Fields: KPI name, formula/denominator rules, rationale, affected properties | Save draft → Send for consultation |
| 3. Property Consultation Panel | Collect GM input | Per-property status (Not reviewed / Objected / Approved), comment thread | GM submits objection or approval |
| 4. Review & Approve | Finance finalizes after consultation | Summary of GM responses, side-by-side old vs. new definition | Approve → Publish, or Revise → back to Screen 2 |
| 5. Executive Approval (conditional) | Only while Finance's ownership role remains unapproved (US-03), or for a flagged ownership-level change | Definition summary, consultation summary | Approve / Reject |
| 6. Published Confirmation | Confirms the definition is live | Version number, effective date, notified stakeholders list | Done / View in Dictionary |

**Open question carried from the workflow doc:** which changes require step 5 versus skipping straight from Screen 4 to 6 is not yet defined — flagged, not assumed.

---

## Flow 2 — Monthly Validation & Consolidation

*Implements Workflows A→B. Primary actor: Finance.*

| Screen | Purpose | Key elements | Primary action(s) |
|---|---|---|---|
| 1. Submission Intake | Shows what's been received from each property | Per-property status: Received / Pending / Late | Mark received / Chase pending |
| 2. Validation Results | Surfaces mismatches against the current KPI dictionary *before* consolidation | Flagged figures, which definition rule triggered the flag, severity | Accept figure / Request clarification (→ Flow 3) |
| 3. Consolidation Draft | Assembles the validated figures into the group view | Property-by-property and group-rollup views, audit trail of any manual adjustment | Proceed to review |
| 4. Review & Publish | Finance's final check before the management pack is produced | Side-by-side vs. prior cycle, open cases still unresolved (linked to Flow 4 if any remain near deadline) | Publish management pack |

---

## Flow 3 — Log & Categorize a Clarification Case

*Implements Epic B (US-06). Primary actor: Finance.*

| Screen | Purpose | Key elements | Primary action(s) |
|---|---|---|---|
| 1. New Case Form | Open a case against a flagged figure | Property, KPI, description, linked validation flag (if from Flow 2) | Save |
| 2. Categorize | Tag the case — not a strict partition (Meeting 3 caveat) | Multi-select: Data correction / Definition clarification / Reconciliation-timing | Apply tags (more than one allowed) |
| 3. Case Detail | Track resolution | Status, resolution time, notes, whether it needed escalation (→ Flow 4) | Resolve / Escalate |

---

## Flow 4 — Escalate an Unresolved Issue

*Implements Workflow D (US-07). Primary actor: Finance.*

| Screen | Purpose | Key elements | Primary action(s) |
|---|---|---|---|
| 1. Deadline Dashboard Alert | Surfaces cases still open as the deadline approaches | List of at-risk cases, days to deadline | Open case → Screen 2 |
| 2. Severity Assessment | Finance judges material impact *(criteria not yet defined — see Workflow D)* | Case detail, impact notes | Choose action: Proceed / Hold / Flag |
| 3. Action Confirmation | Confirms the chosen path and records rationale | Selected action, required rationale field | Confirm |
| 4. Escalation Log Entry | Permanent record for audit (FR-09) | Case, action taken, rationale, who decided, timestamp | Done |

---

*Not designed: any guest-facing, booking, reservations, housekeeping, or billing screens — none were confirmed as in-scope (see [`../03-requirements/business-requirements-document.md`](../03-requirements/business-requirements-document.md) §5.2). Visual design, component styling, and responsive behavior are out of scope for this phase and would follow a design-system decision, not precede it.*
