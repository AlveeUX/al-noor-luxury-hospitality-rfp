# Changelog

All notable changes to this case study are recorded here, newest first.

## 2026-10-05 (3)

- Drafted `05-technology/`: `system-context-and-options.md` (current-state architecture + 3 solution options with a draft recommendation), `integrations-and-data-considerations.md`, `risks-and-dependencies.md`
- **Recommendation: sequence governance before tooling, and do not pursue a full five-property PMS replacement** — grounded directly in Meeting 4's finding that the Excel consolidation layer sits outside the PMS entirely. Not yet validated with Omar or Executive Management.
- Drafted `06-rfp-and-commercial/`: `rfp-document.md` (scoped to the confirmed problem, explicitly not the original "Hotel Management System" brief, with an open build-vs-buy decision flagged up front), `vendor-response-template.md` (compliance matrix against every FR/NFR ID), `evaluation-matrix.md`, `sow-outline.md`
- Drafted `07-estimation-and-delivery/`: `work-breakdown-structure.md`, `estimation-model.md` (person-week ranges only, no currency figures — budget was never disclosed), `delivery-phases.md` (7 gated phases), `assumptions-and-change-log.md` (change-control mechanism, starts empty)
- Pushed `08-ai-workflow/` (`ai-practice-method.md`, `role-requirements-reference.md`) to GitHub for the first time — content was already accurate for phases 05–07 and needed no changes
- Removed `STATUS.md` placeholders from `05-technology/`, `06-rfp-and-commercial/`, `07-estimation-and-delivery/`
- `DECISIONS.md`: 6 new entries; `README.md`: project status table updated — all 8 stages now have content
- **All of 05/06/07 remain explicitly draft** — no technology, procurement, or estimation workshop has been held with Khalid, Nadia, or Omar. The repository's full structure is now populated end-to-end, with every open approval and tracked dependency still visible rather than quietly resolved

## 2026-10-05 (2)

- Drafted `04-ux-and-product/` in full: `personas.md` (4 personas, each traced to a confirmed discovery stakeholder), `user-journeys-and-workflows.md` (2 confirmed process maps + 3 candidate workflows), `information-architecture.md`, `screen-flows.md` (4 flows, wireframe-level detail)
- Entire phase explicitly scoped as illustrative/candidate — built around one possible supporting capability, not a committed design, since `05-technology/` has not yet decided whether a new tool, reconfigured existing tools, or process change alone delivers the `03-requirements/` functional requirements
- Property GM persona explicitly flagged as evidenced by only 2 of 5 properties, not all five
- Removed `04-ux-and-product/STATUS.md` placeholder, superseded by the real content
- `DECISIONS.md`: 2 new entries; `README.md`: project status table updated

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
