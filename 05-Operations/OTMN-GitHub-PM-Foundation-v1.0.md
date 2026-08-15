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

## 3. Current label taxonomy

The OTMN label system is intentionally small and is based on demonstrated workflow needs rather than a comprehensive issue-management model.

### OTMN work/classification labels

- `idea` — An idea or possibility worth preserving; no commitment implied.
- `research` — Work requiring investigation or evaluation before a decision or implementation.
- `future` — Valid work or idea intentionally deferred; not current active work.
- `content-gap` — A missing, incomplete, or needed OTMN content/documentation item.
- `gia` — GIA should execute or process the resulting GitHub work.
- `process` — The issue concerns an OTMN/GitHub process or workflow.
- `question` — Further information or clarification is needed.
- `enhancement` — An improvement to an existing capability or workflow.

### Documentation classification

- `type: documentation` — The issue is primarily documentation/standards work.

Use `type: documentation` as the standard documentation label. The older unprefixed `documentation` label is a duplicate and should be retired after remaining issues using it are migrated.

### GitHub operational labels

These are retained as GitHub issue-management labels rather than part of the OTMN work taxonomy:

- `bug`
- `duplicate`
- `invalid`
- `wontfix`
- `good first issue`
- `help wanted`

### Labels not currently adopted

Do not create the following unless actual workflow demonstrates a need:

- `actionable`
- `idea-review`
- `decision-needed`
- `type: foundation`
- `type: process`
- `type: project`
- `priority: critical`
- `priority: high`
- `priority: medium`
- `priority: low`

`actionable` is specifically not a persistent classification because Active/Defer/Keep/Research/etc. are human triage dispositions rather than issue types.

### Triage dispositions are not labels

These symbols are human triage dispositions and should not be converted into GitHub labels merely to reproduce the vocabulary:

- 🟢 Active
- 🔵 Keep
- 🟡 Defer
- 🟣 Research
- 🔧 Update
- 🔗 Merge
- ✅ Complete
- ❌ Close

### Taxonomy change rule

New labels should earn their way into existence through demonstrated OTMN workflow needs. Do not create labels merely because a possible future issue, project, or process can be imagined.

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

## 7. Issue triage disposition guide

Issue inventory size should not be confused with active workload.

> **Ideas can be unlimited. Candidates can accumulate. Active work must remain intentionally constrained.**

Use the following human-friendly dispositions when reconciling the OTMN issue inventory:

| Symbol | Disposition | Meaning |
|---|---|---|
| 🟢 | **Active** | We are actually working on it now. |
| 🔵 | **Keep** | Valid inventory item, but not currently active work. |
| 🟡 | **Defer** | Valid work intentionally postponed for later. |
| 🟣 | **Research** | Needs investigation before a decision or implementation. |
| 🔧 | **Update** | The issue remains valid but needs its scope, wording, structure, or acceptance criteria updated. |
| 🔗 | **Merge** | Duplicate or substantially overlapping work should be consolidated with another issue. |
| ✅ | **Complete** | The work has already been completed and the issue can be closed as completed. |
| ❌ | **Close** | The issue is no longer needed, valid, or planned; close without treating it as completed work. |

### Recommended triage flow

```text
OPEN ISSUE INVENTORY
        ↓
    REVIEW ISSUE
        ↓
  DOES IT STILL MATTER?
     /           \
   NO             YES
   ↓               ↓
  ❌            WHAT IS ITS STATE?
                   ↓
     ┌─────────────┼─────────────┐
     ↓             ↓             ↓
  🟢 Active     🔵 Keep       🟡 Defer
     ↓             ↓             ↓
  Work now     Inventory     Future work

Additional dispositions:
🟣 Research → investigate first
🔧 Update   → revise issue
🔗 Merge    → consolidate duplicate/overlap
✅ Complete → work already done
❌ Close    → no longer needed
```

### Triage questions

During recurring reconciliation, ask:

1. What is this issue?
2. Does it still represent something OTMN needs to preserve?
3. Is it active work right now?
4. Does it need research or a decision before action?
5. Should it be updated, merged, completed, deferred, or closed?

These dispositions are **human triage vocabulary, not necessarily GitHub labels**. Do not create eight new labels merely to reproduce this table. Labels should remain a deliberately small machine-readable taxonomy.

The workflow is intentionally lightweight and should be expanded only if repeated use demonstrates a real need.

## 8. First PM issues

The initial PM backlog should establish the operating foundation before expanding into additional process.

Priority sequence:

1. Finalize GitHub Project configuration.
2. Reconcile and maintain the label taxonomy based on demonstrated use.
3. Establish issue templates.
4. Establish PR template.
5. Document and pilot GIA workflow.
6. Audit repository privacy/public-information boundaries.
7. Perform a first weekly PM review and simplify anything that proved unnecessary.

## Implementation note

The GitHub connector can create branches, files, issues, and pull requests, but the current connector surface does not expose GitHub Projects or repository-label creation. Those two configuration items therefore remain manual GitHub-admin steps in this implementation pass.
