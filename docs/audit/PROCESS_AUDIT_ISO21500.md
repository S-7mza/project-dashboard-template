# Dashboard Project Process Audit – ISO 21500 / 21502 Reference

Score: **7 / 10**

## Scoring barème

- **0–3:** Processes largely undocumented; governance and principles unclear.
- **4–6:** Core processes exist but principles, roles, and alignment to organization are partial.
- **7–8:** Processes and roles are clear; most ISO expectations met with some gaps in principles and continual improvement.
- **9–10:** Processes, principles, governance, and continual improvement fully defined and practiced.

The **7/10** reflects: good structure and governance, with ISO principles and continual improvement only partially expressed and organization-level linkage not fully explicit.

## Scope of this audit

Reference: ISO project management guidance (principles, processes, governance) mapped to your dashboard playbook.

## Strengths

- **Context and objectives (8/10):** Project brief, charter, and benefits documentation (`docs/PROJECT_BRIEF.md`, `docs/PROJECT_CHARTER (C).md`, `docs/BENEFITS_REALIZATION.md`) describe purpose, outcomes, and constraints.
- **Governance & roles (7/10):** Team and stakeholder artefacts (`docs/TEAM_CHARTER.md`, `docs/STAKEHOLDER_ENGAGEMENT_PLAN.md`, `templates/RACI.md`) define roles and engagement.
- **Planning & resources (7/10):** Workshop roadmap, agile capacity planning, and environment inventory (`templates/WORKSHOP_DETAILED_SESSION_PLAN.csv`, `agile/CAPACITY_PLANNING.md`, `docs/ENVIRONMENT_INVENTORY.md`).
- **Risk and opportunity management (7/10):** Risk register and gating checklist are aligned with ISO expectations for proactive risk handling.
- **Quality & change (7/10):** Quality management plan, UAT plan, and change request template support controlled delivery.

## Gaps / improvement opportunities

- **Principles not made explicit (score limiter):**
  - ISO emphasizes explicit principles (e.g., responsibility, complexity, adaptability). Your playbook reflects them implicitly but does not name or explain them.

- **Organization-level alignment:**
  - The link between this dashboard process and higher-level portfolio or strategy processes is not fully articulated.

- **Lessons learned & continual improvement:**
  - You have retro and benefits tracking artefacts, but there is no explicit loop to update standards (`docs/BEST_PRACTICES.md`, templates) based on completed projects.

## Suggested actions to reach 8–9/10

1. **Add a short "ISO-style principles" section** in `docs/BEST_PRACTICES.md` explaining key principles your process follows (responsibility, transparency, stakeholder engagement, etc.).
2. **Clarify portfolio linkage:** in `docs/PROJECT_BRIEF.md` or a new `PORTFOLIO_LINK.md`, describe how dashboard projects connect to organizational strategy and portfolio selection.
3. **Define an improvement loop:** specify that after each project, outputs from retrospectives and benefits realization are reviewed and used to update templates and best practices.

## Concrete path to 10 / 10

To move from **7/10** toward **10/10** ISO-style alignment:

1. **Formalize ISO-aligned principles**
  - In `docs/BEST_PRACTICES.md`, add a short section mapping your process explicitly to ISO-style principles (responsibility, stakeholder engagement, adaptability, risk-based thinking).
  - Reference those principles in key artefacts (e.g., charter, quality plan) so they are visible to practitioners.

2. **Clarify organization and portfolio linkage**
  - Create a short note or section (e.g., `docs/PROJECT_BRIEF.md` or a new `docs/PORTFOLIO_LINK.md`) describing how dashboard projects are initiated, prioritized, and governed at portfolio level.
  - Specify which governance body approves starting and closing a dashboard project.

3. **Institutionalize lessons learned and standard updates**
  - Define a simple procedure: after each project, review retrospectives and benefits results and capture at least 2–3 improvements into `docs/BEST_PRACTICES.md`.
  - Schedule periodic (e.g., quarterly) reviews of templates based on accumulated lessons.

4. **Evidence and records**
  - Keep a minimal register (even a table in a markdown file) with links to completed charters, plans, risks, and benefits documents for each project to demonstrate consistent application of the process.

---

**Overall ISO-style alignment:** good structure and governance, with room to make principles and improvement cycles more explicit.
