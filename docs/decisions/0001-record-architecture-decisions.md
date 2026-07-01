# 0001. Record the project decisions

- **Status**: Accepted
- **Date**: 2026-07-01
- **Deciders**: Brayan Diaz C

## Context and problem

As the project evolves, decisions are made whose context and motivation get lost over
time. Without a record, already-settled debates are repeated and new contributors do not
understand why things are the way they are.

## Considered options

- **Don't document** — rely on memory and commit history.
- **Document in a wiki** — easy to edit but decoupled from the repository.
- **Architecture Decision Records (ADRs)** — files versioned alongside the content.

## Decision

We adopt lightweight **Architecture Decision Records (ADRs)** (MADR style), versioned in
`docs/decisions/`. Each relevant decision is documented using the
[`0000-template.md`](0000-template.md) template and numbered sequentially.

## Consequences

**Positive:**

- The "why" of each decision is recorded next to the content.
- New contributors get up to speed faster.
- Already-made decisions are not re-litigated.

**Negative / costs:**

- Requires discipline to create the ADR at decision time.

**Neutral / to watch:**

- Keeping the [README](README.md) index up to date.

## References

- [Documenting Architecture Decisions — Michael Nygard](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions)
- [MADR — Markdown Architectural Decision Records](https://adr.github.io/madr/)
