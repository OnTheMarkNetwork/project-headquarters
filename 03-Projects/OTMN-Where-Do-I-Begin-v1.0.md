# OTMN "Where Do I Begin?" Decision Specification v1.0

**Issue:** #38 — Where Do I Begin?
**Status:** Design specification — pending review
**Purpose:** Define the minimum decision model GIA can use to identify the highest-value, unblocked, contextually appropriate next action for OTMN.

## 1. Purpose

"Where Do I Begin?" is a decision layer for the OTMN operating system.

It should answer:

> **Given OTMN's current authoritative work state and operating context, what is the highest-value, unblocked, contextually appropriate next action — and why?**

It is not a replacement for GitHub Issues, the Active Work Queue, or GitHub Projects. It interprets those sources to produce an explainable START HERE recommendation.

## 2. Governing Principle

> **First eliminate what cannot or should not be done. Then choose the work that most directly advances what OTMN has intentionally decided matters now.**

The mechanism must follow the OTMN GIA Standard, including the Minimum Necessary Access, immediate-progress, and no-manufactured-certainty principles.

## 3. Minimum Information Contract

### Required

1. Work-item identity
2. Work-item state
3. Active/future disposition
4. Current OTMN phase
5. Current operating objective/context
6. Prerequisites
7. Dependencies
8. Blockers
9. Enabling/unblocking value
10. Priority/importance
11. Readiness/actionability

### Potentially useful but not yet proven required

- Project execution status
- Area/project context
- Target/date
- Historical momentum or continuity

### Not currently required

- Direct access to the live GitHub Project Board/Table

The minimum contract is intentionally source-oriented rather than Project-field-oriented. A Project field is only a dependency if testing demonstrates that the underlying information is necessary to make a reliable recommendation.

## 4. Authoritative Sources

| Information | Primary source | Role |
|---|---|---|
| Work identity/state | GitHub Issues | Authoritative work inventory and state |
| Active/future disposition | Active Work Queue + issue context | Defines intentional active scope |
| Current phase/objective | Roadmap + current operating context | Defines what matters now |
| Prerequisites/dependencies/blockers | Issues and durable documentation | Establishes eligibility |
| Enabling/unblocking value | Issue rationale and relationships | Establishes leverage |
| Priority | Issue/Project where authoritative | Ranking factor, not sole decision-maker |
| Execution status | Project if needed | Supplemental execution context |

## 5. Decision Pipeline

The decision occurs in two broad stages: **eligibility** followed by **ranking**.

```text
ALL WORK
   ↓
ELIGIBILITY GATE
   ↓
eligible candidates
   ↓
CURRENT CONTEXT ALIGNMENT
   ↓
ENABLING / UNBLOCKING VALUE
   ↓
STRATEGIC VALUE
   ↓
PRIORITY + READINESS
   ↓
ONE WINNER → START HERE
        OR
TRUE TIE → ASK MARK
```

## 6. Eligibility Gate

A candidate should be excluded from START HERE consideration when it is:

- closed or completed;
- explicitly deferred or future-only;
- blocked by an unresolved blocker;
- dependent on an incomplete prerequisite;
- outside the current phase without a justified reason;
- awaiting a required human decision; or
- not actual actionable work.

Eligibility happens **before ranking**. Important work that is not currently eligible should not outrank eligible work.

## 7. Ranking Hierarchy

Among eligible candidates, evaluate in this order:

### 7.1 Current-phase alignment

Does the work advance the phase OTMN is currently in?

### 7.2 Current-objective alignment

Does it directly advance what OTMN has intentionally decided matters now?

When two otherwise eligible items are comparable, prefer the item that is closest to the current objective and produces the most immediate useful progress toward it.

### 7.3 Enabling / unblocking value

Does completing the item unlock, enable, or materially simplify other valuable work?

### 7.4 Strategic value

How materially does the work advance OTMN's broader objectives?

### 7.5 Priority / importance

How important is the work relative to other eligible candidates?

Priority is a ranking factor, not an automatic START HERE selector.

### 7.6 Readiness / actionability

Can meaningful progress be made now, with the available information and without inventing missing decisions?

## 8. Tie-Breaking

If two candidates remain comparable after the ranking hierarchy:

1. Prefer the candidate that produces the smallest meaningful actionable progress toward the current objective.
2. If authoritative information still cannot establish a meaningful difference, **do not manufacture certainty**.
3. State that the candidates are materially equivalent based on the available authoritative information and request human judgment from Mark.

The mechanism should never invent a numerical distinction merely to force a winner.

## 9. Human Judgment Boundary

GIA should recommend, explain, and identify ambiguity. It should not silently resolve decisions that require Mark's judgment.

A genuine tie or an unresolved human decision is an explicit outcome of the mechanism, not a system failure.

## 10. Output Specification

A START HERE recommendation should be concise but explainable:

```text
🟢 START HERE

Issue: #XX — [Title]

Why:
[Why this is the best current choice.]

Current objective:
[What OTMN is intentionally advancing now.]

Eligibility:
✓ Unblocked
✓ Prerequisites satisfied
✓ Current-phase work
✓ Actionable

Value:
[What this advances or unlocks.]

Next action:
[Smallest meaningful step to begin.]

After this:
[Likely next candidate, if determinable.]

Confidence:
[Authoritative / Conditional / Human decision required]
```

## 11. Relationship to Existing OTMN Layers

### GitHub Issues

The authoritative work inventory. Issues establish what work exists and its durable state/context.

### Active Work Queue

The intentional active scope: what OTMN has decided it is working on now. It is not a replacement issue tracker.

### GitHub Projects

The execution and visualization layer. Project fields may supplement the decision model but are not automatically required inputs.

### "Where Do I Begin?"

The decision layer that interprets the current state and produces the START HERE recommendation.

## 12. Access and Security Boundary

The mechanism follows the GIA Minimum Necessary Access Principle.

GIA should use the minimum authoritative information necessary to perform the decision. If required information is inaccessible because of an intentional security or access boundary, GIA should identify the capability gap rather than weakening or bypassing the boundary by default.

Therefore, Project visibility or permissions must not be changed merely for convenience. Additional access requires an intentional, evidence-based decision.

## 13. Validation Criteria

The specification must be tested against real OTMN decisions before implementation is considered complete.

Required tests include:

1. **Obvious prerequisite:** a prerequisite must beat a downstream item even when the downstream item has greater apparent priority.
2. **Multiple eligible candidates:** the model must distinguish candidates using context, enablement, value, priority, and readiness.
3. **Future high-value work:** important but premature work must be excluded from START HERE.
4. **Genuine tie:** the model must refuse to manufacture a distinction and request human judgment.
5. **Missing information:** the model must identify a capability/data gap rather than silently guessing.
6. **Stale queue:** the model must recognize when a written queue no longer matches authoritative GitHub state.

The design/discovery tests performed during #38 produced the current contract and rules. These tests should be retained as examples when the mechanism is implemented.

## 14. v1.0 Scope Boundary

This specification defines the decision model. It does **not** yet implement automatic scoring, automatic queue rewriting, Project automation, new labels, new databases, or additional access permissions.

The first implementation should remain minimal and explainable.

## 15. Success Criteria

#38 is ready to move from design into implementation when the model can:

- identify eligible work correctly;
- select the work that most directly advances the current objective;
- account for enabling/unblocking value;
- avoid treating raw priority as the sole selector;
- explain why the selected item beats reasonable alternatives;
- identify genuine ambiguity instead of manufacturing certainty; and
- operate using the minimum authoritative information necessary.
