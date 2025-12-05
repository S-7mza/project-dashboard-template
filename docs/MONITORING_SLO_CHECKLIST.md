Monitoring & SLO Checklist

Purpose
- Define what to monitor for the dashboard (data pipelines, KPIs, infrastructure) and the service-level objectives (SLOs).

Monitoring Scope
- ETL jobs / pipelines
- Data quality checks
- Dashboard availability and performance

SLOs & Metrics
| Area | Metric | Target / SLO | Owner | Tool / Dashboard |
|------|--------|--------------|-------|------------------|
| ETL freshness | Time since last successful load | [e.g., < 2h] | Data Engineer | [Monitoring tool link] |
| ETL reliability | Failed jobs per week | [e.g., < 1] | Data Engineer | |
| KPI accuracy | Reconciliation error | [e.g., < 1%] | Data Owner | |
| Dashboard availability | Uptime in business hours | [e.g., 99.5%] | Ops | |
| Performance | P95 page load time | [e.g., < 5s] | BI Lead | |

Alerts & Escalation
- Define alert thresholds for each metric.
- Map to escalation path in `follow_up/FUP_TEMPLATE.md`.

Runbooks
- For each critical alert, link to a runbook page or script in `scripts/` explaining how to investigate and resolve.

Review
- Review SLOs quarterly or when usage patterns change.
