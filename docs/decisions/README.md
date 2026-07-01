# Architecture Decision Records (ADRs)

This folder records the project's **relevant decisions** as _Architecture Decision
Records_ (ADRs): short documents that capture a decision, its context, and its
consequences.

## What is an ADR and when to create one?

Create an ADR when you make a decision that is **hard or costly to reverse**, affects
several parts of the project, or that your future self (or a new contributor) will be
grateful to have documented. Examples: changing the template format, adopting a
different commit convention, defining the project's scope.

You do not need an ADR for trivial or easily reversible decisions.

## Numbering and naming convention

- Files: `NNNN-title-in-kebab-case.md` (sequential numbering starting at `0001`).
- The base template is [`0000-template.md`](0000-template.md) — copy it to create a new one.

## State cycle

```
Proposed → Accepted → (eventually) Superseded by ADR-XXXX | Deprecated
```

- **Proposed**: under discussion.
- **Accepted**: current decision.
- **Superseded**: a later decision replaces it (link to the new ADR).
- **Deprecated**: no longer applies.

ADRs are **immutable** once accepted: instead of editing them, create a new one that
supersedes the previous one.

## Index

| ADR                                           | Title                        | Status   |
| --------------------------------------------- | ---------------------------- | -------- |
| [0001](0001-record-architecture-decisions.md) | Record the project decisions | Accepted |
