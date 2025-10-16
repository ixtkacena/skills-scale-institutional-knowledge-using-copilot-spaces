# OctoAcme Project Lifecycle & Delivery Process

## Project Lifecycle

OctoAcme follows a lightweight, iterative project lifecycle designed to help cross-functional teams deliver customer value quickly and safely. The lifecycle consists of the following stages:

1. **Initiation**
    - Capture a one-pager that defines:
        - The problem
        - Measurable success metrics
        - Stakeholders
        - High-level timeline
2. **Planning**
    - Develop:
        - Prioritized backlog
        - Estimates
        - Definition of Done
        - Release plan
3. **Execution**
    - Conduct:
        - Sprints
        - Reviews
        - Demos
4. **Release**
    - Perform:
        - Staged deployments
        - Smoke checks
5. **Close & Retrospective**
    - Document learnings and next steps

**Core Artifacts:**
- Project Charter / One-pager
- Roadmap / Release Plan
- Sprint Backlog
- Acceptance Criteria and Definition of Done
- Risk Register
- Retrospective notes

## Day-to-Day Workflow

- The project board is the team’s single source of truth.
- **Board States:**

  | State         | Description                |
  |---------------|----------------------------|
  | Backlog       | Unprioritized work         |
  | Ready         | Prioritized, ready to start|
  | In Progress   | Actively being worked on   |
  | In Review     | Awaiting code review       |
  | QA            | Undergoing QA validation   |
  | Done          | Completed and accepted     |

- **Backlog items** follow a consistent template:
    - Title
    - Description
    - Acceptance criteria
    - Priority
    - Estimate
    - Owner
- Planning is timeboxed to the sprint length, with capacity considered.
- **Pull request workflow:**
    - Keep PRs small when possible (guideline: ≤ 400 lines)
    - Include the linked issue and acceptance criteria
    - Run CI (tests, linting, security scans) before requesting review
    - Require approval before merging

## Roles and Responsibilities

- **Project Managers (PM):**
    - Coordinate delivery, schedules, risks, and communications
- **Product Managers (PdM):**
    - Own outcomes, prioritization, and success metrics
- **Developers:**
    - Build and test features
- **QA:**
    - Validate acceptance

## Risk and Dependency Management

- Teams maintain a **Risk Register** reviewed in weekly syncs.
- Escalate risks per documented paths when needed.

**Risk Register Fields:**

| ID | Impact | Likelihood | Owner | Mitigation |
|----|--------|------------|-------|------------|
|    |        |            |       |            |

## Communication Cadence

- Daily standups
- Weekly delivery syncs
- PM ↔ PdM weekly alignment
- Monthly stakeholder updates
- Scheduled demos
- Templates for weekly status and incident communications

## Quality Assurance

Quality assurance blends automated and manual checks to keep releases safe and observable.

- Teams write unit and integration tests
- Run end-to-end smoke tests for critical flows
- Include security scanning in CI
- Perform manual QA for acceptance when necessary

**Pre-release gates require:**
- Passing CI and security scans
- Drafted release notes
- A rollback/mitigation plan
- Prepared smoke tests

**Deployments:**
- Favor automated pipelines
- Include post-deploy verifications
- Stakeholder announcements
