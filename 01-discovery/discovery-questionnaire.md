# Discovery Questionnaire — Al Noor Luxury Hospitality Group

**Purpose:** Structured question set prepared ahead of client discovery meetings, built from the gaps identified in [`client-brief-v0.1.md`](client-brief-v0.1.md). Organized by theme and prioritized so the highest-leverage questions are asked first if meeting time is limited. Each question states *why it matters* — the downstream decision it unblocks — so the questions stay traceable to a purpose rather than reading as a generic checklist.

Answers go into [`interview-notes.md`](interview-notes.md), tagged as **Confirmed**, **Assumption (needs validation)**, or **Open / stakeholder dependency**.

---

## 1. Business objectives — why is this happening now?

| # | Question | Why it matters |
|---|---|---|
| 1.1 | What triggered this initiative — a specific incident, a strategic plan, a board directive, or an accumulation of operational pain points? | Separates a reactive purchase from a planned transformation; changes urgency and scope framing |
| 1.2 | What does "operational consistency" and "group-wide visibility" actually mean in practice? Can you give a concrete example of a decision leadership currently cannot make, or a report they cannot get, because of the current setup? | The brief's objective is abstract; a concrete example turns it into a testable requirement |
| 1.3 | Is this primarily an operations problem, a reporting/finance problem, a guest-experience problem, or a cost problem? | Determines which department owns success criteria and which modules matter most |
| 1.4 | Has the group tried to solve this before (process changes, a prior system, manual consolidation)? What happened? | Surfaces prior failed attempts and political/organizational risk factors |
| 1.5 | What happens if this project does not happen — what's the cost of inaction? | Tests whether this is a "nice to have" or genuinely business-critical; affects priority and budget appetite |

## 2. Current environment — what exists today?

| # | Question | Why it matters |
|---|---|---|
| 2.1 | Does each of the five hotels currently run its own PMS, or is there already a shared/group-level system? If separate, which systems (vendor/product names), and are they the same or different across properties? | **The single highest-impact unknown.** Five different legacy systems = migration + integration project. One shared system = an upgrade/consolidation project. These are different projects with different scope, risk, and cost profiles |
| 2.2 | How is "consolidated reporting" done today — manual spreadsheet consolidation, a BI tool, email summaries? Who does it and how often? | Reveals the real current-state pain and a baseline to measure improvement against |
| 2.3 | What other systems need to talk to the hotel system — accounting/ERP, channel manager, booking engine/OTAs, POS (restaurants/spa), CRM/loyalty, revenue management? | Defines the integration surface, which is usually the largest cost and risk driver in hospitality tech projects |
| 2.4 | Are there existing contracts with current vendors, and are any under active term (termination penalties, renewal dates)? | Affects timeline — a mid-contract switch has cost and legal implications |
| 2.5 | What's the IT setup — a central IT team, property-level IT, or outsourced? Who maintains current systems? | Affects implementation support model and training needs |

## 3. Scope — which properties, departments, and capabilities?

| # | Question | Why it matters |
|---|---|---|
| 3.1 | Are all five properties in scope for a single rollout, or is this a phased/pilot approach (e.g., one flagship property first)? | Materially changes delivery phasing and risk approach |
| 3.2 | Beyond rooms/front-desk, which revenue centers are in scope — F&B/restaurants, spa, events/banqueting, retail? | "Hotel Management System" in the brief could mean PMS-only or a full operations suite; this question forces a scope boundary |
| 3.3 | Is a guest-facing component in scope (booking engine, guest app, digital check-in/key), or is this purely a back-of-house/operations system? | The brief doesn't mention guest experience at all — worth explicitly confirming it's out of scope rather than assuming |
| 3.4 | Should the solution support only UAE properties, or is there a possibility of future expansion outside the UAE that the architecture should anticipate? | Affects localization requirements and long-term architecture decisions |

## 4. Stakeholders — who uses it, approves it, and judges vendors?

| # | Question | Why it matters |
|---|---|---|
| 4.1 | Beyond Procurement, which departments have a stake — Operations, Finance, IT, Revenue Management, individual General Managers at each property, Executive/Ownership? | Identifies whose requirements must be gathered and whose sign-off is needed |
| 4.2 | Who is the final decision-maker, and who sits on the evaluation committee? | Shapes how the RFP evaluation criteria should be weighted |
| 4.3 | Will property-level GMs have autonomy to request local customizations, or is the mandate strict standardization across all five hotels? | A recurring tension in multi-property rollouts; directly affects configurability requirements |
| 4.4 | Who are the actual day-to-day end users (front desk agents, housekeeping staff, revenue managers, finance) and what's their current comfort level with technology / language preference (Arabic/English)? | Drives UX, training, and localization requirements |

## 5. Constraints — budget, timeline, regulatory, risk

| # | Question | Why it matters |
|---|---|---|
| 5.1 | Is there an approved budget range or a budget approval process still pending? | Without this, any estimation work is speculative and should be labeled as such |
| 5.2 | Is there a target go-live date tied to a business event (e.g., a peak season, a new property opening, a board deadline)? | Hospitality has hard seasonal constraints — implementing a PMS during peak season is a major operational risk |
| 5.3 | Are there UAE-specific regulatory requirements the system must meet (e.g., tourism-authority reporting integrations per emirate, data residency rules, VAT/e-invoicing compliance)? | GCC hospitality systems often require government integrations (e.g., police/immigration guest reporting, Dubai Tourism / DET systems) — this must be validated, not assumed, and is a likely vendor-differentiator |
| 5.4 | Cloud-hosted vs. on-premise preference, or no preference? | Major architecture and vendor-shortlist decision |
| 5.5 | What is procurement's preferred engagement model — single vendor for everything, or best-of-breed with the group managing integration? | Changes the entire structure of the RFP and evaluation criteria |

## 6. Success criteria — how do we know it worked?

| # | Question | Why it matters |
|---|---|---|
| 6.1 | What specific, measurable outcomes would make this project a success six months after go-live? | Converts a vague objective into acceptance criteria |
| 6.2 | Will success be judged by operational metrics (check-in time, report turnaround), financial metrics (cost savings, RevPAR visibility), or guest satisfaction metrics? | Determines which KPIs belong in the SOW/acceptance criteria |
| 6.3 | Who signs off that the implementation is "done" at each property — a single group sign-off, or per-property acceptance? | Affects the acceptance and change-control process in the eventual SOW |

---

## Prioritization for a time-limited first meeting

If only 30 minutes are available, the highest-leverage questions are **1.2, 1.3, 2.1, 2.3, 3.1, 3.2, 4.1, 5.1, 5.3** — these alone are enough to tell whether this is a PMS replacement project, a full operations-suite project, or something else entirely, and whether it's even fundable.

---

*Next: [interview-notes.md](interview-notes.md) records what was actually confirmed against this questionnaire.*
