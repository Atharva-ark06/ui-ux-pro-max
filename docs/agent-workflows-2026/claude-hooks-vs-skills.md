# Claude Code Hooks vs Skills

Skills explain repeatable work; hooks automate supported lifecycle events. Use each for the job it fits.

| Need | Start with |
| --- | --- |
| Repeatable accessibility audit | Skill |
| Instructions for reviewing a pull request | Skill |
| Deterministic formatting action on a supported event | Hook |
| Explain findings and recommend fixes | Skill plus verification tools |

## Combined workflow

A skill can instruct an agent to run tests and interpret the results. A hook can automate a narrow, predictable check. Keep each automation scoped and documented.

## Safety

Review hook commands before enabling them because they may run automatically. Test in a disposable repository, avoid secrets in configuration, and do not add destructive actions without clear need.

Official references:
- https://docs.anthropic.com/en/docs/claude-code/hooks
- https://docs.anthropic.com/en/docs/claude-code/skills
