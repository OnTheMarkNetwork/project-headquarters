# OTMN Versioning Standard v1.0

**Status:** Proposed working standard

## Purpose

This document defines the minimum versioning convention for OTMN standards, procedures, processes, and manuals.

The goal is consistent, understandable versioning without creating unnecessary version-management machinery.

## Version Format

OTMN documents use:

**vMAJOR.MINOR.PATCH**

Examples:

- `v1.0` — initial approved version
- `v1.5` — meaningful update within the same major version
- `v1.1.1` — small corrective or clarifying update
- `v2.0` — major revision that materially changes the document's structure, purpose, or operating meaning

When the PATCH component is not needed, OTMN may use the shorter `vMAJOR.MINOR` form.

## Version Rules

### MAJOR

Increase the major version when a revision materially changes the document's purpose, structure, or established operating meaning.

### MINOR

Increase the minor version when adding or revising substantive content without materially changing the established purpose or operating meaning.

### PATCH

Increase the patch version for small corrections, clarifications, or other changes that do not materially alter the document's meaning.

## Naming

Where practical, the approved version is included in the filename:

`OTMN-[Document Name]-v1.0.md`

The document's version should also be stated within the document when the document is intended to function as an approved standard, procedure, process, or manual.

## Scope

This standard applies to OTMN-controlled standards, procedures, processes, and manuals.

It does not prescribe GitHub release numbering, software package versioning, or other external versioning systems unless OTMN later establishes a specific need for that guidance.

## Operating Principle

Use the smallest version change that accurately describes what changed.

Versioning should communicate change, not create bureaucracy.

If a future case exposes a genuine ambiguity, the standard may be revised rather than adding rules preemptively.
