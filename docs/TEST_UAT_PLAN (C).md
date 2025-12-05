Test & UAT Plan

Purpose
- Define how the dashboard will be tested prior to sign-off including test types, environments, roles, and exit criteria.

Test Types
- Unit tests: for ETL transforms and SQL logic (developer-owned).
- Integration tests: end-to-end checks from source to dashboard (BI/Data owner).
- Regression tests: ensure new changes don't break existing KPIs.
- Performance tests: measure load times under expected concurrency.
- UAT: business-driven acceptance testing with product owners and stakeholders.

Environments
- Dev: prototype and early development with masked or sampled data.
- Staging / Pre-prod: production-like environment for UAT and performance tests.
- Prod: live environment for deployment.

Test Roles
- Test Owner / QA Lead: coordinates test plan and execution.
- BI Developer: provides test artifacts and fixes.
- Data Owner: validates reconciliation results.
- Product Owner: performs UAT and acceptance.

Test Artifacts
- Test cases and expected results (store in `docs/tests/` or repo)
- Validation queries and datasets
- Automated validation scripts (store in `scripts/`)

UAT Process
- Prepare UAT checklist and acceptance criteria (`templates/ACCEPTANCE_CRITERIA.md`).
- Execute UAT in staging with business users; collect issues in `templates/ISSUE_LOG.md`.
- UAT sign-off recorded in `templates/DECISION_LOG.md` or `follow_up/FUP_TEMPLATE.md`.

Exit Criteria
- All P0 defects resolved.
- KPI reconciliation within defined thresholds.
- Performance tests meet targets.
- Stakeholder sign-off recorded.

Schedule
- Align UAT window with stakeholder availability; include time for remediation and retest.

Post-UAT
- Move deployment to production following runbook and deployment checklist.
- Post-deployment smoke checks and monitoring ramp-up.