# Contributing to jolarca-payments

> **This repository is within the cardholder-data environment (CDE) boundary.**
> All changes are subject to PCI-DSS change-control requirements (Req. 6.3).

## Before you contribute

This repository holds payment processing policy, PCI-DSS compliance artifacts,
and CDE governance for the `jolarca-dev` marketplace. It is **not** application
code — it is the authoritative record of how cardholder data is protected.

Every change to this repository is a change to the CDE and requires:

1. A documented change request (link in the PR body)
2. PCI-DSS impact assessment (what req. does this affect?)
3. Full compliance gate passage (dependency scan, secret scan, license check,
   code quality, security review)

## How to propose changes

1. Fork or branch from `main`
2. Make your changes in a feature branch named `type/short-description`
   (e.g., `docs/update-scope-definition`, `fix/key-rotation-steps`)
3. Ensure all CI checks pass (`ci` and `security` contexts must be green)
4. Open a pull request against `main`
5. Fill in the PR template — include the PCI-DSS requirement(s) affected

## What we review for

- **Accuracy**: Does the policy/procedure match the actual control?
- **Completeness**: Are all PCI-DSS requirements addressed?
- **No secrets**: Never commit keys, tokens, credentials, or cardholder data
- **No PAN**: Primary Account Numbers are NEVER stored here (PCI-DSS Req. 3)
- **Linear history**: Squash-only merge; one logical change per PR

## Security vulnerabilities

If you find a vulnerability, **do not open a public issue**. Follow the
procedure in [SECURITY.md](SECURITY.md).

## Code style

- Markdown: one sentence per line, no trailing whitespace
- YAML: validated against the schema (CI runs `check-yaml`)
- Python: ruff + mypy --strict (see `pyproject.toml`)
- Pre-commit hooks are configured — install with `pre-commit install`

## Questions

Contact the repository owner (@JourneyOfLife) via the `jolarca-dev`
organization. All access follows PCI-DSS Req. 7 need-to-know principles.
