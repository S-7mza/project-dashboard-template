# Dashboard Project Process Audit – PMI / PMBOK Reference

Score: **8 / 10**

## Scoring barème

- **0–3:** Major parts of PMBOK are missing or ad‑hoc.
- **4–6:** Most knowledge areas are documented but unevenly applied.
- **7–8:** All key areas present and generally used; some integration gaps.
- **9–10:** Fully integrated, consistently applied, and continuously improved.

This **8/10** reflects: very strong coverage of scope, schedule, stakeholders, and quality, with partial coverage of cost and change control, and improvement potential in integrated monitoring.

## Scope of this audit

Reference: PMI PMBOK (process groups + knowledge areas) applied to your dashboard playbook (workshops, agile folder, docs, templates).

## Strengths (what is well covered)

- **Integration & Scope (8/10):** Clear artefacts for project brief, charter and plan (`docs/PROJECT_BRIEF.md`, `docs/PROJECT_CHARTER (C).md`, `docs/PROJECT_PLAN (C).md`), and a workshop-based roadmap in `templates/WORKSHOP_DETAILED_SESSION_PLAN.csv`.
- **Schedule & Workshops (9/10):** Detailed workshop plan, pre-work, agendas (`workshops/*`), and comms (`communication/*`) provide a strong, structured schedule baseline.
- **Stakeholder & Communications (9/10):** Dedicated communication plans (`docs/COMMUNICATION_PLAN.md`, `communication/*`) and templates for minutes, decisions, and actions (`templates/MEETING_MINUTES.md`, `templates/DECISION_LOG.md`, `templates/ACTION_LOG.csv`).
- **Quality & UAT (8/10):** Specific artefacts for QA and UAT (`docs/QUALITY_MANAGEMENT_PLAN.md`, `docs/TEST_UAT_PLAN (C).md`, `agile/DEFINITION_OF_DONE.md`, `agile/DOD_CASES.md`).
- **Risk & Issues (7/10):** Templates for risk and issue registers (`templates/RISK_REGISTER.md`, `templates/ISSUE_LOG.md`) and a gating checklist (`02_GATING_CHECKLIST (C).md`).

## Gaps / improvement opportunities

- **Monitoring & Controlling integration (score limiter):**
  - You have good individual artefacts, but less explicit guidance on *how often* they are reviewed and *who* consolidates status across scope/schedule/cost/risk.
  - Status reporting cadence and dashboards for project health could be clearer.

- **Cost management (lightly covered):**
  - Cost/effort is implied (workshops, capacity planning, sprints) but there is no dedicated cost management or budgeting artefact.

- **Formal change control:**
  - There is `templates/CHANGE_REQUEST.md`, but the workflow (who approves, how changes affect scope/time/cost baselines) is not fully spelled out.

## Suggested actions to reach 9–10/10

1. **Add a simple PMI-style status report template** (integrated view of scope, schedule, risk, issues, benefits) and reference it in the cadence (e.g., weekly).
2. **Define a lightweight change control process:** link `templates/CHANGE_REQUEST.md` to the gating checklist and specify approval roles in `docs/CONFIGURATION_MANAGEMENT.md`.
3. **Clarify cost/effort management:** extend `agile/CAPACITY_PLANNING.md` or `docs/PROJECT_PLAN (C).md` with a short section on budget and tracking assumptions.

## Concrete path to 10 / 10

To reach **10/10** on PMI alignment for your dashboard process:

1. **Institutionalize the status reporting cycle**
  - Make the new PMI-style status report mandatory at a defined cadence (e.g., weekly) and tie it to decision forums.
  - Ensure each project logs these reports centrally (e.g., in a folder or tracker) so governance can see trends over time.

2. **Operationalize change control**
  - Define a simple RACI for change approval in `docs/CONFIGURATION_MANAGEMENT.md`.
  - Require a signed `CHANGE_REQUEST.md` for any scope, schedule, or cost impact beyond a small threshold.

3. **Add lightweight cost/effort planning and tracking**
  - Extend `docs/PROJECT_PLAN (C).md` with a section for estimated effort/budget and a simple tracking table.
  - Link this with `agile/CAPACITY_PLANNING.md` so sprint capacity and workshop effort align with the plan.

4. **Close the loop with lessons learned**
  - After each project, review variances in scope/schedule/cost and document corrective actions in `docs/BEST_PRACTICES.md`.
  - Periodically update templates (charter, plan, gating checklist) based on these lessons.

---

**Overall PMI alignment:** strong, practical coverage for a dashboard project context, with minor gaps mainly around cost and integrated monitoring.
