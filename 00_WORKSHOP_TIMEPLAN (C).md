Workshop Timeplan Proposal (C) — Dashboard Project

Purpose
- A recommended, sequenced timeplan for all meetings and workshops required to deliver the dashboard project. Includes dependencies, pre-work windows, suggested durations, and critical-path highlight.

How to read this plan
- "Week" counts from project start (Kickoff = Week 0). Days assume business days.
- "Pre-work lead" indicates how long before the session required materials should be requested.
- Sessions marked **CRITICAL** are on the project's critical path; delays there delay the project.

Summary (priority order — most important first)
1. Kickoff (CRITICAL)
2. Technical Data Discovery (deep) (CRITICAL)
3. Data Modeling / Semantic Layer (CRITICAL)
4. ETL / Pipeline Design (CRITICAL)
5. Dashboard Design (UX + BI)
6. Performance & QA / Validation
7. Deployment & Monitoring
8. User Training & Handoff
9. Retrospective / Benefits Review

Suggested 8-week timeline (example)
- Week 0 (Day 0–5): Kickoff + initial stakeholder alignment
- Week 1 (Day 6–12): Technical Data Discovery (deep) — collect samples, access provisioning
- Week 2 (Day 13–19): Data Modeling / Semantic Layer workshop
- Week 3 (Day 20–26): ETL/Pipeline design workshops and begin implementation
- Week 4 (Day 27–33): Dashboard prototyping & design iterations
- Week 5 (Day 34–40): QA & validation, automated checks
- Week 6 (Day 41–47): Finalize deployment, monitoring & runbook
- Week 7 (Day 48–54): User training and formal handoff
- Week 8 (Day 55–61): Retrospective and benefits first review

Detailed Session Plan

The detailed, editable session plan now lives in `templates/WORKSHOP_DETAILED_SESSION_PLAN.csv`. Use that CSV to sort/filter sessions, adjust dates, or import into your planning tool. This document keeps the high-level timeplan, gating, and dependencies.

Recurring coordination meetings
- Daily standup: 15 min (Week 0 → go-live). Purpose: unblock and coordinate technical work. Participants: core delivery team. Priority: High
- Weekly steering / sponsor update: 30 min (every week). Purpose: milestone status, risks, decisions. Participants: Sponsor, PM, BI Lead. Priority: High
- Prototype demo cadence: end of Week 4 and Week 5 (UAT demo). Purpose: gather feedback and sign-offs. Participants: Stakeholders. Priority: High

Critical path & blockers (summary)
- Data access & sample completeness: Any delay in access or samples blocks Data Discovery and therefore Modeling and ETL. Pre-provision access 5–7 days before the Data Discovery session.
- Modeling decisions (grain, joins, canonical entities): If modeling is delayed, ETL and dashboard development cannot progress reliably.
- ETL implementation & data freshness: ETL must provide reliable datasets for QA and prototyping; prioritize automation and monitoring early.

Parallelization opportunities
- While ETL engineers build base tables, designers and BI developers can progress with mock/aggregated datasets for visualization design.
- Small teams can run Data Modeling and Dashboard Design in parallel if sample data is available and responsibilities are clear.

Compressed schedule option (2–3 week sprint)
- Day 0: Kickoff + immediate request for samples and access.
- Days 1–3: Technical Data Discovery (accelerated) — must have full-time support from data owners.
- Days 4–6: Modeling + ETL design sprint (daily checkpoints).
- Days 7–10: Dashboard rapid prototype using mock data; iterate with stakeholders.
- Days 11–14: QA, deploy minimal viable dashboard, run training and handoff.
Notes: Compression is high-risk; ensure stakeholders and data owners are available and accept trade-offs on depth of validations.

Pre-work deadlines (recommended)
- Kickoff pre-work: 3 working days before Kickoff.
- Data Discovery: request samples and access 5–7 working days before session; samples delivered >=3 days before.
- Modeling & ETL: modeling inputs available 3 days prior.
- Design: wireframes and mock datasets 3 days prior.
- QA: validation rules and expected totals 3 days prior.

PMI gating criteria (Go/No-Go gates per milestone)
Below are the recommended PMI-style gating criteria to confirm before moving from one milestone to the next. Capture sign-offs in `templates/DECISION_LOG.md` and update `templates/ACTION_LOG.csv` for any open remediation tasks.

- After Kickoff (gate: Proceed to Data Discovery)
	- Project Charter signed by Sponsor (`docs/PROJECT_CHARTER.md`).
	- Stakeholder register completed and primary owners identified (`docs/STAKEHOLDER_ENGAGEMENT_PLAN.md`).
	- Initial RACI assigned and PM/BI lead confirmed.

- After Security & Privacy (gate: Begin Data Discovery)
	- Data classification completed; PII/sensitive fields identified (`docs/DATA_GOVERNANCE.md`).
	- Access request process defined and responsible approvers listed.
	- Any required masking/consent actions documented.

- After Technical Data Discovery (gate: Proceed to Modeling)
	- `deliverables/DATA_INVENTORY.md` completed for all in-scope sources.
	- Sample extracts provided and basic profiling completed (row counts, nulls, cardinalities).
	- Outstanding critical data quality issues logged with owners and mitigation plan.

- After Data Modeling (gate: Proceed to ETL design)
	- Canonical model diagram and grain definitions agreed and documented.
	- KPI definitions mapped to model fields in `deliverables/KPI_SPEC.md`.
	- Performance considerations and partitioning strategy noted.

- After ETL Implementation (gate: Proceed to Dashboard prototyping / QA)
	- ETL jobs run successfully in staging with reproducible results and scheduled runs.
	- Basic reconciliation tests pass (key totals match source within acceptance thresholds).
	- Monitoring and alerting for ETL job failures configured and tested.

- After Dashboard Prototype (gate: Proceed to UAT)
	- Wireframes and mockups signed off by Product Owner.
	- Prototype connects to staging datasets and demonstrates key interactions.
	- Initial performance benchmarks meet targets for critical views.

- After QA / UAT (gate: Proceed to Deployment)
	- All P0 defects resolved; P1 defects have documented mitigations and timelines.
	- UAT acceptance criteria met and signed off by Product Owner (`templates/ACCEPTANCE_CRITERIA.md`).
	- Security/compliance sign-off for production access.

- After Deployment (gate: Handoff to BAU)
	- Runbook and monitoring are live and tested (`scripts/README.md`).
	- Training completed and `follow_up/FUP_TEMPLATE.md` contains support contacts and SLA expectations.
	- Benefits tracking plan initiated and baseline metrics recorded (`docs/BENEFITS_REALIZATION.md`).

Deliverables / outputs per session (quick list)
- Kickoff: Updated `docs/PROJECT_BRIEF.md`, action log entries
- Data Discovery: Completed `deliverables/DATA_INVENTORY.md` and sample extracts
- Data Modeling: Model diagram and canonical table definitions
- ETL Design: Pipeline diagrams, schedules, and runbook drafts
- Dashboard Design: Wireframes, `deliverables/KPI_SPEC.md` finalized
- QA & Validation: QA plan, validation scripts, acceptance tests
- Deployment: Runbook, monitoring thresholds, access setup
- Training: Training slides and recorded sessions, `follow_up/FUP_TEMPLATE.md` updated
- Retrospective: Retrospective notes, prioritized backlog

Risk notes & mitigations tied to schedule
- Risk: Access delays — Mitigation: escalate immediately to Sponsor; identify alternate sample sources.
- Risk: Key SME unavailability — Mitigation: identify backup SMEs in advance and use recorded interviews.
- Risk: Performance issues late in schedule — Mitigation: early performance benchmarks and incremental load testing.

Next steps I can take for you
- Generate calendar-ready invite snippets (Outlook/ICS) for each session and save them in `templates/`.
- Produce a printable one-page Gantt (PNG) of this 8-week plan for stakeholder distribution.
- Adapt this plan to your actual project start date and produce per-day calendar items.

---
Files referenced (where to find templates and artifacts)
- `docs/PROJECT_BRIEF.md`
- `workshops/` (agendas and pre-work checklists). Note: workshop files are numbered for priority, for example:
	- `workshops/01_WORKSHOP_AGENDA_KICKOFF.md`
	- `workshops/02_PRE_WORK_DATA_DISCOVERY.md`
	- `workshops/03_PRE_WORK_DATA_MODELING.md`
- `deliverables/` (KPI spec, data inventory, architecture, vis spec)
- `templates/` (action log, email invites, decision log, FUP template)
