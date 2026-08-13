# OTMN Repository Visibility Model v1.0

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

## Related Work

This standard complements the OTMN public-versus-private information work and should be used as the baseline visibility rule before introducing more detailed information-classification procedures.

## Status

Proposed for adoption as an OTMN Standard v1.0.
