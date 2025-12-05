Pre-work Checklists for Workshops

Use these checklists to ensure each workshop is efficient and productive. Share the relevant checklist with attendees at least 3 working days before the session (sooner for technical data requests).

1) Kickoff — Pre-work
- Confirm attendees and their roles in `docs/PROJECT_BRIEF.md`.
- Provide 1-page project summary (objective, timeline, success criteria).
- Ask sponsor to prepare desired outcomes and constraints.
- PM to prepare proposed milestones and an initial RACI.
- Logistics: meeting link, recording, shared whiteboard, expected duration.

2) Technical Data Discovery (deep) — Pre-work
- Request data owners to provide:
  - Connection details (host, db, schema), contact person, and runbook for access.
  - Small sample extract (CSV or SQL `LIMIT 1000`) for each source.
  - Example queries, existing docs, and data dictionaries.
  - Row-counts for key tables and refresh frequency.
- Prepare list of sensitive fields and compliance considerations.
- BI/ETL to prepare initial tooling list (SQL client, transformation tool).
- Attach: `deliverables/DATA_INVENTORY.md`, sample SQL templates (see `templates`).

3) Data Modeling / Semantic Layer — Pre-work
- Provide outputs from Data Discovery: schemas, sample extracts, keys and cardinalities.
- Stakeholders to confirm canonical definitions for core entities (e.g., customer, account).
- BI to draft proposed dimension tables and grain definitions.
- Attach: `deliverables/KPI_SPEC.md` (draft) and `deliverables/DATA_INVENTORY.md`.

4) ETL / Pipeline Design (technical) — Pre-work
- ETL engineers to draft transformation pseudo-SQL or pipeline diagrams.
- Provide current infra constraints (compute, storage, scheduler e.g., Airflow).
- Provide SLAs needed for freshness and recovery RTO/RPO goals.
- Prepare sample data quality rules and failing-case examples.
- Attach: ETL runbook draft, pipeline diagram (if available).

5) Dashboard Design (UX + BI) — Pre-work
- Product owner to provide primary user stories and persona list.
- Request mocked sample dataset (aggregated) for prototyping.
- Designers to prepare initial wireframes or moodboard.
- BI devs to prepare sample charts with the mock dataset.
- Attach: `deliverables/KPI_SPEC.md`, wireframes.

6) Performance & QA / Validation Workshop — Pre-work
- Provide baseline query runtimes and example concurrency expectations.
- Provide expected totals and business validation rules for key KPIs.
- Prepare automated test ideas and any existing smoke test scripts.
- Attach: QA checklist and sample validation queries.

7) Deployment & Monitoring (ops/technical) — Pre-work
- Provide target hosting environment details and access method.
- Ops to prepare monitoring and alerting requirements (metrics, thresholds).
- Prepare a draft runbook and rollback plan.
- Attach: `scripts/README.md` and deployment environment notes.

8) User Training & Handoff Review — Pre-work
- Provide final dashboards for demo and training materials (slides).
- Prepare a short training plan and a list of user groups to train.
- Complete `follow_up/FUP_TEMPLATE.md` with initial handoff notes.

9) Retrospective / Post-release — Pre-work
- Collect feedback notes, bug list, enhancement backlog and usage metrics.
- Ask participants to fill a short survey ahead of time to prioritize topics.

Timing & sequencing notes
- Share technical checklists earlier (5-7 working days) to allow access provisioning.
- Combine non-technical workshops (Kickoff + Design) in a single half-day session when stakeholders are limited.

Deliverables after each workshop
- Updated `docs/PROJECT_BRIEF.md` or `deliverables/*` as applicable.
- Action items recorded in `templates/ACTION_LOG.csv` and `templates/MEETING_MINUTES.md`.
- Assigned owners and due dates added to `follow_up/FUP_TEMPLATE.md` if required.
