# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged (validated by **QA** and **Product Manager**)
- Passing CI and security scans (verified by **Security Lead**)
- Release notes drafted (prepared by **Project Manager** with input from **Product Manager**)
- Rollback / mitigation plan documented (prepared by **Developers** and **Project Manager**)
- Smoke tests prepared (prepared by **QA**)
- Customer communication plan ready (prepared by **Customer Success Manager** if customer-facing)
- Design implementation validated (verified by **UX Designer** for UI changes)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) - coordinated by **Project Manager**
- [ ] Backup or snapshot (if applicable) - verified by **Developers**
- [ ] Deploy to staging and run smoke tests - executed by **Developers** and **QA**
- [ ] Security scan on staging - verified by **Security Lead**
- [ ] Deploy to production (automated pipeline preferred) - executed by **Developers**
- [ ] Run post-deploy verifications - executed by **QA**
- [ ] Monitor error rates and performance - monitored by **Developers** and **Project Manager**
- [ ] Announce release to stakeholders and support - communicated by **Project Manager** and **Customer Success Manager**
- [ ] Update customer-facing documentation (if applicable) - updated by **Customer Success Manager** or **Technical Writers**

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (**Project Manager** coordinates, **Security Lead** for security incidents)
  - Rollback to last known-good release if necessary (executed by **Developers**)
  - **Customer Success Manager** manages customer communications and impact assessment
  - Triage root cause and capture action items (led by **Scrum Master** or **Project Manager**)
  - Schedule blameless post-mortem with all involved roles

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
