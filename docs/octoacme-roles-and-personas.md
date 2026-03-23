# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

> **Role name synonyms used across docs:**
> - *Project Manager* = PM
> - *Product Manager* = PdM = Product Lead
> See the [Role Interactions guide](octoacme-role-interactions.md) for a quick "who to talk to for what" reference.

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

### Interactions
- **Project Manager (PM):** surface blockers, update task status, estimate work
- **Product Manager (PdM):** clarify acceptance criteria and scope
- **DevOps Engineer:** coordinate CI/CD pipeline changes and environment needs
- **Security Lead:** address vulnerability findings and follow secure-coding guidance
- **UX Designer:** review designs and discuss implementation feasibility

---

## Product Managers

### Role Summary
Product Managers (PdM / Product Lead) define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

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

### Interactions
- **Project Manager (PM):** align on scope, timelines, and priorities
- **Developers:** define acceptance criteria and resolve scope questions
- **UX Designer:** shape user flows and validate designs against requirements
- **Data Analyst:** review metrics and inform roadmap decisions
- **Support / Customer Success:** gather user feedback and issue patterns

---

## Project Managers

### Role Summary
Project Managers (PM) coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

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

### Interactions
- **Product Manager (PdM):** align scope and priorities weekly
- **DevOps Engineer:** coordinate release windows and production incident response
- **Security Lead:** escalate security risks and track remediation
- **All roles:** facilitate retrospectives and ensure action items are owned

---

## DevOps Engineer

### Role Summary
DevOps Engineers own the build, release, and infrastructure pipeline. They ensure code moves from development to production safely, reliably, and repeatably.

### Responsibilities
- Design and maintain CI/CD pipelines and automated deployment workflows
- Manage infrastructure, environments (dev, staging, production), and observability tooling
- Coordinate and execute production deployments and rollbacks
- Respond to and resolve infrastructure and production incidents
- Enforce infrastructure-as-code and environment consistency

### Goals
- Reduce deployment friction and mean time to recovery (MTTR)
- Increase deployment frequency and reliability
- Ensure all environments are reproducible and auditable

### Typical Communication
- Deployment schedule updates to PM and stakeholders
- Incident notifications and post-incident summaries
- Pipeline status and infrastructure change notifications

### Interactions
- **Project Manager (PM):** confirm deployment windows, communicate production incidents
- **Developers:** review pipeline requirements, support local environment parity
- **Security Lead:** apply security controls in pipelines (SAST, secret scanning, dependency scanning)
- **Support / Customer Success:** provide incident status updates during production outages

### Lifecycle Involvement
- **Initiation/Planning:** advise on infrastructure requirements and deployment strategy
- **Execution:** maintain CI health, unblock pipeline failures
- **Release:** execute deployment checklist, monitor post-deploy health
- **Retrospective:** contribute to post-incident reviews and process improvements

---

## UX Designer

### Role Summary
UX Designers create intuitive user experiences through research, wireframes, and prototypes. They advocate for end users throughout the product lifecycle.

### Responsibilities
- Conduct user research and synthesize findings into design requirements
- Produce wireframes, prototypes, and design specifications
- Facilitate usability testing and communicate insights to the team
- Maintain design system consistency across the product
- Review implemented features for design fidelity

### Goals
- Reduce friction and improve user satisfaction
- Ensure features are accessible and inclusive
- Bridge user needs with engineering feasibility

### Typical Communication
- Design reviews with Developers and Product Manager
- Usability test reports shared with stakeholders
- Design handoff notes and annotations in design files

### Interactions
- **Product Manager (PdM):** align designs to product requirements and business goals
- **Developers:** discuss implementation constraints and review built features
- **Data Analyst:** use usage data to inform and validate design decisions
- **Support / Customer Success:** incorporate user feedback and pain points into designs

### Lifecycle Involvement
- **Initiation:** define user problem and identify user research needs
- **Planning:** produce wireframes and design specs for backlog items
- **Execution:** support developers during implementation; run usability tests
- **Release:** verify design fidelity before launch
- **Retrospective:** review user feedback gathered post-release

---

## Security Lead

### Role Summary
The Security Lead defines and enforces security standards, reviews the system for vulnerabilities, and leads the response to security incidents.

### Responsibilities
- Define security requirements and threat model for the project
- Review releases and code changes for security vulnerabilities
- Own the security incident response process
- Advise on regulatory and compliance requirements (e.g., data privacy)
- Track and drive remediation of security findings

### Goals
- Prevent security incidents through proactive controls
- Reduce vulnerability exposure and remediation time
- Ensure the team understands and follows secure-coding practices

### Typical Communication
- Security findings reported to PM and PdM with risk ratings
- Security review sign-off as part of pre-release checklist
- Incident notifications and post-incident reports

### Interactions
- **Developers:** communicate vulnerability findings; review fixes before re-release
- **DevOps Engineer:** integrate security tooling (SAST, dependency scanning) into CI/CD
- **Project Manager (PM):** escalate security risks; ensure remediation is tracked
- **Product Manager (PdM):** advise on regulatory requirements that affect scope

### Lifecycle Involvement
- **Initiation:** flag regulatory or compliance constraints early
- **Planning:** add security requirements to acceptance criteria
- **Execution:** perform ongoing security reviews; respond to scan findings
- **Release:** sign off on security pre-release checklist
- **Retrospective:** review security incidents and recommend process improvements

---

## Data Analyst

### Role Summary
Data Analysts collect, analyze, and communicate key metrics that inform product decisions and measure project outcomes.

### Responsibilities
- Define and instrument metrics aligned to project success criteria
- Build and maintain dashboards and reports for stakeholders
- Analyze trends and surface actionable insights
- Support A/B testing and feature-impact measurement
- Ensure data quality and integrity across pipelines

### Goals
- Enable data-driven decision making across the team
- Reduce time to insight for product and leadership
- Ensure reliable, trustworthy data for reporting

### Typical Communication
- Weekly metrics summaries to Product Manager and stakeholders
- Ad-hoc analysis requests from PM, PdM, or leadership
- Data quality and anomaly alerts

### Interactions
- **Product Manager (PdM):** translate business questions into measurable metrics
- **Developers:** coordinate instrumentation, data pipeline integration
- **Project Manager (PM):** provide data to support status reports and risk assessments
- **UX Designer:** share usage data to guide design decisions
- **Support / Customer Success:** provide analysis of issue patterns and user behavior

### Lifecycle Involvement
- **Initiation:** define success metrics for the project one-pager
- **Planning:** ensure tracking instrumentation is included in scope
- **Execution:** monitor early metrics signals and flag anomalies
- **Release:** validate data pipelines are live and dashboards are updated
- **Retrospective:** present outcomes data to inform retrospective discussion

---

## Support / Customer Success

### Role Summary
Support and Customer Success team members are the direct interface between OctoAcme and its users. They gather feedback, coordinate issue resolution, and ensure users are set up for success.

### Responsibilities
- Provide first-line response to user-reported issues
- Document recurring issues, workarounds, and escalation paths
- Gather and channel user feedback to Product and Project Managers
- Coordinate communication to users during incidents
- Contribute to user-facing documentation and onboarding materials

### Goals
- Reduce time-to-resolution for user issues
- Build user confidence and satisfaction
- Ensure the team hears the voice of the customer

### Typical Communication
- Incident updates and resolution notes to users
- Regular feedback summaries to Product Manager
- Escalation tickets or Slack messages to Developers and PM

### Interactions
- **Product Manager (PdM):** deliver user feedback and feature requests
- **Project Manager (PM):** escalate critical user-impacting issues
- **Developers:** report reproducible bugs and validate fixes
- **DevOps Engineer:** stay informed on production incidents; relay status to users
- **UX Designer:** share user pain points and accessibility observations

### Lifecycle Involvement
- **Initiation:** provide customer context and known pain points
- **Planning:** review user-facing acceptance criteria and documentation needs
- **Execution:** review release notes and prepare support documentation
- **Release:** verify user-facing comms are sent; monitor early feedback
- **Retrospective:** report on user-facing impact; suggest improvements

---

## RACI Summary

Use this table as a lightweight guide to accountability across key project activities.
R = Responsible | A = Accountable | C = Consulted | I = Informed

| Activity | PM | PdM | Developer | DevOps | UX Designer | Security Lead | Data Analyst | Support |
|---|---|---|---|---|---|---|---|---|
| Project Charter / One-pager | R/A | C | C | I | C | C | C | I |
| Backlog Prioritization | C | R/A | C | I | C | I | C | I |
| Sprint Planning | R/A | C | R | I | C | I | I | I |
| Architecture & Technical Design | I | C | R/A | C | I | C | I | I |
| UX Design & Usability | I | C | C | I | R/A | I | C | C |
| Security Review | C | C | C | C | I | R/A | I | I |
| CI/CD & Deployments | C | I | C | R/A | I | C | I | I |
| Metrics & Dashboards | C | C | C | I | C | I | R/A | C |
| Release Communication | R/A | C | I | C | I | I | I | C |
| Incident Response (Production) | C | I | C | R/A | I | C | I | I |
| Incident Response (Security) | C | C | C | C | I | R/A | I | I |
| Retrospectives | R/A | C | C | C | C | C | C | C |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [octoacme-role-interactions.md](octoacme-role-interactions.md) for a quick "who to talk to for what" reference.

