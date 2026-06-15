# Process Improvements — Checklists & Templates

This file contains practical checklists and templates to support the new personas and improve clarity on handoffs and responsibilities. Add or adapt items for your team's needs.

---

## Release Manager — Release Checklist (template)

Pre-release
- [ ] Confirm all PRs merged for this release scope
- [ ] Verify CI green and security scan baseline
- [ ] Confirm database migration plan and backup status (if applicable)
- [ ] Validate rollback/runbook is documented and tested
- [ ] Coordinate and confirm smoke-test owners and test plan
- [ ] Communicate release window and impact to stakeholders and support
- [ ] Confirm feature flag plan for staged rollouts (if used)

Deployment
- [ ] Execute deployment steps in pipeline
- [ ] Run smoke tests and verify critical flows
- [ ] Monitor metrics/dashboards for regressions for X minutes/hours
- [ ] Capture deploy artifacts and notes

Post-release
- [ ] Confirm post-deploy verification results
- [ ] Update status in the release tracker and notify stakeholders
- [ ] Close release checklist items and document any follow-ups

Notes:
- Link to runbooks and backout plans.
- Attach telemetry checks (who validates, where to find dashboards).

---

## Technical Program Manager (TPM) — Integration/Dependency Checklist

Planning
- [ ] Identify all dependent teams and owners
- [ ] Create/maintain dependency tracker with owners and due dates
- [ ] Schedule integration checkpoints and tech syncs
- [ ] Identify shared resources or risk (e.g., infra, APIs)

Execution
- [ ] Confirm interface contracts and versioning approach
- [ ] Track integration test results and blocker status
- [ ] Drive cross-team retrospectives for integration learnings

Escalation
- [ ] Escalate unresolved blockers to Product Lead / PM
- [ ] Document mitigation and contingency plans

---

## QA Lead — Test Plan Template

- Feature / Release name:
- Scope:
- Test owner:
- Test environments:
- Automated tests to run:
- Manual testing areas and owners:
- Critical acceptance criteria:
- Known gaps / limitations:
- Sign-off requirements:

---

## Security Reviewer — Pre-merge Checklist

- [ ] Threat model reviewed for the change
- [ ] Dependency and third-party risk assessed
- [ ] Static/dynamic scans passed or mitigations documented
- [ ] Secrets & access review completed
- [ ] Security owner has signed off or next steps recorded

---

## Measurement / Data — Post-release Validation Checklist

- [ ] Instrumentation implemented and reviewed
- [ ] Metrics queries validated on staging (if possible)
- [ ] Dashboards updated with new metrics
- [ ] Data owner verifies expected signals post-release
- [ ] Any data migration or backfill plan documented

---

## Support / On-call Liaison — Incident Handoff Template

- Incident title:
- Severity:
- Time observed:
- Current status:
- Primary owner:
- Immediate mitigation taken:
- Next steps & owners:
- Customer-facing communications (if any):
- Post-incident retrospective owner & schedule

---

## How to use these templates
- Copy the relevant checklist to the pertinent docs or the release issue for each release.
- Assign owners & due dates in the project board or release issue.
- Update checklists based on team retrospectives to make them actionable.
