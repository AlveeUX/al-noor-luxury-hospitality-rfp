# AI-Assisted BA Workflow — Method Notes

This project is deliberately built *with* AI assistance (not despite it), because using AI well — with verification, not blind trust — is itself one of the target role's requirements. This file documents how AI was used at each stage so the method is transparent and auditable.

## Principles followed

1. **AI accelerates, judgment remains mine.** Every requirement, decision, and number that ends up in a deliverable is reviewed and either confirmed or corrected before use.
2. **Separate discovery from solution design.** The AI (or I, playing the client) was instructed not to reveal every requirement upfront — mirroring real discovery, where stakeholders answer what's asked and nothing more.
3. **Distinguish verified facts from assumptions.** Market/vendor research is sourced (see [`../02-research/sources.md`](../02-research/sources.md)); anything about the fictional client that can't be "verified" is explicitly labeled an assumption, never presented as fact.
4. **No estimation without enough information.** Where a critical input is missing, the gap is recorded rather than papered over with an invented number.

## How AI was used, by stage

| Stage | AI use | Human validation step |
|---|---|---|
| Discovery | Drafting a structured, prioritized question set from an incomplete brief | Reviewed each question for leading phrasing / premature assumptions before use |
| Research | Searching and synthesizing real market/vendor information (UAE hospitality market, PMS vendor landscape) | Cross-checked claims against multiple sources; anything unverifiable flagged, not included as fact |
| Requirements | Structuring raw discovery answers into functional/non-functional requirements and a traceability matrix | Checked each requirement traces back to a discovery answer or a sourced research finding |
| UX/Product | Drafting personas, journeys, and screen flows from confirmed requirements | Checked flows against the confirmed scope boundary, not the full "may include" list from the brief |
| Technology | Identifying likely integration points and risks for a multi-property hospitality operation | Validated against sourced vendor/integration documentation where available |
| Estimation | Structuring a WBS and estimation model | Treated every estimate as provisional until underlying scope/requirements were confirmed |

## Reusable prompting approach

The practice method used for client role-play and document drafting follows this structure:
- State the fictional client's known facts and explicitly mark what is *not yet known*.
- Instruct the AI (or myself, in the client role) to withhold information not directly asked for.
- Require every drafted deliverable to separate confirmed facts, assumptions, and open questions.
- After each stage, review AI output against the original brief and prior decisions before accepting it into the repository.

See [`role-requirements-reference.md`](role-requirements-reference.md) for how this maps to the target role's requirements.
