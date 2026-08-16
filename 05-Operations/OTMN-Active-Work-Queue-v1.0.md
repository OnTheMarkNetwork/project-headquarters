# OTMN Active Work Queue v1.0

**Status:** Active  
**Established:** 2026-08-13  
**Last reconciled:** 2026-08-15  
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

### 🟢 NOW — Formalize and implement the Active-Work Authority model

**Issue #68 — Establish Deliberate Active-Work Selection and Current Authority**

Purpose: finalize the current definition of active work, the deliberate selection/authorization transition, the current authority model, the authoritative-record relationship, and the rules for leaving active work.

**Why now:** The current OTMN reconciliation process has demonstrated that open inventory and active workload are different things. The authority model is now defined and needs to be reflected consistently in the operating documentation before the next layer of PM/GIA work is finalized.

**Remaining work:** Review and approve the updated operating documentation, then perform the final conflict check against the existing GIA/PM rules.

**State:** Active.

---

### 🟢 NEXT — Establish the verified Inventory / Active-Work metrics baseline

**Issue #74 — OTMN Inventory / Active-Work Metrics Tracker**

Purpose: establish a lightweight, verifiable way to distinguish total captured inventory from the intentionally constrained active workload.

**Why next:** The current reconciliation run demonstrated that raw issue counts are not sufficient. A repeatable verified snapshot method is needed before relying on inventory/active-work metrics for future START HERE / WHAT'S NEXT decisions.

**Dependency:** The Active-Work Authority model in #68 should be approved first so the metric definitions use the finalized meaning of active work.

**State:** Next.

---

### 🟢 FOLLOWING — Guard against meta-process becoming the workload

**Issue #73 — Meta-Process / Self-Referential Workflow Loops**

Purpose: determine the smallest safeguards needed to improve OTMN's operating system without allowing process design, reconciliation, and optimization to become the primary workload.

**Why following:** The current work has already provided live evidence for the problem. The finalized authority and verified inventory model should be in place before formalizing additional safeguards.

**State:** Following.

---

### 🟢 THEN — Continue GIA identity / scope discovery

**Issue #76 — GIA Identity, Scope, Interface, Intelligence, Automation, Escalation, Voice & Boundaries**

Purpose: determine what GIA actually is within OTMN, what responsibilities it should have, what boundaries it needs, and what interfaces or capabilities are justified by demonstrated use.

**Related discovery family:** #77 (`gia@` interface), #78 (GIDS), #79 (GIA persona/team presence), #80 (emerging GIA principles), and #81 (domain email identity strategy).

**Why then:** The recent GIA/email discoveries are significant, but the organization should resolve the current active-work authority and measurement model before allowing the GIA discovery family to expand into implementation.

**State:** Then / current discovery candidate.

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

These items remain in the GitHub inventory without creating a requirement to work on them now. Related issues may become active later when their prerequisites are satisfied or when fresh reconciliation deliberately selects them.

---

## Completed in the Current Governance Sequence

The following work is now complete and should not remain in the active queue:

- **#9 — Audit OTMN public vs private GitHub information boundaries** — completed August 14, 2026.
- **#36 — Adopt OTMN Repository Visibility Model v1.0** — approved and completed August 14, 2026.
- **#19 — Define the OTMN GitHub Organization Access Model** — completed August 14, 2026.
- **#4 — Determine and configure OTMN GitHub Project PM layer** — completed and validated August 14, 2026.
- **#29 — Document OTMN GitHub Issue Triage Disposition Guide** — completed August 15, 2026; implementation merged via PR #56.
- **#38 — OTMN "Where Do I Begin?" v1.0** — v0.1 implementation/proof completed and merged; retained as an operational mechanism rather than active implementation.

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
#68 ACTIVE-WORK AUTHORITY                   ← NOW
       ↓
#74 VERIFIED INVENTORY / ACTIVE METRICS     ← NEXT
       ↓
#73 META-PROCESS SAFEGUARD                  ← FOLLOWING
       ↓
#76 GIA IDENTITY / SCOPE DISCOVERY          ← THEN
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

The long-term goal is for this queue to become increasingly system-generated from GitHub state, with human judgment remaining authoritative.

---

## Guiding Principles

> **Capture broadly. Commit narrowly.**

> **Open issues are the inventory. Active work is selected workload.**

> **Build the foundation. Prove the workflow. Let the next layer earn its way into existence.**
