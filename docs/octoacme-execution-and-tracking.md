# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
  - Participants: Developers, QA, DevOps, Technical Lead, PM
- Weekly delivery sync — show progress, updates, and flagged risks
  - Participants: PM, PdM, Technical Lead
- Demo/Review at the end of each sprint or milestone
  - Participants: Full team + stakeholders
- Technical design reviews as needed
  - Participants: Technical Lead, Developers, DevOps, QA
- Retrospectives after major milestones
  - Participants: Full delivery team

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Technical Lead or senior developer reviews code
  - DevOps verifies CI pipeline passes (tests, lint, security scans)
  - QA validates against acceptance criteria
  - Require at least one approval before merging (or team-defined policy)
- For collaboration patterns, see [octoacme-collaboration-workflows.md](octoacme-collaboration-workflows.md)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup (Developers, QA, DevOps, Tech Lead)
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues
- Technical blockers: Technical Lead coordinates resolution
- Infrastructure blockers: DevOps Engineer leads with PM support
- See [octoacme-collaboration-workflows.md](octoacme-collaboration-workflows.md) for detailed escalation paths

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
