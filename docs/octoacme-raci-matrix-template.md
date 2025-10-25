# OctoAcme RACI Matrix Template

## Purpose
The RACI matrix clarifies roles and responsibilities for key project activities. Use this template to define accountability and prevent confusion about who does what.

## RACI Legend
- **R** = Responsible: Does the work to complete the task
- **A** = Accountable: Ultimately answerable for completion (only one A per task)
- **C** = Consulted: Provides input and expertise (two-way communication)
- **I** = Informed: Kept up-to-date on progress (one-way communication)

---

## Project Activities RACI Matrix

| Activity | PM | PdM | Dev | Tech Lead | QA | DevOps | BA | Stakeholder |
|----------|----|----|-----|-----------|-------|--------|----|----|
| **Initiation Phase** |
| Define problem statement | C | A/R | I | C | I | I | C | C |
| Create project one-pager | R | A | I | C | I | I | C | I |
| Stakeholder identification | R | C | I | I | I | I | C | A |
| Initial risk assessment | A/R | C | C | C | I | C | C | I |
| Go/no-go decision | C | C | I | I | I | I | I | A |
| **Planning Phase** |
| Kickoff meeting facilitation | A/R | C | C | C | C | C | C | I |
| Backlog creation | C | A/R | C | C | C | I | C | I |
| Technical architecture | C | I | C | A/R | C | C | I | I |
| Test strategy | C | C | C | C | A/R | C | I | I |
| Sprint planning | R | C | A | C | C | I | C | I |
| Definition of Done | C | C | A/R | C | R | C | C | I |
| Release planning | A/R | C | C | C | C | C | I | C |
| **Execution Phase** |
| Feature implementation | I | I | A/R | C | C | I | I | I |
| Code reviews | I | I | R | A/R | I | I | I | I |
| Unit testing | I | I | A/R | C | C | I | I | I |
| Integration testing | I | I | C | C | A/R | C | I | I |
| CI/CD pipeline maintenance | I | I | C | C | C | A/R | I | I |
| Bug triage | C | C | R | C | A/R | I | I | I |
| Daily standups | A/R | I | R | R | R | R | C | I |
| Sprint demos | R | C | R | C | R | C | C | A |
| Risk monitoring | A/R | C | C | C | C | C | C | I |
| **Release Phase** |
| Release notes | R | C | C | I | C | C | C | I |
| Pre-release testing | C | I | C | C | A/R | C | I | I |
| Deployment execution | C | I | C | C | C | A/R | I | I |
| Smoke testing | C | I | R | C | A/R | C | I | I |
| Stakeholder communication | A/R | C | I | I | I | I | I | C |
| **Close Phase** |
| Retrospective facilitation | A/R | C | C | C | C | C | C | I |
| Lessons learned documentation | R | C | C | C | C | C | C | I |
| Project closure report | A/R | C | I | I | I | I | I | C |

---

## How to Use This Template

1. **Customize for your project**: Not all activities may apply. Add or remove rows as needed.
2. **Ensure single accountability**: Each row should have exactly one "A" to prevent confusion.
3. **Review with the team**: Share the matrix during kickoff and validate everyone understands their roles.
4. **Update as needed**: Revisit during retrospectives if role confusion occurs.
5. **Store with project artifacts**: Keep the RACI matrix in your project repository or wiki.

---

## Example: Custom Activity Entry

| Activity | PM | PdM | Dev | Tech Lead | QA | DevOps | BA | Stakeholder |
|----------|----|----|-----|-----------|-------|--------|----|----|
| Security review | C | I | C | A/R | C | C | I | I |
| Performance benchmarking | C | C | R | C | A/R | C | I | I |

---

## Tips for Success

- **Discuss ambiguities**: If multiple people feel accountable, clarify and update.
- **Balance workload**: If one role has too many "R" entries, consider redistributing.
- **Communicate changes**: When roles shift mid-project, update the matrix and notify the team.
- **Use in onboarding**: New team members can quickly understand expectations.
