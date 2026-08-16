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

## 8. Idea → Candidate → Work → Active lifecycle

The OTMN workflow distinguishes between something worth capturing, something worth considering, something deliberately committed as work, and work deliberately selected for current execution attention.

> **Ideas can be captured without creating an obligation to act.**

> **Captured work does not become active work automatically.**

> **Advancement into active work requires deliberate selection.**

| State | Meaning | Does it enter active workload? |
|---|---|---|
| 💡 **Idea** | A captured possibility, observation, question, or opportunity. | No |
| 🔎 **Candidate** | An idea with enough relevance, substance, or potential value to warrant consideration as possible work. | No |
| 🛠️ **Work** | A candidate deliberately committed by OTMN as actionable work with a clear objective or next action. | Eligible for selection; not automatically active |
| 🟢 **Active** | Work deliberately selected to receive current OTMN execution attention. | Yes |

Promotion into active work is deliberate, not automatic:

```text
💡 IDEA
   ↓
worth considering
   ↓
🔎 CANDIDATE
   ↓
deliberate commitment
   ↓
🛠️ WORK
   ↓
START HERE / WHAT'S NEXT evaluation
   ↓
deliberate selection + authorization
   ↓
🟢 ACTIVE WORK
   ↓
execution
   ↓
reconciliation
```

A candidate may remain a candidate indefinitely, be deferred, or be rejected/closed. Work may remain valid without being active. Only deliberately selected **Active Work** enters the current execution workload.

This lifecycle is a lightweight operating rule, not a new GitHub label taxonomy, Project workflow, database, or automation system. Expand it only if repeated OTMN use demonstrates a real need.

## 9. Active-Work Authority

### Current authority rule

**Mark has final authority over what becomes active work under the current OTMN operating model.**

GIA/ChatGPT may:

- discover and capture work;
- analyze the inventory;
- reconcile stale or outdated items;
- identify candidates;
- recommend priorities and sequencing; and
- maintain resulting artifacts when authorized.

GIA/ChatGPT does not independently promote an item into active work unless Mark explicitly authorizes that selection.

This is the current operating model and is not a permanent limitation on future team, delegated, or agentic-AI governance.

### Active-work definition

Active work is work that OTMN has deliberately selected to receive current execution attention. It has:

- a clear current objective, decision, or next action;
- deliberate selection from the current inventory/candidate pool;
- actual current execution attention; and
- a place in the Active Work Queue.

An issue does not become active merely because it is open, interesting, recently created, technically actionable, or high priority in isolation.

> **Open issues are inventory. Active work is selected workload.**

### Active-work authority chain

The current operating cycle is:

```text
Capture → Reconcile → Evaluate → Select → Authorize → Queue → Execute → Reconcile again
```

This is an OTMN operating principle: the organization may capture broadly and learn continuously, but current execution attention is deliberately selected and repeatedly reconciled against what OTMN now knows.

### Authoritative records

Authority is intentionally separated by function:

- **GitHub Issues** are the system of record for individual work items and their acceptance criteria.
- **`05-Operations/OTMN-Active-Work-Queue-v1.0.md`** is the authoritative current record of which work has been selected for execution attention and its sequence.
- **This PM Foundation** documents the underlying lifecycle, triage, and authority rules.
- **START HERE / WHAT'S NEXT** is the recurring decision process used to determine what should receive current attention.

The Active Work Queue is not a second issue tracker. It records current selection and rationale; the individual GitHub issues remain authoritative for the actual work.

### Leaving active work

Active work leaves the active set when:

- **Complete** — the intended work is finished;
- **Defer / Blocked** — work remains valid but cannot or should not continue now;
- **Merge / Supersede** — the work is consolidated into another item;
- **Close** — the work is no longer needed or valid; or
- **Reassessment** — reconciliation determines that another item deserves the execution slot.

When active status changes, the Active Work Queue should be updated and the GitHub issue should reflect the resulting state/disposition.

> **Active status represents current execution attention, not a permanent classification.**

## 10. First PM issues

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
