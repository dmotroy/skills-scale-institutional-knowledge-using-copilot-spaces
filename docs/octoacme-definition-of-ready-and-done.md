# OctoAcme — Definition of Ready & Definition of Done

## Purpose
Provide clear, shared checklists that determine when a backlog item is ready to be worked on and when it is truly complete. This reduces rework, unblocks handoffs, and keeps quality consistent.

> Referenced from: [Project Planning](octoacme-project-planning.md) | [Execution & Tracking](octoacme-execution-and-tracking.md)

---

## Definition of Ready (DoR)
A backlog item is **Ready** to be pulled into a sprint when all of the following are true:

### Story / Feature
- [ ] Clear problem statement or user story written (`As a [user], I want [goal], so that [benefit]`)
- [ ] Acceptance criteria defined and agreed upon by PdM and Developers
- [ ] Dependencies identified and unblocked (or a plan exists to unblock them)
- [ ] UX designs or mockups available (if UI is involved)
- [ ] Security requirements noted (if the item touches auth, data, or APIs)
- [ ] Estimate provided (story points or T-shirt size)
- [ ] Item is small enough to complete within one sprint

### Bug Fix
- [ ] Steps to reproduce documented
- [ ] Expected vs. actual behavior described
- [ ] Severity/priority agreed upon (PM + PdM)
- [ ] Relevant logs, screenshots, or error details attached

---

## Definition of Done (DoD)
A backlog item is **Done** when all of the following are true:

### Code & Quality
- [ ] Code implemented and meets acceptance criteria
- [ ] Unit tests written and passing (covering new logic)
- [ ] Integration/end-to-end tests added or updated where applicable
- [ ] No new linting errors or warnings introduced
- [ ] Code reviewed and approved by at least one peer

### Security & Compliance
- [ ] Security scan (SAST / dependency scan) passing in CI
- [ ] No high- or critical-severity vulnerabilities introduced (or accepted with Security Lead sign-off)
- [ ] Sensitive data (secrets, PII) handled per security policy

### Documentation & Communication
- [ ] Inline code comments updated where needed
- [ ] User-facing documentation updated (if applicable)
- [ ] Release notes entry drafted (for features and significant fixes)
- [ ] PR description links to the issue and summarizes the change

### Deployment & Observability
- [ ] Feature tested in staging environment
- [ ] Monitoring/alerting configured for new functionality (if applicable)
- [ ] Rollback plan documented (for major features or risky changes)

---

## Pull Request (PR) Checklist
Use this before requesting a review:

- [ ] PR title is descriptive and references the issue number
- [ ] Description explains *what* changed and *why*
- [ ] Acceptance criteria from the issue are addressed
- [ ] CI is passing (tests, lint, security scans)
- [ ] PR is <= 400 lines changed (split if larger, when feasible)
- [ ] Self-reviewed the diff for unintended changes
- [ ] Relevant reviewers tagged (at minimum: one peer; Security Lead if touching auth/data)

---

## Notes
- The DoD applies to all items entering the **Done** column on the project board.
- Teams may customize this list per project, but the core security and test requirements are non-negotiable.
- Review and update this document during retrospectives if the team identifies friction points.
