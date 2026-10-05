# Changelog

All notable changes to this case study are recorded here, newest first.

## 2026-10-05

- Drafted `03-requirements/` in full: `business-requirements-document.md`, `user-stories.md` (10 stories across 5 epics), `functional-requirements.md` (12 requirements), `non-functional-requirements.md` (9 requirements), `traceability-matrix.md`
- Every requirement traced back to a specific discovery meeting or research finding — see `traceability-matrix.md` for the full mapping, including a table of items deliberately **not** carried into requirements (and why)
- Requirements written solution-agnostic by design, per the Meeting 2 risk about presupposing a new Hotel Management System purchase
- The two tracked dependencies from discovery (Property D, government/tourism reporting inventory) carried forward as explicit "Pending" user stories (US-09, US-10), not silently dropped
- Removed `03-requirements/STATUS.md` placeholder, superseded by the real content
- `DECISIONS.md`: 4 new entries; `README.md`: project status table updated, 03 — Requirements now "Draft — pending stakeholder validation"
- **All content in this phase is explicitly marked draft** — no stakeholder validation session has been run on it yet; recommended next step before moving to `04-ux-and-product/` or `05-technology/` is circulating this BRD and user stories with Khalid, Nadia, and Omar

## 2026-10-04 (3)

- Follow-up round on the three items left open after the Finance and IT sessions (`01-discovery/interview-notes.md`, Meeting 5)
- Deadline-handling question fully resolved: no formal escalation policy exists today — logged as a candidate governance/process requirement, same family as the missing KPI data dictionary
- Property D and the government/tourism regulatory inventory remain genuinely open (both require IT to engage property teams directly) — converted from open-ended questions into tracked dependencies with a named owner, rather than continuing to re-ask
- `DECISIONS.md`: 3 new entries
- **Discovery phase judged sufficient to begin requirements drafting** — two dependencies carried forward explicitly rather than treated as blockers

## 2026-10-04 (2)

- Conducted a joint discovery session (simulated) with Procurement, Finance, IT, and two property GMs
- `01-discovery/interview-notes.md`: replaced the earlier draft (pre-written, unvalidated answers) with the real session record — confirmed statements, unverified items, open questions, decisions, risks, and a provisional problem statement
- `01-discovery/stakeholder-map.md`: updated with named, confirmed participants (Khalid Rahman, Nadia Hassan, Omar Farouk, Mariam Al Mazrouei, Daniel Thomas); RACI partially filled for KPI/definition governance based on real evidence
- `01-discovery/joint-session-questionnaire.md`: added (v2, revised per client feedback on v1 — trimmed scope, neutral IT phrasing, conditional evidence handling, explicit session structure)
- `DECISIONS.md`: 5 new entries, including discarding the superseded draft and the client's correction on how the problem should be framed
- Key finding: the March occupancy discrepancy traced to a **definitional** difference (room-availability denominator), not a data error — shifted the working hypothesis from "broken reporting" toward "ungoverned KPI definitions across properties"
- Next: dedicated Finance session (historical case volume) and IT session (system landscape, data flow) — not yet scheduled

## 2026-10-04 (1)

- Initial repository scaffold created (8-stage folder structure, README, DECISIONS.md, CHANGELOG.md)
- `01-discovery/`: client brief v0.1 captured verbatim, known-vs-assumed facts table built, discovery questionnaire drafted (6 categories, 24 prioritized questions), stakeholder map drafted (confirmed + inferred/unconfirmed stakeholders), interview notes template created
- Project status: Discovery in progress; no client interview conducted yet
