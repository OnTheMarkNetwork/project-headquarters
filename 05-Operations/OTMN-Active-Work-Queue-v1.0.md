# OTMN Active Work Queue v1.0

**Status:** Active  
**Established:** 2026-08-13  
**Last reconciled:** 2026-08-14  
**Purpose:** Define the intentionally constrained set of work that should receive current OTMN execution attention.

---

## Operating Rule

> **Open issues are the inventory. The Active Work Queue is the work we are actually choosing to move now.**

Ideas and candidates may accumulate. Active work remains intentionally constrained.

The queue is a ranked execution sequence, not a second issue tracker. GitHub Issues remain the system of record for the individual work items.

---

## Current Queue

### 🟢 NOW — Define the OTMN GitHub Organization Access Model

**Issue #19 — Define the OTMN GitHub Organization Access Model**

Purpose: define the operational access layer that accompanies the adopted Repository Visibility Model, including the distinction between human GitHub access and ChatGPT/GIA connected-tool access.

**Why now:** #9 (public/private information-boundary audit), #36 (Repository Visibility Model adoption), and #4 (PM visualization layer) are complete. #19 is the remaining active governance item in this sequence and is now complete as well in the live issue state; this queue update records the reconciliation point and identifies the next work below.

**Status at reconciliation:** Completed in GitHub on August 14, 2026. The durable access model is recorded in `04-Standards/OTMN-GitHub-Organization-Access-Model-v1.0.md`.

---

### 🟢 NEXT — Verify private-repository GIA access boundary when the first restricted repository exists

**Issue #40 — Verify private-repository GIA access boundary when first restricted repository is created**

Purpose: verify the effective repository-level permissions of the ChatGPT/GIA GitHub App when OTMN has its first Team or Founder private repository.

**Dependency:** A restricted OTMN repository must exist before this verification can be performed meaningfully.

**Status:** Deferred until the prerequisite real-world condition exists. This is not current execution work while all OTMN organization repositories remain public.

---

### 🟢 FOLLOWING — Continue Phase 1 operational use and reconciliation

**Issue #38 — OTMN "Where Do I Begin?" v1.0**

Purpose: maintain and exercise the proven START HERE mechanism as part of the OTMN operating rhythm.

**Status:** The v0.1 implementation and proof have been completed and merged. Continued use is operational rather than a new implementation blocker.

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

## Completed in the Current Governance Sequence

The following work is now complete and should not remain in the active queue:

- **#9 — Audit OTMN public vs private GitHub information boundaries** — completed August 14, 2026.
- **#36 — Adopt OTMN Repository Visibility Model v1.0** — approved and completed August 14, 2026.
- **#19 — Define the OTMN GitHub Organization Access Model** — completed August 14, 2026.
- **#4 — Determine and configure OTMN GitHub Project PM layer** — completed and validated August 14, 2026.
- **#38 — OTMN "Where Do I Begin?" v1.0** — v0.1 implementation/proof completed and merged; retained above for operational use rather than active implementation.

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
#9  PUBLIC / PRIVATE AUDIT       ✅ COMPLETE
       ↓
#36 VISIBILITY MODEL             ✅ COMPLETE
       ↓
#19 ACCESS MODEL                ✅ COMPLETE
       ↓
#4  PM / PROJECT VISUALIZATION  ✅ COMPLETE
       ↓
#38 START HERE v0.1              ✅ PROVEN / MERGED
       ↓
#40 PRIVATE-REPO GIA TEST        ⏸ WAITING FOR FIRST PRIVATE REPO
       ↓
CONTINUED OPERATING USE / PHASE 1 CLOSEOUT
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
