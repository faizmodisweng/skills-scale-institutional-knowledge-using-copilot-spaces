# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

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

### Escalation Levels and Role Involvement
- **Level 1 (Team-level)**: Team discusses in standup; **Scrum Master** removes impediments; **Developers** and **QA** collaborate on technical blockers
- **Level 2 (Cross-team)**: **Project Manager** escalates to stakeholders and dependent teams; **Security Lead** involved for security issues; **Business Analyst** clarifies requirements
- **Level 3 (Business impact)**: **Product Manager** and sponsor make priority/scope decisions; **Customer Success Manager** coordinates customer impact assessment
- **Emergency/P0**: **Security Lead** leads security incidents; **Customer Success Manager** manages customer communications; **Project Manager** coordinates resolution

### Escalation Decision Criteria
| Severity | Criteria | Response Time | Escalation Path |
|----------|----------|---------------|-----------------|
| P0 (Critical) | Production down, security breach, major customer impact | Immediate | SM → PM → PdM + Security Lead + CSM → Sponsor |
| P1 (High) | Feature blocked, deadline at risk, significant quality issue | 4 hours | SM → PM → PdM |
| P2 (Medium) | Minor blocker, can work around, needs decision | 1 business day | SM → PM |
| P3 (Low) | Nice-to-have, low impact | Next sprint planning | Team discussion |

## Role-Specific Handoff Checklists

### Requirements Handoff (Business Analyst → Developers)
- [ ] User stories include acceptance criteria
- [ ] Business logic and edge cases documented
- [ ] Dependencies and constraints identified
- [ ] Success metrics and validation approach defined
- [ ] Questions answered and documented
- [ ] Design mockups or wireframes attached (if applicable)

### Design Handoff (UX Designer → Developers)
- [ ] Mockups exported and accessible
- [ ] Design specifications documented (spacing, colors, typography)
- [ ] Interactive prototypes shared (if applicable)
- [ ] Accessibility requirements specified (WCAG level, keyboard navigation)
- [ ] Responsive breakpoints defined
- [ ] Edge cases and error states designed
- [ ] Assets exported in required formats

### Development Handoff (Developers → QA)
- [ ] Code merged to test branch
- [ ] Unit tests passing
- [ ] Test environment deployed
- [ ] Test data prepared or documented
- [ ] Known issues or limitations documented
- [ ] Acceptance criteria referenced in PR
- [ ] Demo/walkthrough scheduled (if needed)

### QA Handoff (QA → Release)
- [ ] All acceptance criteria validated
- [ ] Regression tests passed
- [ ] Performance and security scans completed
- [ ] Test results documented
- [ ] Defects logged and triaged
- [ ] Smoke test plan prepared for production
- [ ] Sign-off from Product Manager and Security Lead

### Release Handoff (Release Team → Customer Success)
- [ ] Release notes published
- [ ] Known issues and workarounds documented
- [ ] Customer-facing documentation updated
- [ ] Training materials prepared (if needed)
- [ ] Rollback plan documented
- [ ] Support team briefed
- [ ] Customer communication sent (if needed)

## Inter-Role Communication Guidelines

### Daily Standup Participants
- **Core**: Developers, Scrum Master, QA
- **As Needed**: Product Manager (for prioritization), UX Designer (for design questions), Business Analyst (for requirements clarification)

### Sprint Planning Participants
- **Required**: Scrum Master (facilitates), Product Manager (prioritizes), Developers (estimate), Business Analyst (clarifies requirements)
- **Recommended**: UX Designer (design readiness), Security Lead (security requirements), QA (testability)

### Sprint Review/Demo Participants
- **Core**: Product Manager, Developers, Scrum Master, Stakeholders
- **Recommended**: Customer Success Manager (customer perspective), UX Designer (design validation), Business Analyst (requirements validation)

### Retrospective Participants
- **Required**: All team members (Developers, Scrum Master, QA, PM)
- **Optional**: Product Manager, UX Designer (for cross-functional insights)

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
