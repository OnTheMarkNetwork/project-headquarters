# Issue #74 — Research Finding

**Title:** OTMN Inventory / Active-Work Metrics Tracker  
**Status:** Research finding documented; operational validation phase  
**Research issue:** #74  
**Date:** 2026-08-16

## Purpose

This document records what Issue #74 has discovered about the smallest useful way to understand OTMN inventory and active work over time.

It is a **research finding**, not a v1.0 standard, dashboard specification, scoring model, or automation design.

The purpose is to preserve the evidence and boundaries discovered during the research so the method can now be used in real OTMN work.

> **Do not build the dashboard because the numbers are interesting. Find the smallest useful measurement first.**

## Research question

Can OTMN maintain a trustworthy understanding of its inventory and active workload with a measurement method that is small, repeatable, and useful without creating a new reporting bureaucracy?

## What the research discovered

### 1. Inventory is not workload

The number of open issues is not the same thing as the amount of active work.

An issue may be valid inventory without being selected for current execution attention.

> **Open issues are inventory. Active work is selected workload.**

Active work requires deliberate selection and authorization rather than being inferred from issue existence, age, priority, or technical actionability.

### 2. Freshness is evidence, not truth

GitHub provides useful evidence signals:

- created/updated timestamps;
- open/closed state;
- issue activity;
- labels and content changes.

Those signals do not, by themselves, establish semantic freshness or relevance.

The research identified these useful states:

- **Current / Verified** — deliberately established as current.
- **Current / Revalidated** — older information deliberately reconciled and confirmed current.
- **Recorded / Aging** — retained information whose current validity has not recently been established.
- **Requires Revalidation** — current use is uncertain or the original framing may no longer reflect reality.
- **Historical** — intentionally retained as a record of a prior state, decision, or event.

Importantly:

> **Closed does not automatically mean historical.**

Historical status is semantic, not mechanical.

### 3. Freshness and active selection answer different questions

The two dimensions should remain separate:

**Freshness / Relevance:**
> Can we trust this information as current enough to use?

**Active / Non-Active:**
> Has OTMN deliberately committed execution attention to it?

Combining them provides useful operational context without collapsing them into one taxonomy.

### 4. Change over time is more useful than a single number

A snapshot tells us what the inventory looks like now.

Comparing snapshots tells us what changed.

The research showed that inventory movement can be interpreted as events such as:

- **Created**
- **Closed / Complete**
- **Reclassified / Updated**
- **Deferred / Non-active**
- **Revalidated**
- **Activated**

These are change events, not additional permanent issue classifications.

A state change is not necessarily a workload change. For example, revalidation can change confidence without changing workload, while activation changes committed workload without necessarily changing total inventory.

### 5. A later snapshot can be maintained incrementally

A complete later snapshot cannot always be inferred from GitHub mechanics alone.

However, the research found that a full manual re-audit is unnecessary when most state can be carried forward and only ambiguous or semantically changed items are reconciled.

The useful model is:

> **Previous verified snapshot + observable changes + targeted reconciliation → current verified snapshot**

This is **incremental reconciliation**, not automatic reconstruction by assumption.

### 6. Targeted reconciliation is the efficiency boundary

The method remains useful because reconciliation is selective.

Unambiguous state can be carried forward. Only items whose semantic state cannot safely be established from recorded evidence require deliberate reconciliation.

The operational warning condition is:

> **If reconciliation becomes nearly as expensive as rebuilding the snapshot, the method has reached its efficiency boundary.**

### 7. The method is repeatable before all organizational judgment is formalized

A future GIA process or another operator can reproduce the mechanical portion of the method from the verified snapshot and observable GitHub changes.

Some semantic decisions still require organizational context. That is a boundary between **measurement mechanics** and **organizational judgment**, not evidence that another measurement dimension is required.

The correct behavior when evidence is insufficient is:

> **Flag for reconciliation — do not infer.**

### 8. The method can be documented compactly

The research tested whether the method required a large playbook. It did not.

The smallest useful recurring procedure is:

1. **Start with the last verified snapshot.**
2. **Identify observable changes** since that snapshot.
3. **Carry forward unambiguous state.**
4. **Flag semantic uncertainty rather than infer it.**
5. **Targeted-reconcile only flagged items.**
6. **Compare the resulting snapshot** with the previous one.
7. **Interpret the changes** as inventory/workflow events.
8. **Record the new verified snapshot.**

The core decision rules are:

> **Known → Carry forward.**  
> **Ambiguous → Reconcile.**  
> **Unknown → Do not infer.**

## Smallest useful operating method

The research currently supports this recurring method:

```text
SNAPSHOT
   ↓
RECORD CHANGES
   ↓
TARGETED RECONCILE
   ↓
COMPARE
   ↓
INTERPRET
   ↓
NEXT SNAPSHOT
```

This feeds the broader OTMN operating cycle:

```text
Capture → Reconcile → Evaluate → Select → Authorize → Queue → Execute → Reconcile again
```

The measurement method and the execution workflow are related but should not be confused. The measurement method helps establish what is current and what changed; it does not replace the decision and authority process for selecting active work.

## What the research did not justify

The research did **not** establish a need for:

- a dashboard;
- a numeric score;
- a freshness score;
- automatic stale timers;
- an automated semantic-classification system;
- a separate reporting database;
- a larger issue-label taxonomy;
- a large reconciliation playbook; or
- a new bureaucracy layer.

None of these should be built merely because they are possible.

## Current boundary

The method still depends on human or GIA judgment when GitHub evidence is insufficient to establish semantic truth.

That boundary is intentional.

> **GitHub events maintain the record; reconciliation establishes current truth.**

The method also does not attempt to encode every piece of tacit organizational knowledge simply to make the process appear fully autonomous.

## Current research conclusion

Issue #74 has provided substantial evidence that the following is currently the **smallest useful measurement method we can justify** for OTMN inventory and active work:

> **Snapshot → Record Changes → Targeted Reconcile → Compare → Interpret → Next Snapshot**

The method is:

- useful for distinguishing inventory from active workload;
- able to incorporate freshness/relevance without scoring;
- able to explain meaningful change over time;
- incrementally maintainable;
- selectively reconcilable;
- repeatable at the process level; and
- compact enough to document without creating a new bureaucracy layer.

This is a **provisional research finding**, not a claim of permanent sufficiency.

## What happens next

The research phase now transitions from hypothetical stress testing to real repeated OTMN use:

> **Use → Observe → Reconcile → Learn**

The method should be applied during normal OTMN/GIA operation rather than expanded through additional hypothetical process design.

If real work exposes a recurring failure that the method cannot handle, **Issue #74 should reopen around that specific failure**.

If repeated use does not expose such a failure, confidence in the method increases through operational evidence.

Only after that validation should OTMN consider whether the method has earned formalization into a future standard or framework.

## Reopening rule

#74 should reopen if real-world use demonstrates a recurring problem that cannot be handled by the existing method without adding disproportionate process overhead or an unjustified new measurement dimension.

A proposed new metric, state, automation, or reporting layer should therefore answer:

1. What demonstrated failure does it solve?
2. Why can the existing method not handle that failure?
3. What evidence shows the added structure is worth its cost?

> **Let the next layer earn its way into existence.**

## Research sequence

**Discover → Test → Prove → Then build.**

#74 has moved from **researching the measurement method** to **testing the method in real OTMN operation**.
