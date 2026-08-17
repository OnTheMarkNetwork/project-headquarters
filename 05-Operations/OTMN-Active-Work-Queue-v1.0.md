# OTMN Active Work Queue v1.0

**Status:** Active  
**Established:** 2026-08-13  
**Last reconciled:** 2026-08-16  
**Purpose:** Define the intentionally constrained set of work that should receive current OTMN execution attention.

---

## Operating Rule

> **Open issues are the inventory. The Active Work Queue is the work we are actually choosing to move now.**

Ideas and candidates may accumulate. Active work remains intentionally constrained.

The queue is a ranked execution sequence, not a second issue tracker. GitHub Issues remain the system of record for the individual work items.

## Active-Work Authority

The current OTMN authority model is:

> **Captured work does not become active work automatically. Advancement into active work requires deliberate selection.**

Under the current operating model, **Mark has final authority over what becomes active work**.

GIA/ChatGPT may discover, capture, analyze, reconcile, recommend, and maintain authorized artifacts, but does not independently promote an item into active work unless Mark explicitly authorizes that selection.

The current operating cycle is:

```text
Capture → Reconcile → Evaluate → Select → Authorize → Queue → Execute → Reconcile again
```

The queue records the result of that selection/authorization step. It is therefore the authoritative current record of **what has been selected for execution attention**, while the individual GitHub issues remain authoritative for the actual work.

---

## Current Queue

### 🟢 NOW — Follow the Path: OTMN/Gia Operational Workflow Discovery

**Issue #85 — Follow the Path — OTMN/Gia Operational Workflow Discovery**

Purpose: research the emerging end-to-end OTMN/Gia operating workflow from information capture through processing, routing, action, notification, reporting, learning, and renewed capture.

**Why now:** The recent #74 measurement test and #86 housekeeping test have provided the first meaningful live evidence that the OTMN operating cycle is functioning as an observable system rather than only as a proposed architecture. #85 is now the best next research target because it can consolidate what has actually been demonstrated without prematurely turning the emerging workflow into a formal architecture.

**Current research question:** What is the minimum viable end-to-end Gia workflow that OTMN can implement and test?

**Scope:** Research and observe the workflow. Do not build a larger workflow platform or formal architecture unless the evidence demonstrates that a new layer is needed.

**State:** Selected as the current NOW item through the August 16, 2026 reconciliation.

---

### 🟢 NEXT — Guard against meta-process becoming the workload

**Issue #73 — Identify and Prevent OTMN Meta-Process / Self-Referential Workflow Loops**

Purpose: determine the smallest safeguards needed to improve OTMN's operating system without allowing process design, reconciliation, and optimization to become the primary workload.

**Why next:** The #74 and #86 tests now provide concrete evidence for evaluating this risk. OTMN is generating substantial new discovery while keeping active work intentionally constrained. #73 can now evaluate whether the existing active-work authority, reconciliation, and capture/commit principles are already sufficient safeguards before any additional governance is created.

**Scope:** Research the observed behavior and identify the minimum useful safeguard, if one is actually needed. Do not create an elaborate governance layer.

**State:** Next.

---

### 🟢 FOLLOWING — Continue GIA identity / scope discovery

**Issue #76 — GIA Identity, Scope, Interface, Intelligence, Automation, Escalation, Voice & Boundaries**

Purpose: determine what GIA actually is within OTMN, what responsibilities it should have, what boundaries it needs, and what interfaces or capabilities are justified by demonstrated use.

**Why following:** #85 and #73 can now provide additional evidence about GIA's actual operating role and boundaries before the larger identity/scope research is undertaken. The related #77, #78, #79, #80, and #81 discoveries remain useful inputs but do not automatically become active work.

**State:** Following.

---

## Recently Validated / Not Active

### #74 — OTMN Inventory / Active-Work Metrics Tracker

The lightweight measurement method has now been tested against multiple verified GitHub snapshots. The test demonstrated that inventory can change in knowledge/composition while active workload remains deliberately constrained, and that numeric counts are most useful when paired with active identity/state changes and material observations.

**Disposition:** Validated / Observe. No dashboard, spreadsheet, automation, or additional reporting layer is currently justified.

### #86 — Gia Project Housekeeping — Health Check Discovery

The first manual housekeeping review has been performed. Its most useful demonstrated function was identifying drift between GitHub's recorded operating state and the actual current state, particularly the stale Active Work Queue.

**Disposition:** Initial test complete; preserve the finding and do not automate yet.

### #68 — Establish Deliberate Active-Work Selection and Current Authority

Completed through the finalized Active-Work Authority documentation and operating-cycle implementation.

**Disposition:** Completed; no longer active work.

---

## Deliberately NOT Active

The following remain valid inventory but are not current execution priorities:

- #18 — OTMN Versioning Standards
- #22 — Google Workspace complementary layer
- #24 — Roadmap Info section
- #26 — Ideas Can Be Unlimited content
- #27 — Author / Creator Intake research
- #31 — Persona Research
- #32 — Build The Network Content
- #33 — Necessity Article
- #37 — Repository Lifecycle Standard
- #39 — ChatGPT Knowledge Migration & Archive
- #40 — Private-repo GIA access boundary
- #53 — Nomenclature Idea Discussion
- #57 — Clean Up OTMN Manifesto Formatting
- #64 — Capture Broadly. Commit Narrowly
- #65 — Inventory Is Not Workload
- #66 — Preserve Reusable Insights
- #67 — Knowing What Not to Build Yet
- #69 — GIA/gia Usage and Shorthand Convention
- #70 — 87/11 metrics
- #71 — Idea/content inventory tool
- #72 — Product discovery pattern
- #75 — Build the System that Builds the System
- #77 — `gia@` OTMN interface
- #78 — GIDS research
- #79 — GIA Persona / Team Presence
- #80 — Emerging GIA principles / working concepts
- #81 — Domain email identity strategy
- #84 — Founder Talk discovery
- #87 — Weekly Management & Intelligence Reporting discovery
- #89 — Sensitive Information / Classification & Access Architecture research

These items remain in the GitHub inventory without creating a requirement to work on them now. Related issues may become active later when their prerequisites are satisfied or when fresh reconciliation deliberately selects them.

---

## Completed in the Current Governance Sequence

The following work is complete and should not remain in the active queue:

- **#9 — Audit OTMN public vs private GitHub information boundaries** — completed August 14, 2026.
- **#36 — Adopt OTMN Repository Visibility Model v1.0** — approved and completed August 14, 2026.
- **#19 — Define the OTMN GitHub Organization Access Model** — completed August 14, 2026.
- **#4 — Determine and configure OTMN GitHub Project PM layer** — completed and validated August 14, 2026.
- **#29 — Document OTMN GitHub Issue Triage Disposition Guide** — completed August 15, 2026; implementation merged via PR #56.
- **#38 — OTMN "Where Do I Begin?" v1.0** — v0.1 implementation/proof completed and merged; retained as an operational mechanism rather than active implementation.
- **#68 — Establish Deliberate Active-Work Selection and Current Authority** — completed August 16, 2026.

---

## Queue Rules

1. **The queue is intentionally small.** Do not activate work merely because an issue is open.
2. **Dependencies matter.** Do prerequisite work before downstream work when the dependency is real.
3. **Roadmap position matters.** Current Phase 1 completion takes precedence over future product work.
4. **Unblocking value matters.** Prefer work that enables multiple important downstream actions.
5. **Deferred work stays deferred.** Do not pull future ideas forward simply because the queue becomes interesting.
6. **One "NOW" item is preferred.** Additional items are ordered NEXT/FOLLOWING/THEN rather than treated as simultaneous active work unless real parallel execution demonstrates a need.
7. **GitHub Issues remain authoritative.** This document records the current queue and rationale; it does not duplicate issue acceptance criteria.
8. **Review the queue after meaningful work sessions.** Completed, blocked, newly discovered, or reprioritized work should cause the queue to be reconsidered.
9. **Selection is deliberate.** The queue must reflect an explicit active-work decision, not automatic promotion from the issue inventory.
10. **Validated work does not automatically become a new project layer.** A successful test should first be observed and reconciled before additional tooling, automation, or standards are created.

---

## Current Execution Sequence

```text
RECONCILE CURRENT INVENTORY                 ✅ COMPLETE
       ↓
STALE / REVIEW DISPOSITION                  ✅ COMPLETE
       ↓
IDENTIFY REAL ACTIVE CANDIDATES             ✅ COMPLETE
       ↓
FRESH START HERE / WHAT'S NEXT              ✅ COMPLETE
       ↓
#68 ACTIVE-WORK AUTHORITY                   ✅ COMPLETE
       ↓
#74 INVENTORY / ACTIVE-WORK MEASUREMENT     ✅ VALIDATED / OBSERVE
       ↓
#86 FIRST MANUAL HOUSEKEEPING TEST          ✅ COMPLETE / OBSERVE
       ↓
FRESH ACTIVE-WORK QUEUE RECONCILIATION      ← CURRENT
       ↓
#85 FOLLOW THE PATH                         ← NOW
       ↓
#73 META-PROCESS SAFEGUARD                  ← NEXT
       ↓
#76 GIA IDENTITY / SCOPE DISCOVERY          ← FOLLOWING
       ↓
RECONCILE AGAIN AFTER MEANINGFUL DISCOVERY
```

---

## Relationship to OTMN Operating Rhythm

At the end of each meaningful work session:

1. Record what changed.
2. Review the current inventory and Active Work Queue.
3. Mark completed or blocked work in GitHub.
4. Reconcile stale or changed items when new knowledge materially affects them.
5. Re-rank the queue if dependencies or priorities changed.
6. Identify the next **NOW** item through deliberate selection and authorization.

The August 16 reconciliation demonstrates this cycle in practice: #68 completed, #74 validated, #86 tested, the queue was found stale, and the next deliberate selection is #85.

The long-term goal is for this queue to become increasingly system-generated from GitHub state, with human judgment remaining authoritative.

---

## Guiding Principles

> **Capture broadly. Commit narrowly.**

> **Open issues are the inventory. Active work is selected workload.**

> **Build the foundation. Prove the workflow. Let the next layer earn its way into existence.**

> **Validated does not mean expanded. Observe before adding the next layer.**
