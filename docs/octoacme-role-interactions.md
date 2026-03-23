# OctoAcme — Role Interactions Guide

## Purpose
A quick "who to talk to for what" reference so team members spend less time figuring out the right person and more time executing.

> For full role descriptions and responsibilities, see [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md).

---

## Quick Reference: Who to Talk to for What

| Situation | Primary Contact | Also Involve |
|---|---|---|
| Feature scope or priority change | Product Manager (PdM) | Project Manager (PM) |
| Timeline, milestone, or schedule question | Project Manager (PM) | PdM |
| Deployment window or pipeline issue | DevOps Engineer | PM |
| Production incident | DevOps Engineer | PM, Support |
| Security vulnerability finding | Security Lead | Developers, PM |
| Security incident | Security Lead | PM, DevOps Engineer |
| UX/design clarification | UX Designer | PdM, Developers |
| Usability feedback from users | UX Designer | Support / Customer Success |
| Metrics, dashboards, or data questions | Data Analyst | PdM |
| User-reported bug or complaint | Support / Customer Success | Developers, PM |
| Regulatory or compliance requirement | Security Lead | PdM, PM |
| Onboarding / user documentation | Support / Customer Success | PdM, UX Designer |
| Retrospective action item | Project Manager (PM) | All |

---

## Key Interaction Patterns

### Product Manager ↔ UX Designer
The Product Manager provides business requirements and success metrics; the UX Designer translates them into user flows and designs. They sync frequently during planning and execution to ensure design decisions are grounded in product goals.

### Developers ↔ DevOps Engineer
Developers rely on DevOps for environment parity and pipeline support. DevOps relies on Developers to build deployable, testable artifacts. They collaborate on CI configuration, build failures, and release readiness.

### Developers ↔ Security Lead
Security Lead reviews code and dependencies for vulnerabilities and communicates findings with severity ratings. Developers own remediation. The Security Lead re-reviews fixes before the next release.

### Project Manager ↔ All Roles
The Project Manager is the coordination hub — they do not own the work but ensure it is visible, prioritized, and unblocked. Any cross-team dependency or escalation goes through or is at minimum communicated to the PM.

### Support / Customer Success ↔ Product Manager
Support channels real user feedback and issue patterns to the Product Manager, who uses this input for backlog prioritization. Support also ensures user-facing communications and documentation are accurate before and after releases.

---

## Escalation Path Summary

```
User Issue → Support / Customer Success → PM → PdM → Sponsor
Production Incident → DevOps Engineer → PM → Sponsor
Security Incident → Security Lead → PM → PdM / Legal / Sponsor
Design Disagreement → UX Designer → PdM → PM
Data/Metric Discrepancy → Data Analyst → PdM → PM
```

---

## Cross-functional Touch Points by Lifecycle Phase

| Phase | Key Interactions |
|---|---|
| **Initiation** | PdM defines goals; PM sets up structure; Security Lead flags constraints; Data Analyst defines metrics; Support shares user context |
| **Planning** | PM facilitates kickoff; UX Designer produces specs; DevOps advises on infrastructure; Security Lead adds security requirements |
| **Execution** | Developers build; DevOps maintains pipelines; Security Lead reviews; UX Designer validates; Data Analyst monitors signals |
| **Release** | DevOps deploys; Security Lead signs off; Support prepares comms; PM announces; Data Analyst validates tracking |
| **Retrospective** | PM facilitates; Data Analyst presents outcomes; Support shares user impact; all roles contribute improvements |
