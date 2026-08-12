# OTMN GitHub PM Foundation v1.0

**Status:** Implementation baseline
**Scope:** OnTheMarkNetwork GitHub project management

## Purpose

Provide a small, repeatable operating foundation for planning and executing OTMN work through GitHub.

## 1. Project Headquarters structure

```text
project-headquarters/
├── 01-Vision/
├── 02-Roadmap/
├── 03-Projects/
├── 04-Standards/
├── 05-Operations/
├── OTMN-CODEX-WRITE-TEST.md
└── README.md
```

GitHub issues and projects are the execution layer; durable documentation belongs in the appropriate headquarters section.

## 2. GitHub Project

Create the organization-level project **OTMN PM — Foundations v1.0**.

Recommended views:
- Board: Backlog → Ready → In Progress → Review → Done
- Roadmap: priority and target sequencing
- Table: full issue inventory

Recommended fields:
- Status
- Priority
- Area
- Target

## 3. Initial labels

Use a deliberately small label set:

- `priority: critical`
- `priority: high`
- `priority: medium`
- `priority: low`
- `type: foundation`
- `type: documentation`
- `type: process`
- `type: project`
- `type: bug`
- `content-gap`
- `gia`

## 4. Issue templates

Provide templates for:
- Feature / initiative
- Task
- Bug / problem
- Documentation / standard

Each template should capture purpose, scope, acceptance criteria, priority, and dependencies where relevant.

## 5. Pull request template

Every PR should state:
- What changed
- Why it changed
- Scope of change
- Validation performed
- Related issue
- Any follow-up work

## 6. GIA workflow

`GIA` means GitHub Item Add. GIA is the OTMN shorthand for turning a clearly defined work item into the appropriate GitHub artifact.

Default flow:

1. Identify the target repository.
2. Read the current relevant file or issue before modifying it.
3. Determine whether the request is an issue, file change, branch/PR, or organizational configuration task.
4. Prefer a branch and PR for substantive repository changes.
5. Make the smallest purposeful change.
6. Create or update the relevant issue and labels when supported.
7. Verify the result.
8. Report exactly what changed and what remains manual.

GIA must not invent repository state, skip required approval, or expand scope without a reason.

## 7. First PM issues

The initial PM backlog should establish the operating foundation before expanding into additional process.

Priority sequence:

1. Finalize GitHub Project configuration.
2. Establish initial label taxonomy.
3. Establish issue templates.
4. Establish PR template.
5. Document and pilot GIA workflow.
6. Audit repository privacy/public-information boundaries.
7. Perform a first weekly PM review and simplify anything that proved unnecessary.

## Implementation note

The GitHub connector can create branches, files, issues, and pull requests, but the current connector surface does not expose GitHub Projects or repository-label creation. Those two configuration items therefore remain manual GitHub-admin steps in this implementation pass.