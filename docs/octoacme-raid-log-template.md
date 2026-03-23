# OctoAcme — RAID Log Template

## Purpose
Track Risks, Assumptions, Issues, and Dependencies (RAID) in one place so the project team always has a current view of what could derail delivery.

> Referenced from: [Risk Management & Communication](octoacme-risks-and-communication.md) | [Project Planning](octoacme-project-planning.md)

---

## How to Use
- Create a copy of this template for each project (e.g., as a file in the project repo or as a GitHub Issue).
- Update the log at least weekly during the PM sync.
- Escalate items with **High** impact or items that remain unresolved for more than two sprints.

---

## Risks

Risks are potential future events that could negatively impact the project.

| ID | Description | Impact (H/M/L) | Likelihood (H/M/L) | Owner | Mitigation Plan | Status | Date Raised |
|---|---|---|---|---|---|---|---|
| R-001 | _Example: Key developer unavailable during release week_ | M | M | PM | Identify backup; document runbooks | Open | YYYY-MM-DD |
| R-002 | _Example: Security vulnerability in third-party dependency_ | H | L | Security Lead | Monitor CVE feeds; pin dependency versions | Monitoring | YYYY-MM-DD |

**Status values:** Open · Monitoring · Mitigated · Closed

---

## Assumptions

Assumptions are things the team is treating as true without confirmation. If an assumption proves false, it may become a risk or issue.

| ID | Assumption | Owner | Validation Method | Validated? | Date |
|---|---|---|---|---|---|
| A-001 | _Example: External API will remain backward-compatible through Q3_ | PdM | Confirm with vendor by sprint 2 | No | YYYY-MM-DD |
| A-002 | _Example: Staging environment mirrors production configuration_ | DevOps Engineer | Run environment comparison script | No | YYYY-MM-DD |

---

## Issues

Issues are problems that are actively impacting the project right now.

| ID | Description | Impact (H/M/L) | Owner | Action Plan | Target Resolution | Status | Date Raised |
|---|---|---|---|---|---|---|---|
| I-001 | _Example: CI pipeline failing intermittently on integration tests_ | M | DevOps Engineer | Investigate flaky test; add retry logic | YYYY-MM-DD | In Progress | YYYY-MM-DD |
| I-002 | _Example: Missing design specs for onboarding flow_ | H | UX Designer | Designer to deliver specs by sprint 3 kickoff | YYYY-MM-DD | Open | YYYY-MM-DD |

**Status values:** Open · In Progress · Resolved · Closed

---

## Dependencies

Dependencies are items or deliverables that this project relies on from other teams, systems, or external parties.

| ID | Description | Type | Dependency Owner | Needed By | Status | Notes |
|---|---|---|---|---|---|---|
| D-001 | _Example: Auth service API endpoint from Platform team_ | Internal | Platform PM | Sprint 3 start | On Track | Confirmed in last cross-team sync |
| D-002 | _Example: Compliance review from Legal_ | External | Security Lead | Pre-release | At Risk | Waiting on Legal scheduling |
| D-003 | _Example: Third-party payment SDK upgrade_ | External | Developer | Sprint 2 | Blocked | Vendor release delayed |

**Type values:** Internal (another team) · External (vendor/partner) · Technical (system/infra)
**Status values:** On Track · At Risk · Blocked · Complete

---

## Escalation Guidance

| Situation | Escalate To |
|---|---|
| High-impact risk with no mitigation plan | PM → PdM → Sponsor |
| Security risk (vulnerability, compliance gap) | Security Lead → PM → PdM |
| Production/infrastructure dependency blocked | DevOps Engineer → PM |
| External dependency delayed | PM → PdM → Sponsor |
| Assumption proven false | Owner → PM immediately |

---

## Change Log

| Date | Change Made | Updated By |
|---|---|---|
| YYYY-MM-DD | Initial log created | PM |
