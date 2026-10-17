# Claude Code Subagent Task Decomposition

Use parallel or delegated work only when subtasks are sufficiently independent and the client supports the required agent features.

## Good candidates

- Audit separate modules with clear boundaries.
- Research independent options and compare findings.
- Review tests and documentation separately from implementation.
- Inspect independent UI pages against the same design system.

## Poor candidates

- Multiple agents editing the same files without coordination.
- Tasks whose results depend on unresolved product decisions.
- Delegation that exposes broader permissions than the parent task needs.
- Parallel work that costs more to integrate than it saves.

## Coordination pattern

1. Define the shared goal and acceptance criteria.
2. Split work by file ownership or clearly independent questions.
3. Give each subtask its own scope and expected output.
4. Ask each worker to report evidence, assumptions, and changed files.
5. Integrate changes centrally and resolve conflicts.
6. Run the complete verification suite after integration.

Delegation does not remove the need for a final diff review or end-to-end tests.

Reference: https://docs.anthropic.com/en/docs/claude-code/sub-agents
