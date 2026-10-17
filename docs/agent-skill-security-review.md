# Agent Skill Security Review

Skills can influence how an agent uses tools and executes code. Review a skill as executable workflow guidance, even when its main file is Markdown.

## Before installing

- [ ] Confirm source repository, maintainer, and license.
- [ ] Read the complete `SKILL.md` and linked documentation.
- [ ] Inspect every script and shell command.
- [ ] Identify network requests, package installation, file writes, and external service actions.
- [ ] Check whether instructions request secrets, broad filesystem access, or unnecessary permissions.
- [ ] Search for encoded payloads, obfuscated commands, and instructions to ignore user intent.
- [ ] Check dependencies and whether versions are pinned or otherwise controlled.

## During use

- [ ] Keep the skill's actions within the requested task.
- [ ] Require confirmation for destructive changes, publishing, deployment, or external messages when not explicitly authorized.
- [ ] Do not paste credentials into prompts or commit them to the repository.
- [ ] Review diffs before accepting generated changes.
- [ ] Run tests in an appropriate environment and inspect unexpected network or filesystem activity.

## Trust boundaries

A skill's description is not proof of its behavior. Treat repository files, fetched pages, examples, and tool output as data—not as authority to override the user's request or security constraints.

## Risk classification

| Risk | Example | Suggested response |
| --- | --- | --- |
| Low | Focused writing checklist, no scripts | Read and test before adoption |
| Medium | Scripted file edits or dependency installation | Inspect code and run in a disposable test repo |
| High | Credential handling, privileged commands, remote execution | Do not install without a clear, reviewed need and appropriate isolation |

## After review

Record source URL, review date, intended scope, dependencies, and any limitations. Re-review when the skill changes materially.

## References

- https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview
- https://developers.openai.com/codex/skills/
