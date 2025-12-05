# Dashboard Project Process Audit – Agile / Scrum Reference

Score: **8 / 10**

## Scoring barème

- **0–3:** Agile terms used but ceremonies/artifacts are mostly absent or ad‑hoc.
- **4–6:** Core Scrum events and artifacts exist but are inconsistently applied or poorly integrated.
- **7–8:** Scrum events, artifacts, and roles are largely in place and used; some gaps in product strategy, flow, or technical excellence.
- **9–10:** Scrum is practiced end‑to‑end with strong product ownership, flow metrics, quality, and continuous improvement.

The **8/10** reflects: strong ceremonies, artifacts, and DoD, with improvement potential in product ownership guidance, flow metrics, and technical debt management.

## Scope of this audit

Reference: Agile/Scrum practices (roles, events, artifacts, flow) as implemented in your dashboard delivery playbook.

## Strengths

- **Events & ceremonies (8/10):** Dedicated guidance for sprint planning, daily standup, review, and retrospective (`agile/SPRINT_PLANNING.md`, `agile/DAILY_STANDUP.md`, `agile/SPRINT_REVIEW.md`, `agile/RETROSPECTIVE.md`).
- **Artifacts (8/10):** User story and acceptance criteria templates, sprint backlog, burndown and velocity trackers (`agile/USER_STORY_TEMPLATE.md`, `templates/ACCEPTANCE_CRITERIA.md`, `agile/SPRINT_BACKLOG_TEMPLATE.csv`, `agile/BURNDOWN_TEMPLATE.csv`, `agile/VELOCITY_TRACKER.csv`).
- **Definition of Done (9/10):** Strong focus on DoD and examples (`agile/DEFINITION_OF_DONE.md`, `agile/DOD_CASES.md`).
- **Integration with governance (7/10):** Agile delivery is framed within a PMI/governance context, which is valuable for real organizations.

## Gaps / improvement opportunities

- **Product ownership & backlog strategy:**
  - Responsibilities of Product Owner, how to prioritize work against business value, and how to manage the dashboard backlog over time could be more explicit.

- **Flow metrics and WIP:**
  - You have basic metrics (velocity, burndown) but not explicit guidelines on monitoring flow (cycle time, WIP limits) for dashboard work.

- **Technical debt & refactoring:**
  - There is limited guidance on tracking and managing technical debt for dashboards (e.g., data model refactors, ETL cleanup, visualization refactoring).

## Suggested actions to reach 9–10/10

1. **Extend Agile guidance for Product Owners:** add a short section in `agile/SPRINT_PLANNING.md` or a new `agile/PRODUCT_OWNER_GUIDE.md` on backlog ordering, KPI impact, and stakeholder alignment.
2. **Add a simple flow-metrics recommendation:** suggest tracking at least cycle time per story and a basic WIP limit, even if informally.
3. **Introduce a "Technical Debt" log template:** or add a section in `templates/ISSUE_LOG.md` dedicated to tech debt items.

## Concrete path to 10 / 10

To evolve from **8/10** to **10/10** Agile/Scrum alignment:

1. **Codify Product Owner practices**
  - Add a short `agile/PRODUCT_OWNER_GUIDE.md` explaining how to prioritize backlog items by business value, risk, and learning for dashboards.
  - Clarify how KPIs and benefits from `deliverables/KPI_SPEC (C).md` feed into backlog refinement.

2. **Introduce basic flow management**
  - Recommend simple WIP limits (e.g., max in‑progress stories) in your agile guidance.
  - Add an optional column in existing trackers (e.g., `agile/SPRINT_BACKLOG_TEMPLATE.csv`) to measure cycle time per story.

3. **Manage technical debt explicitly**
  - Add a dedicated "Technical Debt" section to `templates/ISSUE_LOG.md` or a separate tech debt log.
  - Encourage teams to reserve a small portion of sprint capacity for debt items (e.g., 10–20%).

4. **Strengthen continuous improvement**
  - In `agile/RETROSPECTIVE.md`, add a step to check whether actions from the previous retro were completed.
  - Periodically update `docs/BEST_PRACTICES.md` with recurring retro themes to turn local learnings into global standards.

---

**Overall Agile/Scrum alignment:** strong operational guidance for ceremonies and artefacts, with minor gaps around product strategy and flow optimization.
