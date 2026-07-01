# Roadmap — Git Commit Message Template

> Project status and direction. Living document.
> **Last updated**: 2026-07-01

## Legend

- ✅ Done
- 🚧 In progress
- 📋 Planned
- ⏸️ Deferred

## Vision

Provide a clear Git commit message template in English, based on
[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), easy to adopt in
any project.

## Current status

- ✅ `.gitmessage` template in English.
- ✅ Full usage guide in the `README.md`.
- ✅ Community files (contributing, conduct, security, changelog).

## Ideas / next steps

- 📋 One-command install script (`git config commit.template`).
- 📋 Additional commit examples (breaking changes, reverts, co-authorship).
- 📋 Optional integration with a `commit-msg` hook to validate the format.

## Out of scope

- Heavy validation tooling or dependencies on a specific language: the project stays as
  documentation + a template file.

## How this document is updated

- Review it when closing each version/phase.
- Decisions that change direction are recorded as ADRs in [`../decisions/`](../decisions/README.md).
