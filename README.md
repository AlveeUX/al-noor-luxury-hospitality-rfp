# Hotel Group Digital Transformation — BA Case Study

**A self-directed Business Analyst practice project** simulating end-to-end discovery, requirements, UX/product scoping, technical analysis, RFP preparation, and effort estimation for a fictional five-property luxury hotel group in the UAE.

> **Portfolio note:** This is an independent practice case study, not a real client engagement. "Al Noor Luxury Hospitality Group" is a fictional company invented for this exercise. All client statements, interviews, and decisions in this repository were authored by me as part of a structured self-practice method (role-play discovery + real, source-cited industry research). Nothing here should be read as work performed for an actual client or employer. Where the repository cites external facts (market data, vendor capabilities, regulations), sources are listed in [`02-research/sources.md`](02-research/sources.md).

---

## Why this project exists

I built this to practice the core workflow of a client-facing Business Analyst role at a digital product design agency: turning an ambiguous brief into a clear, validated, estimable scope. The project is designed against a real BA job description's responsibility areas (summarized, not reproduced, in [`08-ai-workflow/role-requirements-reference.md`](08-ai-workflow/role-requirements-reference.md)).

The exercise deliberately starts from an **incomplete client brief** (a one-paragraph RFP request for a "Hotel Management System") and works forward through discovery, research, requirement validation, UX/product scoping, technical feasibility, commercial structuring, and estimation — the same sequence a BA would run on a real RFP.

## What this demonstrates

| Skill area (from the JD) | Where it's evidenced |
|---|---|
| Research & business analysis | [`02-research/`](02-research/) — market research, competitor/vendor landscape, source register |
| Client discovery & requirement validation | [`01-discovery/`](01-discovery/) — questionnaire, interview notes, decision log |
| UX/UI & product scoping | [`04-ux-and-product/`](04-ux-and-product/) — personas, journeys, IA, screen flows |
| Technology & development handoff | [`05-technology/`](05-technology/) — integrations, architecture constraints, risks |
| Scope estimation & planning | [`07-estimation-and-delivery/`](07-estimation-and-delivery/) — WBS, estimation model, phasing |
| RFP / commercial / contract awareness | [`06-rfp-and-commercial/`](06-rfp-and-commercial/) — RFP pack, evaluation matrix, SOW outline |
| AI-assisted BA workflow | [`08-ai-workflow/`](08-ai-workflow/) — prompts, context files, verification log |

## Repository structure

```
01-discovery/            Client brief, stakeholder map, discovery questionnaire, interview notes, open questions
02-research/              Market research, vendor/competitor landscape, source register
03-requirements/          BRD, user stories, functional/non-functional requirements, traceability matrix
04-ux-and-product/        Personas, journeys, workflows, information architecture, screen flows
05-technology/            System context, integrations, data considerations, risks & dependencies
06-rfp-and-commercial/    RFP document, vendor response template, evaluation matrix, SOW outline
07-estimation-and-delivery/  WBS, estimation spreadsheet, delivery phases, assumptions/change log
08-ai-workflow/           AI practice method, reusable prompts, context files, verification log
DECISIONS.md             Key decisions and the evidence/reasoning behind them
CHANGELOG.md             What changed, when, and why
```

## Project status

| Stage | Status |
|---|---|
| 01 — Discovery | **Complete** — joint session, dedicated Finance and IT sessions, follow-up on open items. 2 dependencies tracked forward (see below), not blockers. |
| 02 — Research | Substantial — UAE market data, PMS vendor landscape, UAE/GCC regulatory considerations, all sourced |
| 03 — Requirements | Not started — next up |
| 04 — UX & Product | Not started |
| 05 — Technology | Not started |
| 06 — RFP & Commercial | Not started |
| 07 — Estimation & Delivery | Not started |
| 08 — AI Workflow | Substantial |

**Key discovery finding:** the client's starting request ("Hotel Management System") does not match the confirmed problem. Two independent stakeholders — Finance (process) and IT (technical) — converged on the same root cause from different angles: an ungoverned KPI-definition layer and a manual Excel consolidation process sitting outside the PMS, not a PMS data-availability problem. Full evidence trail in [`01-discovery/interview-notes.md`](01-discovery/interview-notes.md).

**Open dependencies carried into requirements** (not blockers, tracked with an owner): Property D's exact PMS/reporting flow, and a property-by-property inventory of government/tourism-authority reporting obligations — both owned by IT, pending direct property-team confirmation.

_Last updated: 2026-10-04_

## About the fictional client

**Al Noor Luxury Hospitality Group** — a fictional operator of five five-star hotels across individual emirates of the UAE, considering a technology solution to standardize operations and give management consolidated visibility across properties. Full brief: [`01-discovery/client-brief-v0.1.md`](01-discovery/client-brief-v0.1.md).

## Author

Absar Alvee — Business Analyst practice project, 2026.
