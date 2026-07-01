# Security Policy

This is a **documentation** repository: it contains the `.gitmessage` template and its
usage guide. It does not run code or deploy services, so its security surface is
minimal. Even so, we appreciate responsible reports.

## Reporting a Vulnerability

If you find a security issue (for example, a malicious link, inappropriate content, or
accidental exposure of sensitive data in the repository), **do not open a public issue**.
Report it privately:

- **Email**: <brayandiazc@gmail.com> (subject starting with `Security:`).
- **GitHub Security Advisories**: repository _Security_ tab → _Report a vulnerability_.

Include a clear description of the problem and, if applicable, the affected file or commit.
We commit to acknowledging receipt within a reasonable time and keeping you informed.

## Scope

**In scope:**

- Repository content (documentation, the `.gitmessage` template, repo config files).
- The repository's GitHub configuration.

**Out of scope:**

- Automated scanner reports without demonstrated impact.
- Vulnerabilities in third-party tools (Git, GitHub) not attributable to this repository.
- Social engineering, phishing, or DoS.

## Handling Secrets

- **Never** commit secrets (keys, tokens, passwords, `.env` files with real values).
- If a secret is committed by mistake: **rotate it first**, then clean up history —
  rewriting history is not enough; assume it is already compromised.

## Contact

- **Security reports**: <brayandiazc@gmail.com> (subject: `Security: …`)
- **General inquiries**: <brayandiazc@gmail.com>

---

> Version: 1.0 — Last updated: 2026-07-01
