# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

### Communication Responsibility Matrix (RACI)

| Activity | PM | PdM | SM | Dev | QA | BA | UX | Security | CSM |
|----------|----|----|----|----|----|----|----|---------|----|
| Project status updates | R | A | C | I | I | I | I | I | I |
| Risk escalation | A | C | C | I | I | I | I | C | C |
| Sprint planning | C | C | R | C | C | C | C | C | I |
| Requirements clarification | C | C | I | C | C | R | C | I | I |
| Design reviews | I | C | I | C | I | C | R | I | C |
| Security reviews | C | I | I | C | C | I | I | R | I |
| Customer feedback | I | A | I | I | I | C | C | I | R |
| Release communications | R | A | C | I | C | I | I | C | C |
| Retrospectives | C | C | R | C | C | C | C | C | I |

**Legend:**
- **R** = Responsible (does the work)
- **A** = Accountable (final approval/decision)
- **C** = Consulted (provides input)
- **I** = Informed (kept in the loop)

## Role-Specific Communication Templates

### For Project Managers
**Weekly Status Template:**
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:
- Team velocity: [X] story points / sprint

### For Product Managers
**Roadmap Update Template:**
- Priorities this quarter:
- Recently shipped:
- In progress:
- Success metrics / outcomes:
- Customer feedback themes:
- Trade-offs and decisions:

### For Scrum Masters
**Sprint Report Template:**
- Sprint goal: [achieved/not achieved]
- Completed: [X] story points
- Velocity trend: [improving/stable/declining]
- Key impediments removed:
- Upcoming risks:
- Team health: [green/yellow/red]

### For Business Analysts
**Requirements Change Template:**
- Change description:
- Rationale:
- Impact on scope/timeline:
- Affected user stories:
- Stakeholder approval:
- Communication plan:

### For UX Designers
**Design Review Summary:**
- Design goal:
- Key user flows:
- Design decisions and rationale:
- Accessibility considerations:
- Feedback incorporated:
- Next steps:

### For Security Leads
**Security Assessment Summary:**
- Scope of review:
- Vulnerabilities identified: [Critical/High/Med/Low]
- Remediation recommendations:
- Risk acceptance (if applicable):
- Compliance status:
- Sign-off: [approved/conditional/blocked]

### For Customer Success Managers
**Customer Feedback Summary:**
- Feedback period:
- Key themes:
- Feature requests: [P0/P1/P2]
- Pain points:
- Customer sentiment: [positive/neutral/negative]
- Recommended actions:

## Communication Templates

Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
