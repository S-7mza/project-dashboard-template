ETL / Pipeline Design — Pre-work Checklist

Send 3–5 working days before the session.

Required inputs
- Proposed transformation pseudo-SQL or diagrams for key ETL jobs.
- Current infrastructure details: scheduler (Airflow, Prefect), compute/warehouse limits, storage considerations.
- SLAs for data freshness, RTO/RPO and retention policy.
- Typical failure modes and existing retry/error strategies.

Required attendees
- ETL engineers, data owners, BI developer, ops/devops representative.

Attachments to include in invite
- `deliverables/ARCHITECTURE.md` (draft)
- Any existing pipeline diagrams or runbooks.

Goals for the session
- Agree on pipeline orchestration, idempotency, partitioning and incremental strategies.
- Define monitoring and alerting requirements for ETL failures.

Post-meeting outputs
- ETL design document with schedules, recovery steps and monitoring checks.
- Action items for implementation and access needs.
