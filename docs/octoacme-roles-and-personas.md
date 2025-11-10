# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX Designer

### Role Summary
UX Designers define and improve the user experience by creating wireframes, prototypes, and design systems. They ensure that products are intuitive, accessible, and meet user needs through research and iterative design.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, mockups, and interactive prototypes
- Define and maintain design systems and style guides
- Collaborate with Product Managers on requirements and user flows
- Provide design specifications and assets to Developers
- Participate in design reviews and user acceptance testing

### Goals
- Create intuitive, accessible user experiences
- Reduce user friction and improve satisfaction metrics
- Ensure design consistency across the product
- Validate designs through user feedback and testing

### Typical Communication
- Design reviews with Product Managers and Developers
- User research findings and usability test results
- Design specs and asset handoffs via design tools
- Sprint planning for design work alignment

### Interactions with Other Roles
- **Product Managers**: Collaborate on feature requirements, user stories, and acceptance criteria. Provide insights from user research to inform prioritization.
- **Developers**: Provide design specifications, assets, and clarifications during implementation. Review implementations for design accuracy.
- **QA Lead**: Partner on usability testing and acceptance criteria validation from a user experience perspective.
- **Project Managers**: Communicate design timelines, dependencies on user research, and flag design-related risks.

---

## QA Lead

### Role Summary
QA Leads own the quality strategy and coordinate all testing activities to ensure features meet acceptance criteria and quality standards. They bridge development and release by systematically verifying functionality, performance, and reliability.

### Responsibilities
- Define and maintain test strategy and quality standards
- Plan and coordinate manual and automated test activities
- Create and maintain test plans, test cases, and test data
- Track defects, triage issues, and drive resolutions
- Ensure acceptance criteria coverage for all features
- Lead regression testing before releases
- Advocate for quality improvements and preventive measures

### Goals
- Prevent defects from reaching production
- Maintain high test coverage and quality metrics
- Reduce mean time to detect and resolve issues
- Build confidence in release readiness

### Typical Communication
- Daily standups to discuss testing progress and blockers
- Bug reports and defect triage meetings
- Test status updates in sprint reviews
- Quality metrics dashboards and reports

### Interactions with Other Roles
- **Developers**: Collaborate closely during feature development to clarify acceptance criteria, report bugs, and verify fixes. Partner on automated test development.
- **Product Managers**: Work together to refine acceptance criteria and ensure testability. Provide quality insights for release decisions.
- **DevOps Engineer**: Coordinate on test environment setup, test automation integration in CI/CD, and production monitoring.
- **UX Designer**: Partner on usability testing and ensure design implementations meet user experience standards.
- **Customer Support Liaison**: Receive feedback on recurring issues to improve test coverage and prioritize bug fixes.

---

## DevOps Engineer

### Role Summary
DevOps Engineers manage infrastructure, CI/CD pipelines, and deployment automation. They enable reliable, repeatable releases and maintain system health through monitoring, incident response, and infrastructure as code practices.

### Responsibilities
- Design, build, and maintain CI/CD pipelines
- Manage infrastructure as code (IaC) and cloud resources
- Monitor system health, performance, and availability
- Automate deployment processes and rollback procedures
- Support incident triage and resolution
- Implement security best practices in deployment workflows
- Optimize build times and deployment efficiency

### Goals
- Achieve fast, reliable, low-risk deployments
- Minimize manual deployment effort through automation
- Maintain high system availability and performance
- Reduce mean time to recovery (MTTR) for incidents

### Typical Communication
- Deployment status updates and release coordination
- Incident reports and post-mortems
- Infrastructure change notifications
- CI/CD pipeline metrics and improvement proposals

### Interactions with Other Roles
- **Developers**: Partner to streamline development workflows, optimize build processes, and troubleshoot deployment issues. Provide tooling and automation support.
- **Project Managers**: Coordinate on release schedules, communicate deployment windows, and report on infrastructure constraints or risks.
- **QA Lead**: Collaborate on test environment provisioning, test automation integration in CI/CD, and smoke test execution.
- **Product Managers**: Provide deployment capabilities and constraints to inform release planning. Report on system metrics affecting user experience.
- **Customer Support Liaison**: Respond to production incidents and provide system status information.

---

## Customer Support Liaison

### Role Summary
Customer Support Liaisons represent the voice of the customer within the development team. They surface user feedback, pain points, and feature requests while keeping support teams informed about product changes and known issues.

### Responsibilities
- Collect and analyze customer feedback and pain points
- Relay feature requests and bug reports to the product team
- Provide context on customer impact for prioritization decisions
- Communicate upcoming changes and release notes to support teams
- Participate in user acceptance testing from a support perspective
- Document common issues and workarounds for support knowledge base
- Represent customer concerns in retrospectives and planning

### Goals
- Reduce customer-reported issues and support tickets
- Improve product usability based on real user feedback
- Ensure smooth communication between customers and development
- Minimize customer impact during releases and incidents

### Typical Communication
- Weekly summaries of customer feedback trends
- Bug reports with customer impact context
- Release notes and feature announcements for support teams
- Escalations of critical customer issues

### Interactions with Other Roles
- **Product Managers**: Share customer insights to inform roadmap and backlog prioritization. Provide feedback on proposed solutions.
- **Developers**: Report recurring issues with reproduction steps and customer context. Validate fixes from a user perspective.
- **QA Lead**: Collaborate on testing scenarios based on real customer usage patterns. Provide customer data for test case creation.
- **UX Designer**: Share user feedback on design pain points and usability issues. Participate in user research activities.
- **Project Managers**: Communicate customer-critical issues that may affect project scope or timeline. Provide customer impact assessments for risk planning.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

