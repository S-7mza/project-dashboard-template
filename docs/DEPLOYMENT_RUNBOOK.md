Deployment Runbook

Purpose
- Step-by-step guide for deploying the dashboard to each environment.

Environments
- Dev: [URL]
- Staging: [URL]
- Prod: [URL]

Pre-requisites
- CI pipeline configured and green.
- Access to deployment tools.

Steps (example)
1. Tag release in version control.
2. Trigger CI/CD pipeline for Dev → Staging.
3. Run smoke tests (link to scripts in `scripts/`).
4. Obtain UAT sign-off.
5. Trigger production deployment.
6. Run post-deploy smoke and monitoring checks.

Rollback
- Describe rollback steps and conditions.

Contacts
- On-call / support contacts and escalation path.
