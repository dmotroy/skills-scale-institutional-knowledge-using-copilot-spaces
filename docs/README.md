# OctoAcme Project Management Docs

Welcome! This repository centralizes the project management knowledge, processes, and best practices used by OctoAcme. It serves as a single source of truth for how we plan, execute, release, and continuously improve our initiatives — making processes searchable, versioned, and consistently applied across all teams.

## Project Management Process Overview

OctoAcme runs projects through a lightweight, repeatable lifecycle: **Initiation** → **Planning** → **Execution** → **Release** → **Close/Retrospective**. Each phase has defined artifacts and decision gates to ensure clarity and alignment before moving forward. Core artifacts include a project charter/one-pager, a prioritized backlog with acceptance criteria, a risk register, and retrospective action items that feed continuous improvement back into the process docs.

Roles are clearly defined to reduce ambiguity and ensure ownership at every stage. A **Project Manager (PM)** coordinates delivery mechanics — timelines, risks, communications, and meeting facilitation — while a **Product Manager (PdM)** owns outcomes, prioritizes the backlog, and measures impact. **Developers** design and implement features, collaborate on estimation, and maintain tests and documentation; **QA/Testing** validates acceptance criteria and quality; and **Stakeholders** provide input and approvals throughout the lifecycle.

Execution is managed with a steady team rhythm and transparent workflow tracking. Teams use daily standups and weekly delivery syncs to surface progress, blockers, and dependencies, supported by a project board workflow (Backlog → Ready → In Progress → In Review → QA → Done). Communication favors a single source of truth for status, with a simple weekly status update format covering progress, next steps, risks/blockers, and decisions needed. Risk management follows a defined lifecycle (identify, assess, mitigate, monitor) with escalation paths that move from team triage to PM/Product Lead and up to sponsor-level escalation when business impact warrants it.

Quality assurance is built into both development and release practices. OctoAcme encourages small pull requests linked to issues and acceptance criteria, with CI (tests, lint, security scanning) passing before review and at least one approval required per team policy. Testing expectations span unit tests for new logic, integration tests where needed, and end-to-end smoke tests for critical flows — plus manual QA for feature acceptance when appropriate. Releases require readiness checks (acceptance criteria met, scans passing, release notes and rollback plan prepared), followed by staged deployment, post-deploy verification, and stakeholder announcements; failures trigger rollback/incident response and a blameless retrospective with tracked action items.

## Process Documentation

- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning Guide](octoacme-project-planning.md)
- [Execution & Tracking Guide](octoacme-execution-and-tracking.md)
- [Risk Management & Communication Guide](octoacme-risks-and-communication.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement Guide](octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas Reference](octoacme-roles-and-personas.md)
