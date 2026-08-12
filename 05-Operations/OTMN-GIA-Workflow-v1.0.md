# OTMN GIA Workflow v1.0

## Definition

**GIA = GitHub Item Add.**

GIA is an execution shorthand for adding or changing a GitHub work item through a controlled, minimal workflow.

## Operating sequence

### 1. Resolve scope

Identify the exact repository, artifact, and requested outcome.

### 2. Read before writing

For an existing file, issue, or PR, read the current version first. Preserve unrelated content.

### 3. Choose the smallest correct artifact

Use an issue for work that needs tracking. Use a repository file for durable project knowledge. Use a branch/PR when a substantive repository change needs review.

### 4. Execute

Make only the requested change unless a dependency is necessary to complete it correctly.

### 5. Verify

Re-read or fetch the resulting artifact and confirm that the requested state exists.

### 6. Report

State what changed, where it changed, and any manual action or limitation that remains.

## Safety rules

- Do not guess a repository or path when ambiguity affects correctness.
- Do not overwrite unrelated content.
- Do not claim a Project, label, permission, or setting changed unless it was actually verified.
- Prefer PR review for substantive repository changes.
- Direct-to-main is appropriate only for explicitly authorized low-risk changes or where the operating standard permits it.
- If the connector cannot perform an administrative action, identify the manual step instead of simulating success.

## Current GIA command patterns

- `GIA: Create ...` → create the requested GitHub artifact.
- `GIA: Update ...` → read first, then make a targeted update.
- `GIA: Create issue ...` → create a structured issue with title, description, acceptance criteria, and priority.
- `GIA: Put ... through PR workflow` → branch, change, PR, and verification.

This workflow is intentionally practical. Repeated use should determine which rules deserve promotion into the formal GIA Standard.