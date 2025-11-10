# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support, customers)
  - **Customer Support Liaison**: Acts as the voice of customers, relays feedback and concerns to the team
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- **Customer Support Liaison**: Share release notes and known issues with support teams ahead of deployments

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:
- Customer feedback highlights (Customer Support Liaison):

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- **Customer Support Liaison**: Customer impact and communication plan
- **DevOps Engineer**: Technical details and system status
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
- For customer-critical issues: Customer Support Liaison -> PM -> Product Lead
- For infrastructure incidents: DevOps Engineer -> PM -> Infrastructure Lead
