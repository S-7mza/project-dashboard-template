Project Charter — [PROJECT_NAME]

Project Sponsor: [SPONSOR]
Project Manager: [PM]
Start Date: [START_DATE]
Target Delivery Date: [TARGET_DATE]

1. Purpose and Background
- Brief background: why the dashboard is initiated, business context.
- Purpose: what decisions the dashboard will enable and primary users.

2. Objectives / Success Criteria
- Objective 1: e.g., Provide executive-level view of X by Y date.
- Objective 2: Reduce manual reporting time by Z%.
- Success criteria: List measurable acceptance criteria (accuracy, freshness, performance thresholds).

3. Scope
- In-scope: KPIs, data sources, views, initial user groups.
- Out-of-scope: items not included in this release (deep exploratory analytics, ad-hoc ETL for legacy reports).

4. Deliverables
- `deliverables/KPI_SPEC.md` completed for all agreed KPIs.
- `deliverables/DATA_INVENTORY.md` completed.
- Dashboard views (list) with wireframes and signed-off visuals.
- Deployment runbook and training materials.

5. Milestones (high-level)
- Kickoff: [date]
- Complete Data Discovery: [date]
- Model & ETL designs agreed: [date]
- Dashboard initial prototype: [date]
- UAT complete: [date]
- Deployment & Handoff: [date]

6. Budget & Resources
- Estimated budget: [amount]
- Core team: PM, BI lead, BI devs, data engineer, QA, ops
- External vendors: [if any]

7. Roles & Responsibilities
- Sponsor: Approve scope and budget.
- PM: Manage schedule, risks, and communications.
- BI Lead: Technical ownership of visual and KPI definitions.
- Data Engineer: Data sourcing and ETL responsibilities.
- Product Owner: Prioritize requirements and accept UAT.

8. Constraints & Assumptions
- Data access will be provided within X days of kickoff.
- Sensitive data restrictions apply; masking may be required.
- Tooling and infra will support required concurrency and retention.

9. Major Risks & Mitigation
- Risk: Key data owner unavailable — Mitigation: identify alternate contact & escalate to sponsor.
- Risk: Data quality issues — Mitigation: early profiling and agreed quality thresholds.

10. Approval
- Sponsor: [name / signature / date]
- PM: [name / signature / date]

Notes
- Attach `docs/PROJECT_BRIEF.md`, `deliverables/DATA_INVENTORY.md`, `deliverables/KPI_SPEC.md` and `templates/RACI.md` for reference.