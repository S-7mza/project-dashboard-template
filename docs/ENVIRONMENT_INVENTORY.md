Environment Inventory

Use this document to capture environment details for Dev / Staging / Prod used by the project.

Environment | Purpose | Host / URL | Owner | Access method | Credentials vault location | Notes
---|---|---|---|---|---|---
Dev | Development and prototyping | [host] | [owner] | VPN/SSO | [vault link] | Sample/Masked data recommended
Staging | Pre-production testing | [host] | [owner] | VPN/SSO | [vault link] | Mirror prod for UAT
Prod | Production dashboards | [host] | [owner] | SSO/managed | [vault link] | Monitoring and alerts active

Include network, firewall, subnet, and region info if relevant. Do not store credentials in repo.