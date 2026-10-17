# Agent-Assisted Pull Request Workflow

## Author checklist

1. Define the issue and acceptance criteria.
2. Create a focused branch.
3. Make a coherent change.
4. Run relevant checks.
5. Ask an agent to inspect correctness, security, regressions, and test gaps.
6. Verify findings and fix confirmed issues.
7. Open a PR with a summary, evidence, and known limitations.

## Review expectations

- Read the full diff and relevant surrounding code.
- Prioritize correctness, security, data loss, and regressions.
- Cite file paths and lines for findings.
- Explain impact and a reproducible scenario.
- Separate blocking findings from optional suggestions.
- Do not invent findings when evidence is missing.

## Merge gate

- [ ] CI checks pass.
- [ ] Required review is complete.
- [ ] No unresolved high-impact finding remains.
- [ ] Tests and documentation match behavior.
- [ ] No secrets or unrelated generated files were committed.

After merge, check the target branch and CI result. Record follow-up work as issues.
