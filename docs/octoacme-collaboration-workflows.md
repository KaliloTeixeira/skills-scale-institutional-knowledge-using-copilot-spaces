# OctoAcme Collaboration Workflows

## Purpose
Define standard collaboration patterns between roles to improve handoffs, reduce confusion, and accelerate delivery.

---

## Feature Development Workflow

### 1. Requirements Definition
**Flow**: Stakeholder → BA → PdM → Dev Team

1. **Stakeholder** identifies business need
2. **Business Analyst** conducts requirements workshop and documents user stories
3. **Product Manager** prioritizes against roadmap and defines success metrics
4. **Technical Lead** and **Developers** review for feasibility and provide estimates
5. **QA Engineer** reviews acceptance criteria for testability
6. **Product Manager** finalizes and adds to backlog

**Key Artifacts**: User stories, acceptance criteria, success metrics

---

### 2. Sprint Planning
**Flow**: PM facilitates; all delivery roles participate

1. **Project Manager** prepares sprint planning agenda
2. **Product Manager** presents prioritized backlog items
3. **Technical Lead** and **Developers** estimate effort and identify dependencies
4. **QA Engineer** confirms test approach and capacity
5. **DevOps Engineer** highlights infrastructure constraints
6. **Team** commits to sprint scope

**Key Artifacts**: Sprint backlog, Definition of Done, capacity plan

---

### 3. Implementation & Review
**Flow**: Dev → Tech Lead → QA → PM

1. **Developer** implements feature and creates PR
2. **Technical Lead** conducts code review and provides feedback
3. **Developer** updates code based on feedback
4. **DevOps Engineer** ensures CI passes (tests, lint, security scans)
5. **QA Engineer** validates against acceptance criteria
6. **Project Manager** moves item to "Done" and updates status

**Key Artifacts**: Pull request, code review comments, test results

---

### 4. Deployment
**Flow**: DevOps leads; Dev and QA support

1. **QA Engineer** completes final acceptance testing
2. **DevOps Engineer** prepares release and smoke tests
3. **Project Manager** coordinates deployment window with stakeholders
4. **DevOps Engineer** executes deployment
5. **QA Engineer** runs post-deployment smoke tests
6. **Project Manager** announces release to stakeholders

**Key Artifacts**: Release notes, deployment checklist, smoke test results

---

## Cross-Role Collaboration Patterns

### Technical Decision Making
**Participants**: Technical Lead, Developers, DevOps, QA

**When**: Major architectural changes, technology choices, technical debt prioritization

**Process**:
1. **Proposer** creates technical design doc with problem, options, and recommendation
2. **Technical Lead** reviews and adds architectural considerations
3. **DevOps** reviews operational impact (scalability, monitoring, cost)
4. **QA** reviews testability implications
5. **Technical Lead** makes final decision and documents in decision log
6. **Project Manager** updates timeline and risks if needed

---

### Risk Escalation
**Participants**: Any role → PM → PdM/Tech Lead → Stakeholder

**When**: Blockers, delays, quality issues, scope changes

**Process**:
1. **Team member** identifies risk and notifies Project Manager
2. **Project Manager** assesses impact and updates risk register
3. If resolvable at team level: **PM** coordinates mitigation with team
4. If requires product decision: **PM** escalates to **Product Manager**
5. If requires technical decision: **PM** escalates to **Technical Lead**
6. If requires resources/timeline change: **PM** escalates to **Stakeholder**
7. **PM** communicates resolution and updates status

---

### Quality Issues
**Participants**: QA → Dev → Tech Lead → PM

**When**: Defects found, test failures, quality concerns

**Process**:
1. **QA Engineer** creates defect with reproduction steps and severity
2. **Project Manager** and **Product Manager** triage priority
3. **Technical Lead** assigns to appropriate **Developer**
4. **Developer** fixes and creates PR
5. **Technical Lead** reviews fix
6. **QA Engineer** verifies fix
7. **DevOps Engineer** includes in next deployment

---

### Requirements Clarification
**Participants**: Any role → BA/PdM → Stakeholder (if needed)

**When**: Ambiguous requirements, missing acceptance criteria, conflicting needs

**Process**:
1. **Team member** flags ambiguity in backlog item or standup
2. **Business Analyst** schedules clarification session with **Product Manager**
3. If needed, **BA** or **PdM** consults **Stakeholder**
4. **BA** updates user story and acceptance criteria
5. **Product Manager** confirms and reprioritizes if necessary
6. **Project Manager** notifies team of changes

---

## Communication Cadences

### Daily (15 minutes)
- **Participants**: Dev, QA, DevOps, Tech Lead, PM
- **Purpose**: Progress updates, blockers, daily coordination
- **Format**: Standup (async or sync)

### Weekly (30-60 minutes)
- **Participants**: PM, PdM, Tech Lead
- **Purpose**: Roadmap alignment, capacity planning, risk review
- **Format**: Leadership sync

### Sprint/Milestone (2-4 weeks)
- **Participants**: Full team + stakeholders
- **Purpose**: Demo, retrospective, planning
- **Format**: Demo → retro → planning

### Monthly
- **Participants**: PM, PdM, Stakeholders
- **Purpose**: Progress update, roadmap review, budget
- **Format**: Stakeholder review

---

## Best Practices

### For Effective Handoffs
1. **Document decisions**: Use decision logs for important technical and product choices
2. **Clear acceptance criteria**: QA and Dev should align on "done" before starting
3. **Early involvement**: Include QA and DevOps in planning, not just execution
4. **Written summaries**: After meetings, summarize decisions and action items

### For Reducing Bottlenecks
1. **Empower Technical Leads**: Delegate code review and technical decisions
2. **Parallel workstreams**: QA writes test plans while Dev implements
3. **Self-service**: DevOps provides tools for developers to deploy to staging
4. **Clear escalation paths**: Don't wait for the weekly sync to raise blockers

### For Maintaining Alignment
1. **Single source of truth**: Use project board and roadmap as canonical references
2. **Regular syncs**: Don't skip standups or weekly leadership syncs
3. **Visible metrics**: Dashboard with velocity, quality, and customer impact
4. **Feedback loops**: Retrospectives capture and act on improvement ideas

---

## Troubleshooting Common Issues

### "Too many cooks in the kitchen"
- **Symptom**: Multiple people making conflicting decisions
- **Solution**: Review RACI matrix; ensure one accountable person per decision

### "Information silos"
- **Symptom**: Team members surprised by decisions or changes
- **Solution**: Improve documentation in PR descriptions and decision logs

### "Waiting on approvals"
- **Symptom**: Work blocked waiting for reviews or sign-offs
- **Solution**: Set SLAs for reviews; empower more people to approve

### "Unclear ownership"
- **Symptom**: Work falls through the cracks or duplicated effort
- **Solution**: Use RACI matrix and assign explicit owners to backlog items
