## Summary

Describe the change and the problem it solves.

## Scope

- [ ] Focused change with no unrelated refactor
- [ ] Public/private data boundaries reviewed
- [ ] Existing modules/interfaces reused where practical

## Validation

List the exact tests, commands, checks, or manual validation performed.

```text
# Example
pytest tests/path/to/test_file.py -q
```

## Evidence

Attach or link relevant logs, screenshots, benchmark output, traces, or other artifacts when applicable.

## Risk and impact

Describe any impact on:

- security or credentials;
- customer or nonpublic data;
- APIs or compatibility;
- deployment or CI/CD;
- models, datasets, licensing, or provenance;
- operator behavior or safety.

## Follow-up

List known limitations, deferred work, or migration steps.

## Checklist

- [ ] I reviewed the diff for accidental secrets or confidential information.
- [ ] Tests cover the changed behavior where practical.
- [ ] Documentation is updated if behavior or interfaces changed.
- [ ] AI-generated or externally sourced material was reviewed for correctness, security, licensing, and provenance.
