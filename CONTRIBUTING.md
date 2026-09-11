# Contributing to SALT19 Projects

Thank you for contributing to SALT19.

This document provides default contribution guidance for SALT19 repositories. A repository-specific `CONTRIBUTING.md` takes precedence when present.

## Before you start

1. Read the repository README, license, security policy, and any project-specific instructions.
2. Use an issue or project discussion when the scope is unclear or the proposed change is substantial.
3. Never place customer information, credentials, private source code, export-controlled material, or other nonpublic SALT19 information in a public repository, issue, pull request, or third-party service.

## Development workflow

- Create focused branches from the repository's current default branch.
- Keep changes scoped to one coherent problem where practical.
- Reuse existing modules and interfaces before introducing new abstractions.
- Preserve backward compatibility unless the change intentionally modifies a documented contract.
- Add or update tests for behavioral changes.
- Update documentation when interfaces, configuration, deployment, or operator behavior changes.

## Pull requests

A pull request should state:

- what changed;
- why the change is needed;
- how it was tested;
- known limitations or follow-up work;
- any security, licensing, data, model, or deployment implications.

Avoid unrelated formatting sweeps or broad refactors in the same pull request as a functional change unless they are required for the change.

## AI-assisted development

AI-assisted code remains subject to the same engineering standard as human-authored code. Contributors are responsible for reviewing generated or externally sourced material for correctness, security, licensing, provenance, and repository-specific restrictions before submission.

Do not submit SALT19 or customer confidential information, credentials, private source code, or nonpublic data to unauthorized public AI, model-training, or cloud services.

## Testing and evidence

Claims in issues and pull requests should be supported by reproducible tests, logs, benchmarks, screenshots, or other appropriate evidence when practical. Distinguish measured behavior from assumptions, targets, or future work.

## Security

Do not disclose suspected vulnerabilities publicly. Follow [`SECURITY.md`](SECURITY.md).

## Conduct

Be technically rigorous and professional. Review the work rather than the person, document disagreements with evidence, and keep project channels focused on delivery and engineering quality.
