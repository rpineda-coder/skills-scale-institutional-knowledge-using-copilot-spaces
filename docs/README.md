# OctoAcme Project Management Documentation

Welcome to the OctoAcme project management framework documentation. This centralized hub provides a complete guide to how OctoAcme runs projects—from initiation through retrospectives—enabling consistent, repeatable execution and accelerating onboarding for new team members.

---

## Overview

OctoAcme operates a structured five-phase project lifecycle designed to deliver customer value reliably while scaling institutional knowledge across the organization. The framework combines clear role definitions, consistent communication practices, embedded quality assurance, and systematic risk management to enable teams to deliver on commitments efficiently. Whether you're starting a new project, managing execution, or planning a release, these docs provide the playbook for success.

### Core Principles

- **Customer-first**: Prioritize customer value and usability in all decisions
- **Iterative delivery**: Deliver small, testable increments rather than monolithic releases
- **Clear ownership**: Each project has named leadership (PM, Product Manager) with explicit responsibilities
- **Data-informed decisions**: Measure impact and iterate based on evidence, not assumptions
- **Psychological safety**: Encourage feedback, learning, and continuous improvement without fear

---

## OctoAcme Project Management Processes Summary

### Lifecycle & Workflows

OctoAcme operates a structured five-phase project lifecycle: **Initiation**, **Planning**, **Execution**, **Release**, and **Close & Retrospective**. During **Initiation**, teams validate business need by creating a lightweight Project One-pager that captures the problem statement, success metrics, stakeholders, and resource needs. Once approved, the **Planning** phase breaks work into shippable increments with prioritized backlog items, acceptance criteria, and a Definition of Done. The **Execution** phase emphasizes iterative delivery through daily standups, weekly delivery syncs, and a GitHub Projects board with columns spanning Backlog → Ready → In Progress → In Review → QA → Done. Pull requests follow strict conventions (≤400 lines when possible) with automated testing, linting, and at least one approval before merging. **Release** requires passing CI/security scans, smoke testing in staging, and a documented rollback plan, followed by stakeholder announcements. Finally, teams hold **retrospectives** after each sprint or milestone to capture learnings and drive continuous improvement through prioritized action items.

### Core Roles & Communication Cadence

OctoAcme defines clear ownership through four primary personas: **Project Managers** coordinate delivery, manage schedules, risks, and communications; **Product Managers** define what to build, prioritize the backlog, and measure outcomes; **Developers** implement features, write tests, and identify technical risks; and **QA/Testing** validates quality against acceptance criteria. This clarity prevents silos and enables focused accountability. Communication is structured and consistent: teams conduct daily standups (15 min) focused on progress and blockers, weekly syncs between PM and Product Manager, twice-weekly delivery team standups, and monthly stakeholder updates. Ad-hoc escalation paths exist for blockers—escalating from team-level triage through the PM, Product Lead, and finally to the Sponsor for business-impacting issues. A single source of truth (project README or release doc) ensures all stakeholders access current status without confusion.

### Quality Assurance & Risk Management

Quality is embedded throughout execution via **unit tests** for new logic, **integration tests** where applicable, **end-to-end smoke tests** for critical flows before release, and **security scanning in CI**. Manual QA validates feature acceptance when needed. To manage uncertainty, OctoAcme maintains a **Risk Register** (updated weekly) capturing ID, description, impact, likelihood, owner, and mitigation plan. Risks are identified during planning and ongoing execution, assessed for priority, mitigated through proactive actions, and monitored at weekly syncs. The team uses **velocity and burndown tracking**, monitors **success metrics** defined in the Project One-pager, and leverages **dashboards** for key signals (errors, latency, usage). This data-informed approach enables evidence-based decisions and rapid iteration—core to OctoAcme's customer-first, psychological-safe culture.

---

## Project Lifecycle at a Glance

OctoAcme's five-phase approach ensures alignment, quality, and accountability:

1. **Initiation** — Validate business need, align stakeholders, create a lightweight Project One-pager
2. **Planning** — Break work into shippable increments, define acceptance criteria, identify risks and dependencies
3. **Execution** — Build and iterate with daily standups, weekly syncs, and continuous testing
4. **Release** — Deploy to production with smoke tests, rollback plans, and stakeholder communication
5. **Retrospective** — Capture learnings and convert them into actionable improvements

---

## Documentation Guide

### Foundation & Strategy

Start here to understand OctoAcme's overall approach and the core roles involved in every project.

- **[Project Management Overview](octoacme-project-management-overview.md)**  
  Introduction to OctoAcme's principles, core roles, key artifacts, and the high-level project lifecycle. Best for: getting oriented to the framework.

- **[Roles & Personas](octoacme-roles-and-personas.md)**  
  Detailed definitions of Developers, Product Managers, and Project Managers—their responsibilities, goals, and typical communications. Best for: understanding who owns what.

---

### Project Phases

Follow these guides as you move through each stage of a project from conception to completion.

- **[Project Initiation](octoacme-project-initiation.md)**  
  Steps to validate and authorize work, align stakeholders, and create a lightweight plan. Includes the Project One-pager template and initiation checklist. Best for: kicking off a new project or feature proposal.

- **[Project Planning](octoacme-project-planning.md)**  
  Turn an approved initiative into an actionable plan and backlog. Covers kickoff, backlog prioritization, estimation, Definition of Done, and risk/dependency identification. Best for: building your sprint roadmap.

- **[Execution & Tracking](octoacme-execution-and-tracking.md)**  
  Guidance for managing day-to-day execution and tracking progress toward milestones. Covers standups, pull request workflow, quality gates, and blocker escalation. Best for: keeping the team aligned and moving forward.

- **[Release & Deployment](octoacme-release-and-deployment.md)**  
  Standardized procedures for releasing features to production safely and reliably. Includes pre-release requirements, deployment checklist, rollback playbook, and release notes template. Best for: shipping with confidence.

---

### Supporting Processes

These guides address critical cross-cutting concerns that span the entire project lifecycle.

- **[Risk Management & Communication](octoacme-risks-and-communication.md)**  
  How to identify, assess, monitor, and mitigate risks. Covers the Risk Register, escalation paths, stakeholder communication strategies, and incident response. Best for: staying ahead of blockers and keeping everyone informed.

- **[Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)**  
  Structure and facilitation guidance for retrospectives. Captures learnings and converts them into prioritized action items. Best for: driving iterative improvements and building a culture of feedback.

---

## Quick Start for New Team Members

1. **Read first**: [Project Management Overview](octoacme-project-management-overview.md) (10 min)
2. **Understand your role**: Find yourself in [Roles & Personas](octoacme-roles-and-personas.md) (5 min)
3. **Current project?** Jump to the phase you're in (Initiation → Planning → Execution → Release)
4. **Questions about risk or communication?** See [Risk Management & Communication](octoacme-risks-and-communication.md)

---

## Key Workflows at a Glance

### Pull Request Workflow
- Keep PRs ≤400 lines when possible
- Include issue link and acceptance criteria in description
- Run automated tests and linting before requesting review
- Require at least one approval before merging

### Project Board Columns
Backlog → Ready → In Progress → In Review → QA → Done

### Communication Cadence
- **Daily**: 15-min standup (progress, blockers, dependencies)
- **Weekly**: PM + Product Manager sync; twice-weekly delivery team standup
- **Monthly**: Stakeholder updates
- **Ad-hoc**: Escalation for blockers and critical issues

### Quality Gates
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

---

## How to Use These Docs

- **Keep the Project Charter updated** in your project repo
- **Reference process docs** when onboarding new team members
- **Add project-specific customizations** to `.copilot/` if using Copilot Spaces for context
- **Update the Risk Register weekly** during execution
- **Treat retrospective action items** as first-class backlog items

---

## Common Scenarios

- **Starting a new project?** → Begin with [Project Initiation](octoacme-project-initiation.md)
- **Need to plan sprints?** → See [Project Planning](octoacme-project-planning.md)
- **Managing a blocker?** → Check [Risk Management & Communication](octoacme-risks-and-communication.md)
- **Preparing to ship?** → Follow [Release & Deployment](octoacme-release-and-deployment.md)
- **Wrapping up a milestone?** → Run the process in [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)

---

## Questions or Feedback?

These docs are living artifacts. If you find gaps, have suggestions, or want to add clarity:

- **Suggest an update**: Use the [Add/Update Content to Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template
- **Raise a question**: Open an issue or comment on existing ones
- **Share learnings**: Contribute improvements from your project retrospectives

Together, we scale OctoAcme's institutional knowledge and make project execution more consistent and efficient for everyone.
