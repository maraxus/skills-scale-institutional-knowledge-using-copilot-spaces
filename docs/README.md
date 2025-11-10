# OctoAcme Project Management Guide

Welcome to OctoAcme's project management documentation! This guide provides an overview of how we run projects, manage teams, and deliver value to our customers.

## Introduction

OctoAcme's project management approach is designed to help new team members quickly understand our processes, workflows, and expectations. We follow a structured yet flexible methodology that emphasizes:

- **Customer-first thinking**: We prioritize customer value and usability in every decision
- **Iterative delivery**: We deliver small, testable increments rather than large releases
- **Clear ownership**: Every project has designated owners and accountable roles
- **Data-informed decisions**: We measure impact and iterate based on evidence
- **Psychological safety**: We encourage feedback, learning, and continuous improvement

This approach applies to all cross-functional projects that deliver product features, services, or integrations.

## Process Lifecycle

OctoAcme projects follow a five-phase lifecycle:

### 1. Initiation

The initiation phase validates and authorizes new work before significant resources are committed.

**Key Activities:**
- Confirm business need and measurable outcomes
- Identify stakeholders and champions
- Define success criteria and initial timeline
- Assess initial risks and dependencies
- Estimate resource needs

**Key Deliverables:**
- Project One-pager (Problem, Goal, Success Metrics)
- Stakeholder list and communication plan
- High-level timeline with key milestones
- Initial risk assessment
- Resource requirements (team roles, effort estimate)

**Decision Gate:** Move to planning when success metrics are clear, stakeholders agree on priority, and team availability is confirmed.

### 2. Planning

The planning phase transforms an approved initiative into an actionable delivery plan.

**Key Activities:**
- Hold kickoff meeting with stakeholders and delivery team
- Create prioritized backlog with acceptance criteria
- Estimate scope (T-shirt sizing or story points)
- Define Definition of Done (DoD)
- Identify dependencies and integration points
- Create release plan and milestone map

**Key Deliverables:**
- Prioritized and estimated backlog
- Release timeline with milestones
- Definition of Done documentation
- Risk register with mitigation strategies
- Initial test plan and QA approach

### 3. Execution

The execution phase focuses on day-to-day development, testing, and progress tracking.

**Key Activities:**
- Daily standups (15 min) — progress, blockers, dependencies
- Weekly delivery sync — show progress and flag risks
- Demo/Review at sprint or milestone completion
- Pull Request workflow with code reviews
- Continuous testing and quality assurance
- Regular risk register updates

**Workflows:**
- Use project boards with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Create small PRs (≤ 400 lines when possible)
- Include issue links and acceptance criteria in PR descriptions
- Run automated tests and linting in CI before requesting review
- Require at least one approval before merging

**Quality & Testing:**
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows
- Security scanning in CI
- Manual QA for feature acceptance when needed

### 4. Release & Deployment

The release phase standardizes how features reach production with minimal risk.

**Release Types:**
- **Patch**: Hotfixes addressing critical production issues
- **Minor**: Incremental features and improvements
- **Major**: Significant functionality or breaking changes

**Pre-release Requirements:**
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback/mitigation plan documented
- Smoke tests prepared

**Deployment Process:**
1. Schedule deployment window (if needed)
2. Create backup or snapshot (if applicable)
3. Deploy to staging and run smoke tests
4. Deploy to production (automated pipeline preferred)
5. Run post-deploy verifications
6. Announce release to stakeholders and support

**Rollback Plan:** If deployment fails or causes critical issues, trigger incident response, rollback to last known-good release if necessary, and capture action items for improvement.

### 5. Retrospective & Continuous Improvement

The retrospective phase captures learnings and converts them into actionable improvements.

**When:** After each sprint, release, important milestone, or incident.

**Structure:**
- What went well
- What could be improved
- Action items with owners and due dates
- Follow-up on previous action items

**Best Practices:**
- Timebox to 45–75 minutes depending on team size
- Use anonymous idea boards when needed to encourage candor
- Prioritize 2–3 top action items to avoid overload
- Add action items to backlog with clear owners and timelines
- Measure impact of improvements and celebrate progress

## Roles & Responsibilities

### Developer

**Role Summary:** Developers design, build, test, and deliver software components while collaborating with product and project leads.

**Key Responsibilities:**
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

**Communication:** Daily standups, sprint planning, PR descriptions, code review comments, and technical design docs.

### Product Manager (PdM)

**Role Summary:** Product Managers define what should be built to deliver customer and business value. They own the product vision and measure outcomes.

**Key Responsibilities:**
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

**Communication:** Weekly alignment with PM and engineering leads, roadmap updates, stakeholder briefings, and feature specifications.

### Project Manager (PM)

**Role Summary:** Project Managers coordinate delivery activities, manage schedules, risks, and communications to enable efficient delivery.

**Key Responsibilities:**
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

**Communication:** Weekly status updates, stakeholder reports, risk registers, decision logs, and meeting facilitation.

### Stakeholders

**Role Summary:** Stakeholders provide inputs, approvals, and feedback to ensure projects meet business needs.

**Key Responsibilities:**
- Provide business context and requirements
- Review and approve key decisions and deliverables
- Participate in milestone reviews and demos
- Communicate organizational priorities and constraints

**Communication:** Monthly stakeholder updates, milestone reviews, and ad-hoc escalations as needed.

## Communication Strategies

### Regular Cadence

- **Daily standups** (15 min): Team-level progress, blockers, dependencies
- **Twice-weekly team standups**: Delivery team coordination (or as agreed)
- **Weekly PM + PdM sync**: Alignment on priorities and risks
- **Weekly delivery sync**: Progress updates and risk flagging
- **Monthly stakeholder updates**: High-level status and upcoming milestones
- **Sprint/milestone demos**: Showcase completed work

### Status Reporting

**Weekly Status Template:**
- Progress this week
- Next steps
- Risks & blockers
- Asks/decisions needed

### Escalation Paths

- **Level 1**: Team-level triage in daily standup
- **Level 2**: PM escalates to Product Lead and dependent teams
- **Level 3**: Sponsor-level escalation for business-impacting issues
- **Security incidents**: Follow security incident runbook and notify Security on-call

### Stakeholder Communication

- Identify stakeholder groups and their communication needs (engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Maintain a single source of truth (project README or release doc) for status
- Use appropriate channels for different audiences

## Quality Assurance Practices

OctoAcme maintains high quality standards through multiple complementary practices:

### Testing Strategy

- **Unit tests**: Test individual components and logic in isolation
- **Integration tests**: Verify interactions between components
- **End-to-end smoke tests**: Validate critical user flows before release
- **Manual QA**: Feature acceptance testing when needed
- **Test coverage**: Maintain high coverage and observability

### Code Reviews

- All code changes reviewed before merging
- Small PRs (≤ 400 lines when possible) for easier review
- PR descriptions include issue links and acceptance criteria
- At least one approval required (or team-defined policy)
- Focus on correctness, maintainability, and security

### Continuous Integration/Continuous Deployment (CI/CD)

- **Automated testing**: Run tests in CI before code review
- **Linting and formatting**: Enforce code style standards
- **Security scanning**: Automated vulnerability detection
- **Automated deployment**: Pipeline-based deployments to reduce manual errors
- **Rollback capability**: Quick rollback to last known-good release

### Definition of Done (DoD)

Each team defines their DoD, typically including:
- Feature meets all acceptance criteria
- Tests written and passing
- Code reviewed and approved
- Documentation updated
- Security scan passed
- Deployed to staging and verified

### Retrospectives

- Regular retrospectives after sprints, releases, and incidents
- Blameless culture focused on learning
- Action items tracked and reviewed
- Continuous process improvement based on team feedback

### Risk Management

**Risk Register:** Maintain a simple table tracking:
- ID and description
- Impact and likelihood (High/Med/Low)
- Owner and mitigation plan
- Current status

**Risk Lifecycle:**
1. **Identify**: During planning and ongoing execution
2. **Assess**: Estimate impact and likelihood
3. **Mitigate**: Implement actions and contingency plans
4. **Monitor**: Review at weekly syncs and update status

## Key Artifacts

Throughout the project lifecycle, maintain these key documents:

- **Project Charter / One-pager**: Problem statement, goals, success metrics
- **Roadmap and Release Plan**: Timeline with milestones and deliverables
- **Sprint/Iteration Backlog**: Prioritized work items with estimates
- **Acceptance Criteria & Definition of Done**: Quality standards for completion
- **Risk Register**: Current risks, mitigations, and owners
- **Retrospective Notes and Action Items**: Learnings and improvements
- **Release Notes**: Changes, migration steps, and known issues

## How to Use These Docs

- Keep the Project Charter updated in your project repository
- Add process-specific documentation to `.copilot/` if you want Copilot Spaces to use them as context
- Reference specific guides for detailed workflows:
  - [Project Management Overview](octoacme-project-management-overview.md)
  - [Roles and Personas](octoacme-roles-and-personas.md)
  - [Project Initiation](octoacme-project-initiation.md)
  - [Project Planning](octoacme-project-planning.md)
  - [Execution and Tracking](octoacme-execution-and-tracking.md)
  - [Release and Deployment](octoacme-release-and-deployment.md)
  - [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
  - [Risk Management and Communication](octoacme-risks-and-communication.md)

## Getting Started

New to OctoAcme projects? Follow these steps:

1. **Read this guide** to understand our overall approach
2. **Review the detailed guides** relevant to your role
3. **Join the team's daily standup** to understand current work
4. **Connect with your Project Manager** for onboarding and context
5. **Review the project board** to see current status and backlog
6. **Ask questions** — we value learning and psychological safety!

---

*This guide synthesizes OctoAcme's project management documentation to provide a comprehensive overview for new team members. For detailed procedures and templates, refer to the individual guides linked above.*
