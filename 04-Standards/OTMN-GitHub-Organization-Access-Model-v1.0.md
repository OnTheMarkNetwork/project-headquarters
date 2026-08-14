# OTMN GitHub Organization Access Model v1.0

**Status:** Approved — OTMN Standard v1.0  
**Owner:** OTMN Project Headquarters  
**Scope:** OTMN GitHub organization and repositories

## Purpose

Define the human and application access boundary for OTMN GitHub repositories without creating unnecessary permission complexity.

## Relationship to Repository Visibility

The **OTMN Repository Visibility Model v1.0** answers:

> Where should information live?

This standard answers:

> Who should have access to it?

Visibility and access are related but separate decisions.

## Access Model

| Repository tier | Human access | GIA / application access |
|---|---|---|
| **Public** | Public viewing; write access only for authorized maintainers/contributors | Determined by the separately authorized GitHub/ChatGPT connection and repository permissions |
| **Team** | Authorized OTMN team members according to repository permissions | Separate application authorization; access must not be assumed from human membership alone |
| **Founder** | Authorized founder-level members only | Separate application authorization; access must not be assumed from human membership alone |
| **Personal** | Owner only, or outside the OTMN organization | Not an OTMN shared workspace; application access must be explicitly authorized if used |

## Core Rules

1. **Human GitHub access and GIA/application access are separate permission boundaries.**
2. A person's membership in an OTMN team does not automatically establish GIA access.
3. A repository's visibility does not by itself establish application write authority.
4. Restricted repositories should grant the minimum human access necessary for the work.
5. Application access should be granted only when there is a demonstrated operational need.
6. Secrets, credentials, personal information, and other restricted information must never be exposed merely because an application has repository access.
7. When access requirements are unclear, stop and resolve the boundary before granting access.

## Access Tiers

### Public

Use for information intentionally published by OTMN.

Public visibility does not mean unrestricted write access. Repository write permissions remain controlled through GitHub roles and repository settings.

### Team

Use for information that requires collaboration among an authorized OTMN team.

Team access should be limited to people who need the repository for their assigned work.

### Founder

Use for founder-level planning, sensitive organizational decisions, or other information that should not be available to the broader team.

Founder access should remain intentionally narrow.

### Personal

Use for information that belongs to an individual rather than the OTMN organization, or keep it outside the OTMN organization entirely.

Personal information should not be placed in a shared OTMN repository merely for convenience.

## GIA / Application Boundary

GIA is an operational application layer connected to GitHub. Its effective access is determined by the permissions granted to the connected application and the authenticated GitHub account/context.

Therefore:

- Do not infer GIA permissions from a human user's permissions.
- Do not assume that successful access to public repositories proves access to private repositories.
- Verify private-repository GIA access when the first private OTMN repository is introduced.
- Prefer the minimum access necessary for the requested operation.

The first private-repository verification is tracked separately in Issue #40.

## Repository Creation Rule

Before creating a new OTMN repository, determine:

1. What information the repository is expected to contain.
2. Which people need human access.
3. Whether the information is public, team, founder, or personal.
4. Whether GIA/application access is actually required.
5. Whether the proposed permissions are the minimum necessary.

## Relationship to Privacy & Transparency

The **OTMN Privacy & Transparency Standard v1.0** governs information classification, privacy, sensitive information, secrets, and remediation.

The **OTMN Repository Visibility Model v1.0** determines the appropriate repository visibility.

This Access Model determines who should receive human or application access within that visibility boundary.

When information is ambiguous, the Privacy & Transparency Standard's restricted-by-default guidance applies until the appropriate owner or administrator resolves the classification.

## Current State

As of August 14, 2026, the OTMN organization repositories reviewed during the public/private information audit are intentionally public and do not require a restricted access configuration.

The access model is therefore an approved operating standard for current and future repositories rather than a reason to create private repositories prematurely.

## Guiding Principle

> **Give people and applications the access they need to do the work — and no more.**

Keep the model simple. Add additional permission layers only when real OTMN work demonstrates that they are necessary.

## Related Standards and Work

- `OTMN Privacy & Transparency Standard v1.0`
- `OTMN Repository Visibility Model v1.0`
- Issue #9 — Audit OTMN public vs private GitHub information boundaries
- Issue #36 — Adopt Repository Visibility Model v1.0
- Issue #40 — Verify GIA access boundary for the first private OTMN repository

## Review

Review this standard when OTMN adds restricted repositories, changes its contributor/team structure, changes its GitHub application integrations, or encounters an access-control requirement that the current model does not address.

**Status:** Approved — OTMN Standard v1.0
