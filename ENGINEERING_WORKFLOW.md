# SALT19 Engineering Workflow

This document defines the default engineering workflow for SALT19 repositories unless a repository provides stricter project-specific instructions.

## Source of truth

GitHub is the durable engineering system of record for source code, issues, pull requests, tests, release artifacts, and material technical decisions. Chat and email are coordination layers; decisions that affect implementation, interfaces, risk, or release state should be reflected in GitHub.

## Branches

- `main` is the default integration branch unless a repository states otherwise.
- Use short-lived topic branches for functional work.
- Prefer branch names such as `fix/...`, `feat/...`, `docs/...`, `test/...`, or `chore/...`.
- Avoid direct pushes to protected branches when branch protection is enabled.

## Changes

Before adding new modules, search for an existing implementation, adapter, interface, or utility that can be reused or repaired. Prefer thin integrations over duplicate subsystems.

Changes should preserve local behavior and compatibility unless a deliberate contract change is documented and reviewed.

## Pull requests

Pull requests should be small enough to review, contain a clear validation plan, and identify known risks. Functional changes should include tests or a written explanation of why automated coverage is not practical.

At least one independent review is preferred for material code changes. High-risk changes involving security, credentials, authority, safety, customer data, deployment, or destructive operations should receive additional scrutiny before merge.

## CI and evidence

A green CI result is necessary evidence, not proof of correctness. Reviewers should consider the test surface, failure modes, runtime assumptions, and whether the evidence actually supports the claim being made.

Do not weaken tests, gates, or acceptance criteria merely to obtain a passing build without documenting the reason and resulting risk.

## Secrets and customer data

Never commit credentials, private keys, tokens, customer data, confidential documents, or security-sensitive operational details. Use approved secret-management and customer-specific systems instead.

## AI-assisted engineering

AI tools may assist development, review, testing, and documentation, but generated output must be treated as untrusted until reviewed. The submitting engineer remains responsible for correctness, security, licensing, provenance, and adherence to customer restrictions.

## Releases

Release notes should distinguish demonstrated behavior from planned work. Material known limitations should not be hidden. When a release changes interfaces, configuration, deployment, or operator behavior, update the relevant documentation in the same change or explicitly track the documentation debt.
