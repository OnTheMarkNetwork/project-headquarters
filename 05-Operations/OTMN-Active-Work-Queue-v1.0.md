# OTMN Active Work Queue v1.0

**Status:** Active  
**Established:** 2026-08-13  
**Purpose:** Define the intentionally constrained set of work that should receive current OTMN execution attention.

---

## Operating Rule

> **Open issues are the inventory. The Active Work Queue is the work we are actually choosing to move now.**

Ideas and candidates may accumulate. Active work remains intentionally constrained.

The queue is a ranked execution sequence, not a second issue tracker. GitHub Issues remain the system of record for the individual work items.

---

## Current Queue

### 🟢 NOW — Finish Phase 1 inventory/governance reconciliation

**Issue #9 — Audit OTMN public vs private GitHub information boundaries**

Purpose: finish/verify the remaining audit work and close the loop against the Privacy & Transparency Standard and Repository Visibility Model.

**Why now:** This is a prerequisite for confidently adopting the visibility model and proceeding with the access model.

---

### 🟢 NEXT — Adopt the repository visibility baseline

**Issue #36 — Adopt OTMN Repository Visibility Model v1.0**

Purpose: formally move the existing visibility model from proposed to approved after reconciliation with the privacy standard and current repositories.

**Dependency:** #9

---

### 🟢 FOLLOWING — Define the access layer

**Issue #19 — Define the OTMN GitHub Organization Access Model**

Purpose: determine who can access each repository visibility tier, including the distinction between human GitHub access and ChatGPT/GIA connected-tool access.

**Dependency:** #36

---

### 🟢 THEN — Establish the PM visualization layer

**Issue #4 — Determine and configure OTMN GitHub Project PM layer**

Purpose: establish the organization-level project views needed to visualize the work queue and operating state.

**Dependency:** Current foundation/governance reconciliation. Manual GitHub Project configuration may be required because the connected GitHub tooling does not currently expose project creation/configuration.

---

### 🟢 AFTER THE QUEUE PROVES ITSELF — Build the decision mechanism

**Issue #38 — OTMN "Where Do I Begin?" v1.0**

Purpose: turn the trusted active inventory into an explainable START HERE recommendation.

**Dependency:** A trustworthy active queue and sufficient real-world use to test the decision model.

---

## Deliberately NOT Active

The following remain valid inventory but are not current execution priorities:

- #15 — Do not design the next layer until needed
- #16 — Do not expand GIA rules prematurely
- #17 — Different work types need different intake structures
- #18 — OTMN Versioning Standards
- #20 — OTMN Core Idea
- #21 — Add OTMN Core Idea to Manifesto
- #22 — Google Workspace complementary layer
- #23 — Idea → Candidate → Work lifecycle
- #24 — Roadmap Info section
- #25 — Idea & Work Philosophy in Manifesto
- #26 — Ideas Can Be Unlimited content
- #27 — Author / Creator Intake research
- #28 — Website MVP historical audit archive
- #29 — Issue Triage Disposition Guide
- #30 — Mobile Capture selections
- #31 — Persona Research
- #32 — Build The Network Content
- #33 — Necessity Article
- #37 — Repository Lifecycle Standard
- #39 — ChatGPT Knowledge Migration & Archive

These items remain in the GitHub inventory without creating a requirement to work on them now.

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

---

## Current Execution Sequence

```text
ROADMAP AUDIT                    ✅ COMPLETE
       ↓
ISSUE / INVENTORY CLEANUP        ✅ PASS 1 COMPLETE
       ↓
#9  PUBLIC / PRIVATE AUDIT       ← NOW
       ↓
#36 VISIBILITY MODEL             ← NEXT
       ↓
#19 ACCESS MODEL                 ← FOLLOWING
       ↓
#4  PM / PROJECT VISUALIZATION   ← THEN
       ↓
#38 WHERE DO I BEGIN?            ← AFTER QUEUE PROVES ITSELF
       ↓
PHASE 1 COMPLETE / PHASE 2
```

---

## Relationship to OTMN Operating Rhythm

At the end of each meaningful work session:

1. Record what changed.
2. Review the current queue.
3. Mark completed or blocked work in GitHub.
4. Re-rank the queue if dependencies or priorities changed.
5. Identify the next **NOW** item.

The long-term goal is for this queue to become increasingly system-generated from GitHub state, with human judgment remaining authoritative.

---

## Guiding Principle

> **Build the foundation. Prove the workflow. Let the next layer earn its way into existence.**
