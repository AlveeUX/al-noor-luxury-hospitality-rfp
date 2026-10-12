# Scope of Work

## Platforms

Web application, desktop-first (Finance's primary workflow is desk-based, cycle-driven work). Responsive behavior for tablet access is included; no native mobile app is scoped — nothing in the RFP or its supporting discovery evidence indicates property GMs or Finance need mobile access to this workflow, and we'd rather confirm that need than build for it speculatively.

## User roles

| Role | Access level | Primary use |
|---|---|---|
| Group Finance | Owner — propose/approve definitions, run consolidation, manage escalations | Daily during the monthly cycle; periodic governance activity between cycles |
| Group IT | Consulted — read access to definitions and system-landscape notes | Periodic, plus active work on the two open dependencies until resolved |
| Property GM | Consulted/viewer — respond to consultation requests, submit variance requests, view own-property data | Occasional, triggered by a consultation or variance submission |
| Executive Management | Informed — approval gate for governance-level changes while Finance's ownership role is pending | Infrequent, approval-only |

## Key user flows included in this scope

1. **Propose and approve a KPI definition change** — draft, mandatory property consultation, Finance review, conditional executive approval, publish.
2. **Monthly validation and consolidation** — intake, pre-consolidation validation against the dictionary, consolidated draft, review and publish.
3. **Log and categorize a clarification case** — open a case, apply one or more category tags, track to resolution.
4. **Escalate an unresolved issue** — deadline-driven alert, severity assessment, documented action (proceed / hold / flag), permanent log entry.
5. **Submit and review a property-level variance** — GM-initiated, jointly reviewed with Finance, recorded and visible, distinct from an unapproved inconsistency.

## In scope

- A version-controlled KPI/business-definition dictionary (occupancy at launch; revenue, ADR, RevPAR added only once each is independently confirmed as affected)
- Pre-consolidation validation against the agreed dictionary
- A single authoritative, auditable consolidation workspace
- Clarification-case logging, categorization, and volume/frequency reporting
- A documented, severity-based escalation workflow
- A property-variance register, distinct from the case log
- Role-based access aligned to the governance RACI
- A full, timestamped, attributable change history across definitions and consolidation figures

## Explicitly out of scope for this engagement

- Replacement of any property's PMS, reservations, or front-desk system
- Guest-facing functionality: booking engine, channel manager, POS/F&B, guest CRM
- Government/tourism-authority reporting integration — scoped separately once Al Noor's property-by-property inventory is complete
- The fifth property's onboarding — scoped separately once its PMS and reporting flow are confirmed
- Native mobile apps
- Any procurement or guest-service metrics — not yet evidenced as part of this problem per the RFP itself

## What success looks like

We'd confirm formal acceptance criteria during discovery (the RFP itself notes these aren't finalized yet), but based on the objectives stated in the RFP, we're designing toward: less back-and-forth during consolidation, a predictable and shorter monthly cycle, a documented explanation whenever a property legitimately differs from group basis, and reduced dependence on any one person's memorized knowledge of how a property's figures are built.
