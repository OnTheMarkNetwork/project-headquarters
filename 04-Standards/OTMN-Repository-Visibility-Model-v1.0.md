# OTMN Repository Visibility Model v1.0

**Status:** Approved — OTMN Standard v1.0
**Owner:** OTMN Project Headquarters
**Scope:** OTMN GitHub organization and repositories

## Purpose

Provide a simple organization-wide rule for deciding where OTMN information belongs based on who should have access to it.

## Rule

> **Public information belongs in public repositories.**
>
> **Team information belongs in team-access private repositories.**
>
> **Founder information belongs in founder-access private repositories.**
>
> **Personal information belongs outside the organization or in a repository restricted exclusively to the owner.**

## Operating Model

| Information type | Appropriate location |
|---|---|
| Public | Public repository |
| Team | Team-access private repository |
| Founder | Founder-access private repository |
| Personal | Outside the organization, or owner-only private repository |

## Relationship to Privacy & Transparency

This model is the repository-level application of the OTMN Privacy & Transparency Standard v1.0.

The Privacy & Transparency Standard defines information classification, privacy, sensitive-information handling, secrets protection, and remediation. This Visibility Model provides the simpler repository-placement decision that follows from those requirements.

The two standards are complementary and should not be interpreted as competing classification systems.

When information is ambiguous, the Privacy & Transparency Standard's restricted-by-default guidance applies until the appropriate owner or administrator resolves the classification.

## Principle

Use the simplest repository visibility that correctly protects the information. Do not create a larger governance system when a clear visibility boundary is sufficient.

This model is intentionally lightweight. More detailed classification or governance should be introduced only when real OTMN work demonstrates that this rule is insufficient.

## Application

This model should guide:

- Repository creation and selection
- Placement of documentation and project information
- GitHub organization structure
- OTMN team and founder workspaces
- ChatGPT/GIA decisions about where information should be stored
- Reviews of public versus private information boundaries

Before creating or repurposing a repository, its intended visibility should be considered against the information it is expected to contain.

## Current OTMN Repositories

As of August 14, 2026, the OTMN organization repositories reviewed under this standard are intentionally public and are consistent with their current purposes and contents.

Future repositories should be assigned an intentional visibility level before use, and a repository's visibility should be reconsidered when its purpose or information changes materially.

## Related Standards and Work

- `OTMN Privacy & Transparency Standard v1.0` — organization-wide information handling and privacy baseline
- Issue #19 — OTMN GitHub Organization Access Model
- Issue #9 — Audit OTMN public vs private GitHub information boundaries

## Review

This standard should be reviewed when OTMN's repository structure, contributor model, or information-handling requirements materially change.

**Status:** Approved — OTMN Standard v1.0
