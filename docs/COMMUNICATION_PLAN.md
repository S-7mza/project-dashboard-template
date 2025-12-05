Communication Plan
Communication Plan — Dashboard Project

## 1. Objectives

- Align stakeholders on scope, priorities, and timeline.
- Avoid surprises by surfacing risks, issues, and scope changes early.
- Support timely decisions at each gate and design milestone.
- Drive adoption with clear, consistent messaging to end users.

## 2. Stakeholder Groups

- Executive Sponsor / Steering Committee
- Product Owner / Business Lead
- Project Manager
- BI / Data Engineering Team
- Data Owners / SMEs
- Security / Compliance
- Operations / DevOps
- End Users / Trainers

## 3. Communication Matrix

| Channel / Artifact | Audience | Owner | Purpose | Frequency / Timing | Format & Tools |
|---|---|---|---|---|---|
| Project Charter & Brief | Sponsor, PO, PM, core team | PM | Align on objectives, scope, success metrics | Once at project start; update on major change | `docs/PROJECT_BRIEF.md`, `docs/PROJECT_CHARTER (C).md` |
| Weekly status report | Sponsor, PO, key stakeholders | PM | Summarize progress, risks, decisions, next steps | Weekly until go-live | Email + links to `templates/DECISION_LOG.md`, `templates/ACTION_LOG.csv`, `templates/ISSUE_LOG.md` |
| Steering / Sponsor meeting | Sponsor, PM, BI Lead | PM | Confirm milestones, resolve escalations, Go/No-Go | Every 2–3 weeks or at key gates | 30–45 min call + slides; use `02_GATING_CHECKLIST (C).md` |
| Daily standup | Delivery team | Scrum Master / PM | Coordinate work, unblock issues | Daily on working days | 15 min standup; capture actions in `templates/ACTION_LOG.csv` |
| Workshop invitations | Stakeholders per workshop | PM / PO | Ensure right people join with prep | Per workshop, 5–10 days before | Calendar invite referencing `workshops/*`, `00_WORKSHOP_TIMEPLAN (C).md`, templates from `templates/EMAIL_INVITES.md` |
| Design / Prototype demos | Sponsor, PO, key users | BI Lead / PO | Validate design, collect feedback, sign-off | At least end of Weeks 4 & 5 | Demo meetings; capture decisions in `templates/DECISION_LOG.md` |
| Risk & issue updates | PM, Sponsor, team | PM | Make risks and issues visible and owned | Weekly review or as needed | `templates/RISK_REGISTER.md`, `templates/ISSUE_LOG.md`, summary in status report |
| Security & privacy review | Security, Data Owners, PM | Security Lead | Approve data usage, access, controls | Once during early Data Discovery; as needed | Session using `workshops/02_WORKSHOP_AGENDA_SECURITY_PRIVACY.md`, `docs/DATA_GOVERNANCE (C).md` |
| UAT communications | UAT testers, PO, PM | QA Lead / PO | Prepare and run UAT, capture outcomes | Before and during UAT window | UAT brief + `docs/TEST_UAT_PLAN (C).md`, `templates/ACCEPTANCE_CRITERIA.md` |
| Deployment & change notice | Operations, users, support | PM / Ops | Announce deployment, downtime, and changes | Before go-live, plus follow-up | Email / intranet; reference `docs/DEPLOYMENT_RUNBOOK.md`, `deliverables/DASHBOARD_USER_GUIDE.md` |
| Training invitations & materials | End users, trainers | Training Lead / PM | Ensure users know how and when to join training | Before training sessions | Calendar invites referencing `workshops/08_WORKSHOP_AGENDA_TRAINING_HANDOFF.md`, materials in `follow_up/FUP_TEMPLATE.md` |
| Post-go-live support comms | Users, support, PM | Support Lead / PM | Provide support channels and SLAs | At go-live and first weeks | Support contact info and SLAs in `follow_up/FUP_TEMPLATE.md` |
| Benefits tracking update | Sponsor, PO, PMO | PM / PO | Show realized and expected benefits | Monthly/quarterly | `docs/BENEFITS_REALIZATION.md`, `docs/BENEFITS_TRACKER.csv` |

## 4. Key Messages by Phase

- Initiation (Weeks 0–1): Why the project exists, what success looks like, who decides what.
- Discovery & Design (Weeks 1–4): Data in scope, constraints, risks, and how/when feedback is collected.
- Build & Test (Weeks 3–6): What is being built now, limits of this release, testing windows.
- Deployment & Handoff (Weeks 6–7): Go-live timing, impact, rollback, training and support.
- Benefits & Continuous Improvement (Week 8+): Early benefits, adoption metrics, how to request enhancements.

## 5. Routines to Ensure Nothing Is Missed

- Single sources of truth:
	- All actions in `templates/ACTION_LOG.csv`.
	- All decisions in `templates/DECISION_LOG.md`.
	- All issues in `templates/ISSUE_LOG.md`.
- Standard closing questions for every recurring meeting:
	- Any new risks or issues? → log in `RISK_REGISTER.md` / `ISSUE_LOG.md`.
	- Any decisions today? → log in `DECISION_LOG.md`.
	- Any actions? → log with owner & due date in `ACTION_LOG.csv`.
- Gate reviews:
	- Before each gate, send pre-read referencing `02_GATING_CHECKLIST (C).md` and relevant artifacts.
	- After each gate, send a short outcome email with decision and action IDs.

## 6. Escalation Paths

- Operational / technical blocker (>1 day impact):
	- Raise in daily standup and log in `ISSUE_LOG.md`.
	- If unresolved within agreed SLA, PM escalates to Sponsor via status report and, if severe, direct email.
- Scope / priority conflicts:
	- Discuss first in backlog grooming with PO.
	- If unresolved, escalate to Sponsor/Steering with options and impact.
- Risk materialization:
	- PM updates `RISK_REGISTER.md` and links to actions.
	- Communicate impact and mitigation in next status report.

## 7. Plan Review

- At project start, PM reviews this communication plan with Sponsor and PO and stores it here.
- Every 2–3 weeks, PM checks whether channels, frequencies, and audiences are still appropriate and adjusts as needed.

Purpose
- Standardize communications across the project to ensure timely, consistent information flow.

Audiences & Frequency
- Sponsor: Weekly executive summary (email/one-pager).
- Steering group: Bi-weekly progress review and milestone updates.
- Core team: Daily standup (async) and weekly sync.
- End users: Feature demos at milestone completion and training sessions.

Channels
- Instant messaging (Teams/Slack) for day-to-day questions.
- Email for formal updates and approvals.
- Shared docs (this repo) for artifacts and source of truth.
- Calendar invites for workshops and key milestones.

Templates & Artifacts
- Use `templates/EMAIL_INVITES.md` for invites.
- Use `templates/MEETING_MINUTES.md` for meeting outputs.
- Use `templates/ACTION_LOG.csv` to track and report open actions.

Escalation
- Urgent operational incidents: follow the escalation path in `follow_up/FUP_TEMPLATE.md`.
- Unresolved scope or budget issues: escalate to Sponsor.

Owner
- PM is the primary owner for communications; BI Lead manages technical updates.

Review cadence
- Review this plan at each major milestone or when stakeholder list changes.