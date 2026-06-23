# OctoAcme Project Management Docs

This README provides a short summary of OctoAcme's project management processes and links to detailed process documents in this folder.

## OctoAcme Project Management Overview

OctoAcme follows a structured, iterative project lifecycle organized into five key phases: **Initiation**, **Planning**, **Execution**, **Release**, and **Continuous Improvement**. 

During **Initiation**, teams validate business needs and create a lightweight Project One-pager that defines the problem statement, objectives, success metrics, stakeholders, and resource requirements. The **Planning** phase transforms approved initiatives into actionable backlogs by breaking work into shippable increments, estimating scope using T-shirt sizing or story points, and establishing a Definition of Done. **Execution** emphasizes small, testable PRs (≤400 lines), automated CI/CD with tests and linting, and daily standups focused on progress and blockers. **Release** standardizes deployment through pre-release requirements including passing CI, security scans, smoke testing, and rollback plans. Finally, **retrospectives** capture learnings and convert them into tracked action items, fostering continuous improvement.

### Core Roles & Communication

OctoAcme operates with clearly defined roles: **Project Managers** coordinate schedules, risks, and cross-team communication; **Product Managers** own prioritization, success metrics, and user value; **Developers** implement features while collaborating on design and testability; **QA** validates quality and acceptance criteria; and **Stakeholders** provide inputs and approvals. 

Communication follows a structured cadence with daily standups (15 min) focused on progress and blockers, weekly PM-PdM syncs, twice-weekly team standups, monthly stakeholder updates, and ad-hoc escalations as needed. Risk escalation is tiered: Level 1 involves team-level triage in standups, Level 2 escalates to PM and Product Lead, and Level 3 reaches sponsor level for business-impacting issues.

### Quality Assurance & Key Artifacts

Quality is embedded throughout the OctoAcme process through unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA for feature acceptance. Key artifacts include the Project One-pager, prioritized backlog with acceptance criteria, Definition of Done, Risk Register, and Release Notes. Teams track velocity and burndown, monitor success metrics via dashboards, and use GitHub Projects for workflow management.

---

## Process Documents

Explore detailed guidance for each phase:

- **[OctoAcme Project Management Overview](octoacme-project-management-overview.md)** — Introduction to roles, principles, and high-level lifecycle
- **[OctoAcme — Project Initiation](octoacme-project-initiation.md)** — How to validate ideas and get stakeholder alignment
- **[OctoAcme — Project Planning](octoacme-project-planning.md)** — Backlog creation, estimation, and release planning
- **[OctoAcme — Execution & Tracking](octoacme-execution-and-tracking.md)** — Daily standups, PR workflow, quality standards, and progress tracking
- **[OctoAcme — Release & Deployment](octoacme-release-and-deployment.md)** — Pre-release checklist, deployment process, rollback, and incident response
- **[OctoAcme — Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)** — Running retrospectives and tracking action items
- **[OctoAcme — Risk Management & Communication](octoacme-risks-and-communication.md)** — Risk registers, escalation paths, and stakeholder updates
- **[OctoAcme — Roles and Personas](octoacme-roles-and-personas.md)** — Detailed definitions of team roles and responsibilities

---

## How to Use These Docs

- **New to OctoAcme?** Start with the overview above, then browse the Process Documents list.
- **Looking for templates?** Each detailed doc contains checklists, templates, and examples.
- **Want to update or add content?** Use the "[Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml)" issue template.
- **Need help with a specific phase?** Jump to the relevant document link above.

---

## Key Principles

- **Customer-first**: Prioritize customer value and usability
- **Iterative delivery**: Deliver small, testable increments
- **Clear ownership**: Each project has a named Project Manager and Product Lead
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback and learning
