Technical Data Discovery — Agenda (detailed)

Duration: 90–120 minutes (may be run per source)
Attendees: Data owners, ETL engineers, BI developers, PM

1. Objective & scope (10 min)
- Confirm goals, KPIs in scope, and what we must deliver from this session.

2. Source inventory walkthrough (30–40 min)
- For each source: owner, schema, sample queries, row counts, refresh cadence.
- Note access method and credentials owner (do not share secrets in the meeting).

3. Sample data review (30 min)
- Walk through sample extracts; run a couple of validation queries live.
- Identify data quality issues, NULLs, unexpected values and cardinality problems.

4. Security & compliance check (15 min)
- Identify PII and sensitive fields, masking requirements and data residency constraints.

5. Next steps & actions (15 min)
- Assign owners for access provisioning, data fixes, and alternative sources.

Outputs
- Updated `deliverables/DATA_INVENTORY.md` entries, sample extract files, initial quality report and action items in `templates/ACTION_LOG.csv`.
