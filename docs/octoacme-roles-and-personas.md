# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

## Role ownership and decision boundaries

These roles describe responsibilities, not mandatory new positions. One person may hold multiple roles; name an owner for each applicable responsibility in the Project One-pager and record handoffs in the project board. Explicit ownership improves onboarding, reduces duplicated or missed work, and makes delivery and escalation more predictable.

- PM means Project Manager; PdM means Product Manager. Product Lead refers to the project's accountable product leadership responsibility in the lifecycle guides. Record whether the PdM fills that responsibility or a separate Product Lead holds it, including any delegated approval authority.
- The PdM owns product outcomes and backlog prioritization; the PM owns delivery coordination, schedules, risks, and communications. Technical, design, quality, and operations roles contribute specialist evidence without taking over those responsibilities.
- During planning, agree with stakeholders who prepares evidence, recommends readiness, and approves scope changes or release decisions. Record named decision owners and authority in the project plan or decision log; these personas do not introduce new approval gates or replace existing release requirements.
- For release decisions, QA provides test results and outstanding defects, the Technical Lead provides technical risk assessments, and the Release / Operations Lead consolidates operational readiness and recommends deployment readiness. The PdM confirms acceptance against product outcomes; the PM coordinates the decision with the agreed approver and records the outcome.
- Follow the existing escalation path: team-level -> PM -> Product Lead -> Sponsor. For security incidents, follow the security incident runbook and notify Security on-call.

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

## QA / Test Lead

### Role Summary
The QA / Test Lead coordinates quality validation and provides evidence that work meets acceptance criteria. Developers remain responsible for writing and maintaining their tests.

### Responsibilities
- Own the test plan and coordinate integration, end-to-end, and manual acceptance testing as applicable
- Clarify testable acceptance criteria with the PdM and testability needs with Developers
- Track defects and verification results with Developers; share severity and customer impact with the PdM for prioritization
- Report test coverage, unresolved defects, and quality risks to the PM and Release / Operations Lead

### Goals
- Detect defects early and reduce escaped defects
- Make acceptance and release readiness evidence clear

### Typical Communication
- Acceptance criteria reviews with the PdM and Developers
- Defect triage and test results in issues and the project board
- Quality readiness summaries and blocker escalation to the PM

---

## Technical Lead

### Role Summary
The Technical Lead guides technical design and engineering decisions, helping Developers deliver maintainable components and reliable integrations. Product prioritization stays with the PdM and delivery coordination stays with the PM.

### Responsibilities
- Own technical design decisions and document their rationale and trade-offs
- Collaborate with Developers on engineering standards, design reviews, and integration approaches
- Explain feasibility, technical constraints, and implementation options to the PdM
- Provide estimates, dependencies, and technical risk mitigations to the PM
- Share technical readiness evidence with QA and the Release / Operations Lead

### Goals
- Reduce integration surprises and technical rework
- Maintain reliable, supportable architecture

### Typical Communication
- Technical design documents and PR reviews with Developers
- Planning discussions with the PdM and PM
- Technical risk updates in the risk register and release readiness discussions

---

## UX / Design Lead

### Role Summary
The UX / Design Lead translates user needs into usable, accessible experiences and validates design choices with users and the delivery team.

### Responsibilities
- Own research findings, user journeys, and interaction designs
- Partner with the PdM to validate problems, desired outcomes, and usability-related acceptance criteria
- Provide designs, accessibility expectations, and behavior clarifications to Developers and QA
- Coordinate design handoffs, dependencies, and research timelines with the PM
- Review implemented experiences and share usability findings with the PdM for prioritization

### Goals
- Improve usability and accessibility
- Reduce rework caused by unclear user needs or designs

### Typical Communication
- Research summaries and design reviews with the PdM and Developers
- Design handoffs and acceptance discussions with Developers and QA
- Design dependency updates through the project board and PM

---

## Release / Operations Lead

### Role Summary
The Release / Operations Lead coordinates operational readiness and deployment activities, using QA and engineering evidence to recommend deployment readiness rather than replacing their validation or the agreed approver.

### Responsibilities
- Own the deployment checklist, operational readiness summary, and rollback plan with input from Developers
- Coordinate staging and production deployments, smoke tests, monitoring, and post-deploy verification with Developers and QA
- Align release timing and communications with the PM and release scope and customer impact with the PdM
- Consolidate readiness evidence and raise unresolved deployment risks to the PM and agreed release approver
- Trigger incident response and notify on-call when needed; coordinate rollback under the agreed incident and release authority

### Goals
- Make releases predictable and observable
- Reduce deployment failures and recovery time

### Typical Communication
- Release readiness reviews with Developers, QA, the PdM, and PM
- Deployment status and rollback instructions in the release document
- Incident updates through the established on-call and stakeholder channels

---

## Project Sponsor

### Role Summary
The Project Sponsor champions the business outcome, secures organizational support, and resolves escalated business decisions within agreed authority. The Sponsor does not manage daily delivery.

### Responsibilities
- Support business alignment and resource commitments for the Project One-pager
- Resolve escalated funding, scope, and priority conflicts within documented authority; route decisions beyond that authority to the appropriate stakeholders
- Review status and escalations from the PM through the existing escalation path
- Align major outcome trade-offs with the PdM or designated Product Lead and seek feasibility input from the Technical Lead and Developers
- Record sponsorship decisions and rationale in the decision log with the PM

### Goals
- Keep the project aligned with business objectives
- Reduce delays caused by unresolved resource constraints or business decisions

### Typical Communication
- Initiation alignment and milestone reviews with the PM and PdM
- Stakeholder updates and decision requests coordinated by the PM
- Escalation decisions documented in the decision log

---

## Customer Support / Customer Success Representative

### Role Summary
The Customer Support / Customer Success Representative connects customer experience with delivery, preparing customer-facing teams for changes and bringing post-release feedback into product planning.

### Responsibilities
- Gather recurring customer problems and share evidence and impact with the PdM for prioritization
- Own support guidance and customer-facing known-issue information, using release notes and technical input
- Coordinate launch communications and support readiness with the PM and Release / Operations Lead
- Work with Developers and QA to provide reproducible issue reports and verify troubleshooting guidance
- Summarize adoption concerns and post-release feedback for the PdM; escalate urgent delivery blockers through the PM and production incidents through the established incident process

### Goals
- Improve customer adoption and support readiness
- Shorten the feedback loop between customers and the delivery team

### Typical Communication
- Customer feedback summaries and backlog discussions with the PdM
- Launch readiness updates with the PM and Release / Operations Lead
- Reproducible issue reports and known-issue updates with Developers and QA

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

