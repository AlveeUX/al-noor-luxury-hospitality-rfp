# Personas — Al Noor Luxury Hospitality Group

**Status: Draft.** No dedicated UX research session has been run — these personas are built directly from confirmed discovery statements (not invented demographics or behaviors), consistent with the project's traceability principle. Where something about a persona was never actually asked in discovery, it is marked **Not confirmed** rather than assumed.

**Framing note:** per [`../03-requirements/business-requirements-document.md`](../03-requirements/business-requirements-document.md) §2, whether these personas end up using a *new piece of software* or a *redesigned process with lighter supporting tooling* is still an open question for [`../05-technology/`](../05-technology/). The personas, journeys, and screens in this folder describe the people and their goals either way — they are written to hold regardless of which delivery mechanism is ultimately chosen, and the IA/screen-flow artifacts are explicitly labeled as one illustrative candidate, not a committed design.

---

## Primary persona: Nadia — Group Finance Director

| | |
|---|---|
| **Based on** | Nadia Hassan (confirmed stakeholder, Meetings 2, 3, 5) |
| **Role in the process** | Tentative accountable owner of KPI/business definitions (pending Executive approval — see US-03); owns the monthly consolidation process |
| **Goals** | A trusted, comparable, group-level view of property performance; less reconciliation back-and-forth; a faster, more predictable monthly cycle; less dependence on her own or her team's undocumented knowledge of how each property's figures are built |
| **Pain points (confirmed)** | No KPI data dictionary exists; consolidation runs through Excel with no centralized integration; no formal escalation policy for unresolved issues at the deadline; informal/memorized knowledge of property-specific calculations is a key-person risk she named explicitly |
| **Representative quote** | *"I wouldn't want to jump from that statement directly to a technology requirement. We haven't established what mechanism would be appropriate."* (Meeting 3) |
| **Tech comfort / tooling today** | Works in Excel/spreadsheets today (confirmed, Meeting 4). Broader technology comfort level was never asked (discovery questionnaire Q4.4) — **Not confirmed**, do not assume beyond spreadsheet proficiency. |
| **Frequency of use (candidate tool)** | Cycle-driven — intensive during the monthly consolidation window, lighter governance activity (definition review/approval) between cycles |

## Secondary persona: Omar — Group IT Manager

| | |
|---|---|
| **Based on** | Omar Farouk (confirmed stakeholder, Meetings 2, 4, 5) |
| **Role in the process** | Consulted (not owning) on KPI/business definitions; owns the two tracked dependencies (Property D, government/tourism reporting inventory) |
| **Goals** | Clear, documented, agreed definitions so IT isn't asked to resolve what are actually process/governance questions; an accurate, current system-landscape record he can stand behind with stated confidence levels |
| **Pain points (confirmed)** | Separates IT-confirmed facts from current-understanding-but-unverified explicitly, because internal records about Property D were inconsistent; flagged that some of the reporting flow sits with Finance and property teams, so IT alone can't answer every question directed at it |
| **Representative quote** | *"[Shared PMS across properties does] not imply standardized configuration, reporting setup, process, or user practice."* (Meeting 4) |
| **Tech comfort** | High — IT professional; not a usability risk for this persona |
| **Frequency of use (candidate tool)** | Periodic — definition-review consultation, plus active work on the two open dependencies until resolved |

## Tertiary persona: Property GM (composite of Mariam Al Mazrouei and Daniel Thomas)

| | |
|---|---|
| **Based on** | Two of five property GMs (Meeting 2 only) — **this persona is evidenced by 40% of properties.** The other three GMs have not yet been engaged; do not assume this persona represents all five properties. |
| **Role in the process** | Consulted stakeholder in the KPI-definition governance process (US-02); may submit a documented property-level variance (US-08) |
| **Goals** | Preserve legitimate, intentional operational differences between properties; be consulted with a real process, not have definitions imposed |
| **Pain points (confirmed)** | Explicitly wary of "corporate imposing definitions without understanding property impact" — supports clearer definitions only *if* there's a proper agreement process |
| **Representative quote** | *(paraphrased from Meeting 2, both GMs)* "...provided there is a proper process for agreeing them, and legitimate property-level differences are preserved rather than overridden for corporate convenience." |
| **Tech comfort / language preference** | **Not confirmed** — discovery questionnaire Q4.4 (end-user comfort level, Arabic/English preference) was never put to this stakeholder group. Any UI design decision depending on this must be validated before build, not assumed here. |
| **Frequency of use (candidate tool)** | Occasional — triggered by a consultation request or a variance submission, not a recurring daily user |

## Peripheral persona: Khalid — Group Procurement Manager

| | |
|---|---|
| **Based on** | Khalid Rahman (confirmed stakeholder, Meetings 1, 2) |
| **Role in the process** | Process owner of the overall initiative; not a day-to-day user of any candidate supporting tool |
| **Goals** | Ensure the eventual RFP targets the real, confirmed problem rather than the originally requested "Hotel Management System" label |
| **Representative quote** | Corrected the problem framing in Meeting 2: autonomy itself is not the problem — the issue is specifically where flexibility affects information that needs to be compared or governed at group level. |
| **Frequency of use (candidate tool)** | Oversight/reporting view only, if any — not scoped as an active governance participant in the stories drafted so far |

---

## Explicitly not modeled as personas (and why)

- **Front-desk / housekeeping staff** — discovery questionnaire Q4.4 raised this group, but no session has engaged them and their relevance to this specific problem (KPI governance, not daily operations) has not been established.
- **Executive Management / Group COO** — referenced as the approval authority (US-03) but has not personally attended a session; treated as an approval gate, not a persona, until they participate directly.
- **The remaining three property GMs** — see the caveat on the Property GM persona above.
