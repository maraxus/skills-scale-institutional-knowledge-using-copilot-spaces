# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
  - **QA Lead**: Owns the QA column, coordinates testing activities, and approves items moving to Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - **UX Designer**: Review PRs affecting user interface for design accuracy
  - Run automated tests and linting in CI before requesting review
  - **DevOps Engineer**: Maintain CI/CD pipeline to run tests, security scans, and builds
  - Require at least one approval before merging (or team-defined policy)
  - **QA Lead**: Perform manual testing when automated tests are insufficient

## Quality & Testing
- **QA Lead**: Owns overall test strategy and quality assurance
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- **DevOps Engineer**: Security scanning in CI/CD pipeline
- Manual QA for feature acceptance when needed (coordinated by QA Lead)
- **UX Designer**: Usability validation for new features and design changes

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- **DevOps Engineer**: Maintain dashboards for key signals (errors, latency, usage, system health)
- **QA Lead**: Track quality metrics (defect rates, test coverage, escaped defects)
- **Customer Support Liaison**: Report customer feedback trends and support ticket volumes

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint (DevOps Engineer)
- [ ] Design assets and specifications available (UX Designer)
- [ ] Test environments provisioned and accessible (DevOps Engineer, QA Lead)
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Quality metrics dashboard in place (QA Lead)
- [ ] Customer feedback collection process active (Customer Support Liaison)
