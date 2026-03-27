# Contributing to Ph4wkm00n's Projects

> All research and tooling in this org is for **educational and authorized use only**.
> By contributing you agree to operate within legal and ethical boundaries.

---

## Before You Open Anything

1. **Check existing issues and PRs** — avoid duplicates.
2. **Open an issue first** for non-trivial changes — alignment before effort.
3. **No unsolicited features** — scope creep kills focused tools.

---

## Setup

```bash
# 1. Fork and clone
git clone git@github.com:YOUR_HANDLE/REPO_NAME.git
cd REPO_NAME

# 2. Create a feature branch (never work on main)
git checkout -b feat/short-description

# 3. Install deps (varies per project — check the repo's README)
```

---

## Commit Style

Use [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short imperative summary>

[optional body — explain WHY, not what]
[optional footer — e.g. Fixes #42]
```

| Type | When |
|------|------|
| `feat` | New capability |
| `fix` | Bug fix |
| `docs` | Docs only |
| `refactor` | Code restructure, no behaviour change |
| `test` | Add or fix tests |
| `chore` | Tooling, CI, deps |
| `vuln` | Security finding or patch |

**Examples:**
```
feat(scanner): add UDP sweep mode
fix(payload): handle null byte in shellcode encoder
vuln(parser): patch heap overflow in PCAP reader  (Fixes #7)
```

---

## Code Standards

- **Python**: `black` + `ruff`. Line length 100. Type hints on all public functions.
- **Bash**: `shellcheck` clean. `set -euo pipefail` at the top.
- **Go / Rust**: `gofmt` / `rustfmt` — CI will reject unformatted code.
- **No secrets in code** — use env vars or `.env` (listed in `.gitignore_global`).
- **No hardcoded IPs, domains, or credentials** — parameterise everything.

---

## Pull Requests

- Keep PRs **small and focused** — one concern per PR.
- Fill out the PR template (auto-populated from `.github/PULL_REQUEST_TEMPLATE.md`).
- All CI checks must pass before review.
- At least one approving review required to merge.

---

## Security Issues

**Do NOT open a public issue for vulnerabilities.**

Report privately:
- **Email**: `ph4wkm00n [at] proton [dot] me` — PGP preferred
- **Keybase**: `keybase.io/ph4wkm00n`

I'll acknowledge within 48 h and aim to patch within 14 days.
Please allow time for a fix before public disclosure.

---

## Ethical Boundaries

All tools here are dual-use by nature. By contributing you agree:

- You will not use, adapt, or redistribute this code for unauthorized access.
- You will not weaponize research against civilian infrastructure.
- You accept that misuse is entirely your legal and moral responsibility.

---

*Thanks for keeping this community sharp and clean. 🦅*
