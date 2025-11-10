# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- **UX Designer**: Design QA completed for user-facing changes
- **QA Lead**: All tests passed, regression testing complete
- **DevOps Engineer**: Infrastructure and deployment automation verified
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) - coordinated by PM and DevOps Engineer
- [ ] Backup or snapshot (if applicable) - DevOps Engineer
- [ ] Deploy to staging and run smoke tests - DevOps Engineer, QA Lead
- [ ] Deploy to production (automated pipeline preferred) - DevOps Engineer
- [ ] Run post-deploy verifications - QA Lead, DevOps Engineer
- [ ] Monitor system health and error rates - DevOps Engineer
- [ ] Announce release to stakeholders and support - PM, Customer Support Liaison
- [ ] Customer Support Liaison notified of release notes and known issues

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **DevOps Engineer**: Trigger incident response and notify on-call
  - **DevOps Engineer**: Rollback to last known-good release if necessary
  - **QA Lead**: Verify rollback success and system stability
  - **Customer Support Liaison**: Communicate status to affected customers
  - **PM**: Triage root cause and capture action items with team

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
