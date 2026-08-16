# OTMN Operating Principles v1.0

**Status:** Current working standard
**Scope:** How OTMN captures, evaluates, selects, executes, and re-evaluates work

## Purpose

Define the small set of operating principles that have been demonstrated through actual OTMN work and are durable enough to guide future decisions.

These principles describe **how OTMN works**. They complement:

- the **OTMN Core Idea**, which describes what OTMN fundamentally does;
- the **OTMN Manifesto**, which describes why OTMN exists and what it believes; and
- operational documentation, which describes the procedures used to apply these principles.

This document should grow only when repeated OTMN use demonstrates a durable principle worth preserving.

## Principle 1 — Capture Broadly. Commit Narrowly.

OTMN should be willing to capture useful ideas, observations, questions, opportunities, and discoveries without treating every captured item as a commitment to execute it.

> **Ideas can be unlimited. Candidates can accumulate. Active work must remain intentionally constrained.**

Capture preserves knowledge. Deliberate selection protects execution capacity.

## Principle 2 — Active Work Is Deliberately Selected

Captured work does not become active work automatically.

> **Open issues are the inventory. Active work is selected workload.**

Advancement into active work requires deliberate selection and authorization under the current OTMN operating model. An item is not active merely because it is open, interesting, recently created, technically actionable, or high priority in isolation.

## Principle 3 — The OTMN Operating Cycle

OTMN currently operates through a recurring cycle:

```text
Capture → Reconcile → Evaluate → Select → Authorize → Queue → Execute → Reconcile again
```

Each stage has a distinct purpose:

- **Capture** — preserve useful ideas, work, questions, discoveries, and opportunities.
- **Reconcile** — compare the inventory with what OTMN now knows; identify stale, obsolete, duplicated, or changed work without discarding useful history.
- **Evaluate** — determine what still matters, what has earned candidate status, what is blocked or deferred, and what deserves consideration.
- **Select** — choose the small set of work that actually deserves current attention.
- **Authorize** — under the current model, Mark has final authority over what becomes active work.
- **Queue** — record the selected work and execution sequence in the Active Work Queue.
- **Execute** — perform the selected work using the appropriate GitHub/project workflow.
- **Reconcile again** — after meaningful work or discovery, reassess the current state because new knowledge may change what deserves attention.

This cycle is intentionally iterative. Reconciliation is not merely cleanup; it is part of how OTMN converts new knowledge into better decisions.

## Principle 4 — Preserve Useful History

When an issue or idea becomes stale, obsolete, superseded, or no longer active, OTMN should distinguish that state from the loss of the underlying knowledge.

> **Stale work may cease to be current work without ceasing to be useful history.**

Reconciliation should therefore preserve relevant context whenever practical while allowing outdated execution commitments to be closed, deferred, merged, or superseded.

## Principle 5 — Let the Next Layer Earn Its Way Into Existence

OTMN should not build additional process, taxonomy, automation, documentation, or infrastructure merely because it can be imagined.

> **Build the foundation. Prove the workflow. Let the next layer earn its way into existence.**

Repeated real-world use should demonstrate the need before a new layer becomes part of the operating system.

## Current Authority

The detailed active-work authority rules are documented in:

- `05-Operations/OTMN-GitHub-PM-Foundation-v1.0.md`
- `05-Operations/OTMN-Active-Work-Queue-v1.0.md`

The individual GitHub issue remains the system of record for its own work item and acceptance criteria.

## Change Rule

These principles are current operating rules, not immutable doctrine. A principle may be revised when sustained OTMN use demonstrates that the current wording no longer accurately represents how OTMN works.

Changes should preserve useful history and explain why the principle changed.
