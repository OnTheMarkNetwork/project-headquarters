# OTMN Privacy & Transparency Standard v1.0

**Status:** Proposed — pending review and approval
**Owner:** OTMN Project Headquarters
**Scope:** OTMN GitHub organization, repositories, documentation, issues, pull requests, and related operational artifacts

## Purpose

OTMN uses transparency to make appropriate organizational work understandable and accessible, while protecting information that should not be public.

This standard defines how OTMN classifies information, chooses appropriate visibility, protects sensitive information, and responds when information is exposed incorrectly.

## 1. Information Classification

### Public

Information may be public when it is intentionally suitable for public visibility and does not contain confidential, sensitive, personal, or security-sensitive material.

Examples include:

- Public organization and project information
- Approved public documentation and standards
- Public roadmaps and project descriptions intended for publication
- Public source code and configuration that is safe to disclose
- Public issues, discussions, and pull requests where the repository is intentionally public

Public does not mean that every piece of information about OTMN belongs in a public repository. Public visibility must be intentional.

### Internal

Internal information is operational material intended for OTMN participants but not necessarily for public distribution.

Examples include:

- Internal planning and working notes
- Unpublished operational decisions
- Contributor or administrative information not intended for public release
- Internal evaluations, drafts, or discussions
- Business information whose publication has not been approved

Internal information should be kept in an appropriately restricted repository or system when the repository itself is public.

### Private / Sensitive

Private or sensitive information requires restricted access and should not be placed in a public repository or public issue, pull request, discussion, or document.

Examples include:

- Credentials, API keys, tokens, passwords, private keys, and secrets
- Personal information that is not intentionally public
- Security-sensitive information
- Confidential business or contractual information
- Unpublished information where disclosure could create material risk
- Information supplied under an expectation of confidentiality

When in doubt between public and restricted handling, treat the information as restricted until its classification is resolved.

## 2. Repository Visibility

Repository visibility should follow the information it is intended to contain.

- **Public repository:** Use for work intentionally intended for public visibility.
- **Private repository:** Use when the repository contains internal, private, sensitive, or otherwise restricted material.
- A public repository must not be used as a substitute for private operational storage.

Repository visibility is a governance decision, not merely a technical setting. Repository owners and administrators are responsible for reviewing whether the repository's visibility remains appropriate as its contents and purpose change.

## 3. Secrets and Credentials

Secrets and credentials must never be intentionally committed to a public repository.

This includes passwords, API keys, access tokens, private keys, authentication material, and similar credentials.

Use appropriate secret-management mechanisms instead of storing credentials in source files, documentation, issues, pull requests, or commits.

If a secret is accidentally committed, assume it may be compromised. Remove the exposed material from the repository where practical, rotate or revoke the affected credential, assess the exposure, and document the remediation as appropriate.

Removing a secret from the latest file alone does not necessarily remove it from Git history or other copies. Remediation should account for the actual exposure path.

## 4. Personal and Sensitive Information

OTMN should minimize collection and publication of personal information.

Personal information should not be placed in public repositories, issues, pull requests, or other public artifacts unless there is a clear reason for publication and the information is intentionally public.

Sensitive information should be handled through an appropriately restricted system and shared only with people who have a legitimate need to access it.

## 5. Unpublished Business and Project Information

Unpublished business plans, commercial information, private partnerships, unreleased product information, confidential contributor material, and similar information should remain restricted until authorized for public release.

Draft status alone does not automatically make information private; however, information should not be assumed public merely because it appears in a working repository or document.

## 6. Classification Authority

The repository owner or designated project owner is responsible for the initial classification of information within the repository or project they control.

Organization-level visibility or policy decisions may be escalated to the OTMN organization administrator when they affect multiple repositories, organization-wide standards, contributor access, or significant privacy/security concerns.

When classification is ambiguous, the safer restricted classification should be used until the appropriate owner or administrator resolves the question.

## 7. Accidental Exposure and Remediation

If restricted information is accidentally published:

1. **Stop further exposure** where practical.
2. **Identify what was exposed**, where it appeared, and who may have had access.
3. **Rotate, revoke, or replace credentials** immediately when credentials or secrets are involved.
4. **Remove or restrict the exposed material** using the appropriate GitHub or system controls.
5. **Consider repository and Git history**, not only the current file contents.
6. **Assess whether additional notification or remediation is required.**
7. **Document the incident and corrective action** when the exposure is material or operationally significant.
8. **Review the workflow that allowed the exposure** and improve it when a systemic issue is identified.

The goal is containment and remediation, not simply deleting the visible copy of the information.

## 8. Transparency Principle

OTMN should prefer transparency for information that is intentionally public and appropriate to share, while respecting privacy, security, confidentiality, and legitimate operational boundaries.

The objective is not maximum disclosure. The objective is **appropriate transparency**.

## 9. Review

This standard is a working v1.0 standard and should be reviewed as OTMN's repository structure, contributor model, and operational requirements evolve.

Changes that materially affect organization-wide information handling should be reviewed and approved before being treated as the current standard.
