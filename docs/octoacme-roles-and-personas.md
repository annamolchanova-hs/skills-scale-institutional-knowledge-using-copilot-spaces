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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas (proposed additions)

Purpose: capture operational and cross-functional roles that commonly appear in delivery, clarify responsibilities, and make handoffs explicit.

### Technical Program Manager (TPM)
Role summary
- TPMs coordinate cross-team technical dependencies and drive technical program execution across multiple teams.

Responsibilities
- Coordinate cross-team technical dependencies and integration plans.
- Run technical planning sessions and syncs.
- Maintain dependency trackers and integration timelines.
- Monitor technical risks and surface them to Product Lead / PM.
- Facilitate architectural decisions and alignment across teams.

Interactions / Handoffs
- Works closely with Product Manager to translate product priorities into technical milestones.
- Partners with Project Manager to align schedules and dependencies.
- Escalates unresolved cross-team blockers to Product Lead.

Example scenarios
- Coordinating a multi-team integration requiring interface changes across services.
- Leading a migration that spans multiple squads.

---

### Release Manager
Role summary
- Owns release readiness and execution for a release window, ensuring gating criteria and communications are met.

Responsibilities
- Plan release windows and gates.
- Validate rollback/runbook readiness and coordinate rehearsals when needed.
- Coordinate release tasks across Dev, QA, and Ops.
- Ensure release checklist items (pre- and post-deploy) are complete.
- Lead post-release verification activities and capture outcomes.

Interactions / Handoffs
- Coordinates with Developers and QA for gating and smoke tests.
- Communicates release timing and impact to stakeholders and support teams.
- Works with Project Manager to schedule deployments and resolve cross-team conflicts.

Example scenarios
- Managing a minor release with database migrations and coordinated feature flags.
- Running a canary rollout and leading verification.

---

### QA Lead / Test Engineer (distinct persona)
Role summary
- Owns test strategy and quality validation for major features and releases.

Responsibilities
- Define test strategies and acceptance criteria for features.
- Draft and maintain test plans for significant releases.
- Coordinate manual QA and test environment readiness.
- Track and validate test coverage and test automation gaps.

Interactions / Handoffs
- Works with Developers to refine acceptance criteria and prevent regressions.
- Partners with PM to prioritize testing scope for releases.
- Escalates critical quality risks to Project Manager and Product Lead.

Example scenarios
- Leading test planning for a complex integration involving several services.
- Coordinating exploratory testing for user-facing changes.

---

### Security Representative / Security Reviewer
Role summary
- Represents security in the planning and review process, ensuring appropriate threat modeling and mitigations.

Responsibilities
- Perform threat modeling for new features or architectural changes.
- Approve security-related changes and check required scan passes.
- Recommend security mitigations and validate fixes.
- Ensure compliance requirements are considered during planning.

Interactions / Handoffs
- Engages during planning and design reviews; participates in PR reviews for security-relevant changes.
- Works with Developers and TPMs to balance risk and delivery timelines.
- Notifies Product and Project Managers when security review findings impact scope or timelines.

Example scenarios
- Reviewing a public API change for potential data exposure.
- Conducting an architecture-level threat modeling session for a new integration.

---

### Data Analyst / Measurement Owner
Role summary
- Owns success metrics and measurement strategy for features and releases.

Responsibilities
- Define clear success metrics and instrumentation needs.
- Work with Engineers to implement telemetry and validate data collection.
- Analyze post-release data to confirm outcomes.
- Recommend product changes based on measurement results.

Interactions / Handoffs
- Partners with Product Manager to specify measurable outcomes and SLIs.
- Works with Developers to ensure instrumentation is implemented and tested.
- Communicates findings to stakeholders and feeds insights into backlog prioritization.

Example scenarios
- Defining experiment and metric instrumentation for an A/B test.
- Validating telemetry after a release to ensure feature adoption is tracked.

---

### Support / On-call Liaison
Role summary
- Bridges support/operations and the delivery team to ensure runbooks, triage, and feedback loops are maintained.

Responsibilities
- Represent support and operational constraints during planning.
- Triage post-release issues and coordinate fixes with the delivery team.
- Feed incident learnings back into the roadmap and risk register.
- Maintain prioritized backlog of operational fixes and customer-facing issues.

Interactions / Handoffs
- Works with PM/Project Manager to prioritize post-release fixes.
- Collaborates with Developers during incident response.
- Coordinates incident communication with stakeholders and customers.

Example scenarios
- Coordinating triage and communication during a Sev1 incident.
- Prioritizing a recurring customer-facing bug discovered by support.

---

### UX Researcher / Designer
Role summary
- Owns user research and design validation to ensure usability and product fit.

Responsibilities
- Plan and conduct user research and usability testing.
- Produce design deliverables and ensure design handoff quality.
- Define UX-related acceptance criteria and validate outcomes.
- Collaborate on accessibility checks and usability improvements.

Interactions / Handoffs
- Partners with Product Manager on problem definition and validation.
- Works with Developers to ensure designs are implementable and tested.
- Shares research findings with stakeholders to influence prioritization.

Example scenarios
- Running rapid usability tests for a new checkout flow.
- Working with PM and Devs to iterate on designs after beta feedback.

---

## Implementation notes / cross-links
- Add an "Additional Personas" section header for easy navigation (done above).
- Link each persona to related process documents:
  - Release Manager -> docs/octoacme-release-and-deployment.md (release checklist/process)
  - TPM -> docs/octoacme-project-planning.md (dependencies & planning)
  - QA Lead -> docs/octoacme-execution-and-tracking.md (testing & CI)
  - Security Representative -> security/process (if a security runbook exists) or add cross-link to CI/security scanning docs
  - Data Analyst -> reporting & metrics sections in docs/octoacme-execution-and-tracking.md
  - Support Liaison -> docs/octoacme-release-and-deployment.md and docs/octoacme-risks-and-communication.md

- Add short examples / contact templates where useful (optional).
- Consider adding a quick lookup table mapping persona -> primary doc(s) -> typical contact for each project type.
