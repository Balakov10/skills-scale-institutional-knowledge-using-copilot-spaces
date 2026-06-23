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

## Additional Personas

### Release Manager

#### Role Summary
Release Managers own the coordination, scheduling, and execution of releases. They ensure deployment readiness, manage rollback strategies, and communicate release information to all stakeholders. This role bridges engineering delivery with production operations.

#### Responsibilities
- Coordinate release windows and deployment schedules
- Ensure pre-release readiness (backups, snapshots, smoke tests)
- Author comprehensive release notes with migration steps
- Validate rollback plans and incident response procedures
- Communicate release status to stakeholders and support teams
- Track and manage known issues post-release

#### Goals
- Reduce deployment risk and cycle time
- Minimize release-related incidents and regressions
- Ensure clear stakeholder communication throughout the release

#### Typical Communication
- Release planning meetings with PM and engineering leads
- Pre-release readiness checklists with infrastructure/ops
- Release announcements to support and customer success teams
- Post-release retrospectives and incident reviews

#### Interactions
- **Product Manager**: Align on release timing, priority, and customer communication
- **Developers**: Validate deployment readiness and coordinate cutover activities
- **QA/Testing**: Coordinate pre-release testing and sign-off
- **Infrastructure/SRE**: Plan infrastructure changes, backups, and rollback procedures
- **Support/Customer Success**: Prepare support runbooks and customer-facing announcements

---

### Observability / On-Call Engineer

#### Role Summary
Observability Engineers ensure production systems are properly instrumented, monitored, and alerted. They define SLOs, maintain dashboards, and own the post-incident instrumentation improvements. This role enables fast detection and diagnosis of production issues.

#### Responsibilities
- Define and maintain SLOs (Service Level Objectives) and error budgets
- Instrument code for observability (metrics, logs, traces)
- Design and maintain dashboards for key system signals
- Configure and tune alerting rules to reduce noise and false positives
- Own on-call runbooks and incident playbooks
- Conduct post-incident reviews to identify instrumentation gaps

#### Goals
- Achieve reliable, predictable system behavior
- Enable rapid incident detection and diagnosis
- Reduce mean time to recovery (MTTR) and time to detection (TTD)
- Balance alerting sensitivity with alert fatigue

#### Typical Communication
- Weekly observability reviews in execution/standup meetings
- Incident war rooms during production issues
- Retrospectives focused on instrumentation improvements
- On-call handoff briefings

#### Interactions
- **Developers**: Guide instrumentation best practices and review code for observable patterns
- **Product Managers**: Align on critical business metrics and SLOs
- **Security/Infrastructure**: Coordinate on compliance and infrastructure metrics
- **Release Manager**: Communicate health dashboards during deployments

---

### Security Reviewer (Security SME)

#### Role Summary
Security Reviewers provide security expertise throughout the project lifecycle. They conduct threat modeling, approve security scans, validate compliance requirements, and help teams build security into features from the start rather than as an afterthought.

#### Responsibilities
- Conduct threat modeling and security design reviews for new features
- Review and approve security scan results before release
- Validate compliance with regulatory and organizational security standards
- Identify and track security remediation work
- Provide guidance on secure coding practices and architecture patterns
- Collaborate on incident response for security-related issues

#### Goals
- Prevent security vulnerabilities from reaching production
- Ensure features meet compliance and regulatory requirements
- Build a security-aware development culture
- Reduce security debt and legacy vulnerabilities

#### Typical Communication
- Security design reviews during planning phase
- Pre-release security scan sign-off
- Security incident response and post-mortems
- Security training and best practice guidance

#### Interactions
- **Developers**: Review code for security vulnerabilities and provide remediation guidance
- **Product Manager**: Communicate security trade-offs and compliance implications
- **Release Manager**: Gate releases on security scan results
- **Infrastructure/Platform**: Coordinate on platform security controls and secrets management

---

### UX Researcher / Design Lead

#### Role Summary
UX Researchers and Design Leads ensure features are usable, desirable, and solve real user problems. They conduct user research, provide design guidance, and validate that acceptance criteria adequately reflect user needs and usability requirements.

#### Responsibilities
- Conduct or advise on user research to validate problem statements
- Provide design guidance and review mockups/prototypes
- Review acceptance criteria for usability completeness
- Conduct usability testing with end users
- Identify and document user experience gaps and opportunities
- Advocate for user needs in trade-off discussions

#### Goals
- Ensure features are intuitive and discoverable
- Reduce user friction and support burden
- Align features with actual user workflows and mental models
- Maximize adoption and user satisfaction

#### Typical Communication
- Planning sessions to discuss user research findings
- Design review meetings with developers
- Usability testing reports and recommendations
- User feedback integration in retrospectives

#### Interactions
- **Product Manager**: Share research findings to inform prioritization and requirements
- **Developers**: Collaborate on implementation trade-offs that affect usability
- **QA/Testing**: Provide usability testing guidance and acceptance criteria
- **Customer Success**: Gather user feedback and pain points from support interactions

---

### Data Analyst

#### Role Summary
Data Analysts define, instrument, and validate success metrics for features. They instrument events, create dashboards, analyze experiments, and provide data-driven insights to inform decision-making and measure business impact.

#### Responsibilities
- Define measurable success metrics aligned with business goals
- Design and validate event schemas for proper instrumentation
- Create and maintain dashboards for metric tracking
- Conduct experiment analysis and A/B test interpretation
- Provide insights on user behavior and feature adoption
- Monitor metrics post-launch and identify trends or anomalies

#### Goals
- Enable data-driven decision-making across the organization
- Ensure features deliver measurable business value
- Reduce guesswork in prioritization and release decisions
- Build institutional knowledge of what drives outcomes

#### Typical Communication
- Weekly metric reviews in product/execution syncs
- Experiment results and statistical analysis reports
- Dashboard and data visualization presentations
- Post-launch metric reviews and retrospectives

#### Interactions
- **Product Manager**: Align on success metrics and business KPIs
- **Developers**: Guide on event instrumentation and data collection best practices
- **Observability Engineer**: Coordinate on metric definitions and dashboard creation
- **Stakeholders**: Present data insights and outcomes to leadership

---

### Technical Writer / Documentation Owner

#### Role Summary
Technical Writers ensure comprehensive documentation exists for features, processes, and operations. They own user-facing documentation, internal runbooks, release notes, and onboarding materials to reduce confusion and support burden.

#### Responsibilities
- Write and maintain user-facing documentation and help content
- Author and update internal runbooks and operational procedures
- Create comprehensive release notes with migration steps
- Maintain FAQ and troubleshooting guides
- Ensure onboarding materials are current and accessible
- Review technical accuracy of documentation

#### Goals
- Reduce support burden through clear, accessible documentation
- Enable users and operators to self-serve and troubleshoot
- Ensure consistent terminology and documentation standards
- Accelerate onboarding and reduce time-to-productivity

#### Typical Communication
- Documentation reviews with developers and subject matter experts
- Release coordination for release notes and announcements
- Documentation planning during project planning phase
- Support feedback integration for documentation improvements

#### Interactions
- **Developers**: Validate technical accuracy and gather feature details
- **Product Manager**: Understand audience and scope of documentation
- **Release Manager**: Coordinate release notes and deployment procedures
- **Support/Customer Success**: Gather user questions and documentation gaps

---

### Platform / Tooling Engineer

#### Role Summary
Platform and Tooling Engineers own CI/CD infrastructure, developer tooling, and platform reliability aspects that impact all team members' ability to deliver. They ensure efficient builds, reliable deployments, and robust internal tools.

#### Responsibilities
- Design, maintain, and improve CI/CD pipelines and deployment automation
- Provide guidance on performance, scalability, and reliability trade-offs
- Manage platform changes and infrastructure updates
- Monitor and improve build/test/deploy cycle times
- Support local development environment setup and troubleshooting
- Collaborate on performance optimization and capacity planning

#### Goals
- Minimize build, test, and deployment cycle times
- Ensure reliable, predictable CI/CD infrastructure
- Enable developers to be productive with high-quality tooling
- Reduce operational friction and toil

#### Typical Communication
- Infrastructure status reports and planned maintenance announcements
- Performance review and optimization planning meetings
- Tool adoption and training for new platform changes
- Incident response for CI/CD failures

#### Interactions
- **Developers**: Support efficient local development and CI/CD troubleshooting
- **Release Manager**: Ensure reliable deployment automation and rollback procedures
- **Observability Engineer**: Instrument CI/CD for visibility into build/deploy performance
- **Security Reviewer**: Implement security controls and secrets management in pipelines

---

### Customer Success / Support Liaison

#### Role Summary
Customer Success and Support Liaisons bridge the gap between engineering and customers. They represent customer needs during planning, flag customer-impacting requirements, and ensure support teams and customers are prepared for feature releases.

#### Responsibilities
- Flag customer-impacting requirements and pain points during planning
- Prepare support runbooks and troubleshooting guides pre-release
- Communicate major changes and migration steps to customers
- Gather customer feedback on features and usability
- Participate in release planning to identify customer communication needs
- Triage and escalate customer issues to engineering teams

#### Goals
- Reduce support burden and customer confusion through proactive communication
- Ensure customer needs are represented in product decisions
- Accelerate customer adoption and success with new features
- Build strong customer relationships and satisfaction

#### Typical Communication
- Planning sessions to identify customer-impacting changes
- Release coordination meetings to plan customer communication
- Support runbook reviews and training
- Customer feedback summaries and trends

#### Interactions
- **Product Manager**: Share customer feedback to inform prioritization
- **Release Manager**: Coordinate customer communication and announcements
- **Developers**: Help identify edge cases and usability issues from support interactions
- **QA/Testing**: Provide acceptance criteria based on common customer scenarios

---

## How these personas are used in the exercise

- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When encountering responsibilities not clearly assigned, reference this document to identify the appropriate owner.
- Use these persona descriptions to facilitate cross-functional communication and accountability in project retrospectives.
