# OTMN START HERE v0.1 — Operational Procedure

**Related issue:** #38 — OTMN "Where Do I Begin?" v1.0
**Status:** First implementation / proof-of-operation
**Purpose:** Provide the smallest working, repeatable START HERE mechanism using the validated v1.0 decision model.

## 1. Operating Question

When Mark asks:

> **Where do I begin?**

GIA should identify **exactly one** next action from the current OTMN work state and explain why it was selected.

This procedure is intentionally manual/read-only. It does not create scoring, rewrite queues, automate Projects, add labels, create databases, or require additional permissions.

## 2. Inputs

Use only the minimum authoritative information needed to make the decision:

- GitHub Issues for work identity and durable state
- Active Work Queue and issue context for intentional active scope
- Current OTMN roadmap/phase and operating objective
- Issue relationships for prerequisites, dependencies, blockers, and enabling value
- Priority and readiness where authoritative

If a required input cannot be established, report the information gap instead of guessing.

## 3. Procedure

### Step 1 — Establish current context

Identify:

- current OTMN phase;
- current operating objective;
- current active-work scope.

### Step 2 — Build the candidate set

Start with current OTMN work inventory, then retain only work that is intentionally active or otherwise clearly actionable in the current context.

Do **not** treat every open issue as active work.

### Step 3 — Apply the eligibility gate

Exclude any candidate that is:

- closed or completed;
- future/deferred;
- blocked by an unresolved blocker;
- dependent on an incomplete prerequisite;
- outside the current phase without justification;
- awaiting a required human decision; or
- not actionable now.

### Step 4 — Rank remaining candidates

Evaluate eligible candidates in this order:

1. Current-phase alignment
2. Current-objective alignment
3. Enabling/unblocking value
4. Strategic value
5. Priority/importance
6. Readiness/actionability

Do not use raw priority as the sole selector.

### Step 5 — Resolve ties honestly

If candidates remain materially equivalent:

1. Prefer the smallest meaningful actionable progress toward the current objective.
2. If authoritative information still cannot distinguish them, **do not manufacture certainty**.
3. Ask Mark for the required judgment.

### Step 6 — Produce exactly one recommendation

Return one START HERE recommendation unless a genuine unresolved tie or missing authoritative information prevents a responsible choice.

## 4. Output Format

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

## 5. State-Quality Rule

The Active Work Queue expresses intentional active scope, but GitHub Issues remain authoritative for durable work-item state.

If the queue and GitHub materially disagree:

- identify the discrepancy;
- do not silently treat stale queue information as current truth;
- exclude completed/invalid work from executable candidates;
- make the recommendation from authoritative state; and
- flag the queue for reconciliation when the discrepancy affects the result.

## 6. v0.1 Boundary

This implementation deliberately does **not** introduce:

- numerical scoring;
- automatic queue rewriting;
- Project automation;
- new labels;
- a new database;
- new permissions or access;
- dashboards; or
- background automation.

The mechanism is simply:

**Current OTMN state → Active candidates → Eligibility → Ranking → ONE START HERE + explanation**

## 7. Proof of Operation

v0.1 is considered operational when GIA can apply this procedure to the real OTMN state and produce a recommendation that is:

- eligible;
- contextually appropriate;
- unblocked;
- explainable;
- reproducible from the authoritative inputs; and
- honest about ambiguity or missing information.

The next implementation layer should only be added after this procedure demonstrates repeatable value in actual OTMN operation.
