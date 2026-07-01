# Contributing Guide

Thank you for your interest in contributing to **Git Commit Message Template**! This is
a documentation repository (the `.gitmessage` template and its usage guide), so
contributions are mainly improvements to wording, examples, and structure.

## Table of Contents

- [Getting Started](#getting-started)
- [Workflow](#workflow)
- [Documentation Standards](#documentation-standards)
- [Commits and Messages](#commits-and-messages)
- [Pull Requests](#pull-requests)

## Getting Started

1. **Fork** the repository.
2. Clone it to your machine:

   ```bash
   git clone https://github.com/your-username/gitmessage-template-en.git
   cd gitmessage-template-en
   ```

3. Create a branch for your change (see below).

There are no dependencies to install and no build to run: a text editor is enough.

## Workflow

We use a simple flow based on short branches off `main`.

### Branching strategy

| Branch    | Purpose                                     | From   | Into   |
| --------- | ------------------------------------------- | ------ | ------ |
| `main`    | Published content. Always stable.           | —      | —      |
| `feat/*`  | New feature or section.                     | `main` | `main` |
| `fix/*`   | Fix for an error or inconsistency.          | `main` | `main` |
| `docs/*`  | Documentation-only changes.                 | `main` | `main` |
| `chore/*` | Maintenance, tooling, configuration tasks.  | `main` | `main` |

### Branch naming

- Lowercase, with a type prefix and a `kebab-case` description:
  `feat/spanish-example`, `fix/readme-typo`, `docs/clarify-footer`.

### Typical flow

```bash
git checkout main
git pull origin main
git checkout -b docs/my-improvement
# ... edit ...
git add .
git commit   # use this repo's template (see below)
git push origin docs/my-improvement
# open a Pull Request into main
```

## Documentation Standards

- UTF-8 encoding, LF line endings (see [`.editorconfig`](.editorconfig)).
- Clear Markdown, consistent with the existing style.
- Keep the example bodies within the conventions this project documents
  (title ≤ 50, body ≤ 72 characters).

## Commits and Messages

This repository **provides and uses** its own commit template. Configure and use it
when contributing:

```bash
git config commit.template .gitmessage
```

We follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/):

```
<type>: <short description in imperative mood>
```

Common types: `feat`, `fix`, `docs`, `style`, `refactor`, `chore`.

Examples:

```
docs: clarify footer usage in the README
fix: correct the title character limit
feat: add a commit example with a co-author
```

## Pull Requests

- Use the [PR template](.github/PULL_REQUEST_TEMPLATE.md) (loaded automatically).
- One PR per logical change; keep them small and focused.
- Link related issues (`Closes #123`).
- Describe **what** you change and **why**.

We appreciate your help! 🙌
