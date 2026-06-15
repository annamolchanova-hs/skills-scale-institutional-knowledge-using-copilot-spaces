# OctoAcme Project Management Documentation

Welcome to the OctoAcme project management process documentation. This folder contains the complete guide for how OctoAcme runs projects from initiation through delivery, retrospective, and continuous improvement.

## Quick Start

New to OctoAcme? Start with [octoacme-project-management-overview.md](./octoacme-project-management-overview.md) for a high-level introduction to our approach, roles, and key artifacts.

## OctoAcme Project Management Overview

OctoAcme operates on a customer-first, iterative delivery model with clear ownership and data-informed decision-making. The organization follows a structured project lifecycle that spans initiation, planning, execution, release, and retrospective phases. Central to this approach are three key roles—**Project Manager** (coordinates delivery and timelines), **Product Manager** (defines outcomes and measures success), and **Developers** (implement features collaboratively)—supported by QA/Testing and Stakeholders. The framework emphasizes psychological safety, encouraging feedback and learning across teams while maintaining accountability through named owners and transparent communication.

### Key Workflows & Execution Practices

Projects begin with an **initiation phase** where a Project One-pager establishes business need, success metrics, stakeholders, and initial timeline—serving as the decision gate before planning proceeds. Once approved, the **planning phase** breaks work into shippable increments with prioritized backlogs, estimated scope, and a documented Definition of Done. During **execution**, teams follow a structured rhythm of daily 15-minute standups focusing on progress and blockers, weekly delivery syncs to review milestones and flag risks, and regular demos. The delivery workflow emphasizes small PRs (≤400 lines), automated CI/CD including tests and security scanning, and at least one approval before merging. Risk management is ongoing, with a Risk Register maintained and reviewed at weekly syncs.

### Quality, Release, & Communication Standards

Quality assurance spans unit tests for new logic, integration tests where applicable, end-to-end smoke tests before release, and security scanning in CI pipelines. Before **deployment**, teams verify all acceptance criteria are met, CI and security scans pass, release notes are drafted, and a rollback plan is documented. The communication cadence includes weekly syncs between PM and Product Manager, twice-weekly standups for the delivery team, monthly stakeholder updates, and ad-hoc escalations. Escalation follows a clear three-level path: team-level triage in standup, PM escalation to Product Lead and dependent teams, and sponsor-level escalation for business-impacting issues.

### Continuous Improvement & Knowledge Management

OctoAcme institutionalizes learning through blameless post-incident retrospectives and structured action item tracking integrated into project backlogs. Process knowledge is centralized in versioned documentation, reducing single-person dependency, accelerating onboarding, and ensuring consistent, repeatable project execution. Teams measure the impact of improvements and celebrate successes, embedding a culture where small, iterative changes drive continuous evolution of the project management practice.

## Documentation Index

### Core Process Documents

- **[octoacme-project-management-overview.md](./octoacme-project-management-overview.md)** — High-level overview of OctoAcme's approach, core roles, key artifacts, and how to use these documents
- **[octoacme-project-initiation.md](./octoacme-project-initiation.md)** — How to validate and authorize work, align stakeholders, and create a lightweight Project One-pager
- **[octoacme-project-planning.md](./octoacme-project-planning.md)** — Breaking work into shippable increments, creating backlogs with acceptance criteria, and identifying dependencies
- **[octoacme-execution-and-tracking.md](./octoacme-execution-and-tracking.md)** — Team rhythm (standups, syncs), pull request workflows, quality assurance, and blocker escalation
- **[octoacme-risks-and-communication.md](./octoacme-risks-and-communication.md)** — Risk register management, stakeholder communication templates, and escalation paths
- **[octoacme-release-and-deployment.md](./octoacme-release-and-deployment.md)** — Release types, pre-release requirements, deployment checklist, and rollback playbook
- **[octoacme-retrospective-and-continuous-improvement.md](./octoacme-retrospective-and-continuous-improvement.md)** — Running retrospectives, tracking improvements, and building a continuous improvement culture

### Reference Documents

- **[octoacme-roles-and-personas.md](./octoacme-roles-and-personas.md)** — Detailed descriptions of key roles (Developers, Product Managers, Project Managers), their responsibilities, goals, and typical communication patterns

## How to Use These Docs

1. **For new projects**: Follow the lifecycle in order—Initiation → Planning → Execution → Release → Retrospective
2. **For specific guidance**: Jump directly to the document that covers your current phase or question
3. **For process improvements**: Use the "Add Content to Project Management Process Docs" issue template in `.github/ISSUE_TEMPLATE/` to propose updates
4. **For context in Copilot Spaces**: These docs are designed to be attached to Copilot Spaces to provide role-specific guidance and process alignment

## Contributing to Process Documentation

Have feedback, identified a gap, or want to propose an improvement to our processes? Use the **[Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml)** issue template to:

- Request clarifications or additional examples
- Add new sections or checklists based on team learnings
- Incorporate best practices discovered during projects
- Close gaps identified during onboarding or retrospectives

All updates are reviewed for alignment with existing docs and validated with stakeholders before being incorporated.

## Version History

- **v1.0** (June 2026): Initial OctoAcme project management documentation suite with core processes for initiation, planning, execution, release, and continuous improvement
