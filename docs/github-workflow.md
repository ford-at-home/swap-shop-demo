# 🔄 GitHub Workflow Protocols

## Overview
This document defines the GitHub workflow protocols and standards for autonomous agent collaboration. These protocols ensure consistent, traceable, and high-quality development practices.

## Project Management Structure

### 1. Issue
A work unit representing a small task, bug report, or feature request (e.g., evaluate Vercel vs. AWS, deploy app to localhost, implement comprehensive integration testing, rollout to prod environment).

**Used for**: Assignable, actionable pieces of work.

**Best practices**:
- Stored as a GitHub issue
- One owner per issue, but multiple is OK
- Clear definition of done
- Linked to commits and PRs
- Labeled for type (bug, enhancement, infra), status (in progress, blocked, etc.), and team (frontend, backend, etc.)
- Estimated with time or complexity (e.g., t-shirt size, story points)

### 2. Epic
A feature-level objective comprised of a collection of related issues contributing to a broader goal (e.g., select tech stack, setup 3-environment cloud environment, develop frontend interface, frontend-backend integration).

**Used for**: Grouping all work needed for a feature, initiative, or large unit of value.

**Best practices**:
- Stored as a GitHub issue labeled 'epic'
- Has a goal or user story
- Has a checklist of child issues
- Progress is visualized through the number of closed issues

### 3. Milestone
A phase-based container representing a step towards a (MVP) product release or upgrade (e.g., research, backend, frontend, cloud deployment, beta rollout).

**Used for**: Planning work toward goals

**Best practices**:
- One milestone per sprint or release (e.g., Sprint 27, Q3 Launch)
- Comprised of child epics containing child issues

---

## Agent Execution Protocol

### 1. Work Execution Protocol

#### 1.1 Issue Eligibility
An agent may only begin work on an issue if all of the following are true:
- The issue includes a label matching the agent's role (frontend, backend, infra, etc.)
- The issue is assigned to a Milestone
- The issue is linked as a child to an Epic
- The parent Epic is labeled "In Progress"
- The issue is assigned to the agent

#### 1.2 Escalation and Triage
If an agent encounters unexpected complexity or blockers, it must:

1. Apply a label to the issue in the format: `<role>-level-2-triage`
   - Example: `backend-level-2-triage`

2. Add a comment describing:
   - What action was being taken
   - The specific blocker encountered
   - Any conflicting requirements or technical ambiguity

3. The agent must halt execution on the issue until a senior agent or human acknowledges and clears the blocker.

### 2. Branching Protocol

#### 2.1 Branch Naming
Branches must be created from main using the following format:
```
<type>/<issue-number>-<slug>
```

**Examples**:
- `feature/123-reset-password`
- `bugfix/147-fix-timezone-issue`

#### 2.2 Restrictions
- No agent may commit directly to main
- No use of unstructured or ad-hoc branch names

### 3. Commit Standards

#### 3.1 Format
All commits must follow the Conventional Commits specification:
```
<type>: <description> (#<issue-number>)
```

**Examples**:
- `feat: implement reset password form (#123)`
- `fix: correct timezone calculation (#147)`

#### 3.2 Restrictions
- Do not commit messages like "wip", "quick fix", or "misc"
- Commit scope must be minimal and traceable to the linked issue

### 4. Pull Request Workflow

#### 4.1 Creation Requirements
When opening a PR, agents must:

1. Base it on a single GitHub Issue
2. Use the naming format: `[#<issue-number>] <descriptive title>`
3. Use the repository's PR template
4. Include:
   - `Closes #<issue-number>` in the body
   - A description of the change
   - Screenshots or logs if applicable

#### 4.2 Size and CI Enforcement
- PRs must be under 500 lines of code changed
- PRs must remain in Draft state until:
  - All required CI checks pass (lint, tests, typechecking)
  - The PR is fully ready for review
- Agents must not mark PRs as "Ready for Review" if any checks are failing

### 5. Test Protocol
- All business logic must include unit tests
- All user-facing flows must include integration or end-to-end tests
- CI must confirm all tests pass before merge is allowed

### 6. Merge Behavior
- Only use "Squash and Merge"
- All required reviews and CI checks must be complete
- Feature branches must be deleted after merge

### 7. Project Hygiene & Governance
- `main` must remain deployable at all times
- A nightly CI pipeline must run against main
- Issue triage occurs weekly
- Technical debt is reviewed monthly
- GitHub Project board must be kept in sync: Backlog, Ready, In Progress, In Review, Done

### 8. Enforcement
Compliance is enforced through:
- GitHub branch protection rules
- CODEOWNERS for critical files
- Required status checks
- Static PR and Issue templates in `.github/`

**Agents found non-compliant will be suspended or re-initialized.**

---

## Label System

### Issue Type Labels
- `bug` - Something isn't working
- `enhancement` - New feature or request
- `documentation` - Improvements or additions to documentation
- `refactor` - Code improvement without functional changes
- `test` - Testing related changes
- `infrastructure` - DevOps, deployment, or tooling changes

### Status Labels
- `in-progress` - Currently being worked on
- `blocked` - Cannot proceed due to external dependency
- `review-needed` - Ready for review
- `needs-testing` - Requires additional testing
- `ready-to-merge` - Approved and ready for merge

### Role Labels
- `frontend` - Frontend development work
- `backend` - Backend development work
- `devops` - Infrastructure and deployment
- `design` - UI/UX design work
- `research` - Research and analysis tasks
- `security` - Security-related work
- `performance` - Performance optimization

### Priority Labels
- `priority-critical` - Must be fixed immediately
- `priority-high` - Should be resolved soon
- `priority-medium` - Normal priority
- `priority-low` - Can be deferred

### Phase Labels
- `phase-discovery` - Discovery & validation phase
- `phase-specification` - Product specification phase
- `phase-architecture` - Architecture & planning phase
- `phase-implementation` - Implementation phase
- `phase-qa` - QA & review phase
- `phase-release` - Release & monitoring phase
- `phase-iteration` - Feedback & iteration phase

---

## Templates

### Issue Template
```markdown
## Description
Brief description of the issue or feature request.

## Acceptance Criteria
- [ ] Criterion 1
- [ ] Criterion 2
- [ ] Criterion 3

## Implementation Notes
Any technical details, constraints, or considerations.

## Definition of Done
- [ ] Code implemented
- [ ] Tests written and passing
- [ ] Documentation updated
- [ ] Code reviewed and approved
- [ ] Deployed to staging

## Related Issues
- Epic: #XXX
- Related: #XXX
```

### Pull Request Template
```markdown
## Description
Brief description of the changes made.

## Changes Made
- Change 1
- Change 2
- Change 3

## Testing
- [ ] Unit tests added/updated
- [ ] Integration tests added/updated
- [ ] Manual testing completed
- [ ] All tests passing

## Screenshots/Logs
(If applicable)

## Closes
Closes #XXX
```

---

*This document is part of the [Swarm Playbook](../CLAUDE.md) for autonomous agent collaboration.*
