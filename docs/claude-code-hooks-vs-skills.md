# Claude Code Hooks vs Skills

Skills and hooks solve different problems and should not be treated as interchangeable.

## Skills

Skills package reusable task instructions. They are useful when an agent needs a repeatable process such as reviewing a pull request, implementing a UI from a design, or checking accessibility.

Use a skill when the workflow requires judgment, context, or a sequence of steps.

## Hooks

Hooks are configured lifecycle actions that run in response to supported events. They are useful for deterministic automation such as formatting after edits or enforcing a local policy check.

Use a hook when the desired behavior is an explicit event-triggered action that can be reliably automated.

## Decision guide

| Need | Better starting point |
| --- | --- |
| Explain how to conduct a security review | Skill |
| Run a formatter after a supported file-change event | Hook |
| Provide a reusable Figma-to-code procedure | Skill |
| Block a command according to a deterministic policy | Hook or an appropriate external policy control |
| Check a change and explain trade-offs | Skill, with tests or hooks where useful |

## Combined workflow

A skill can instruct the agent to run tests and inspect their output; a hook can automate a narrow check at an appropriate event. Keep automation transparent, scoped, and easy to disable during troubleshooting.

## Safety

Review hook commands carefully because they may run automatically. Avoid secrets in hook configuration, and test in a disposable repository before enabling commands with side effects.

## Official reference

https://docs.anthropic.com/en/docs/claude-code/hooks
https://docs.anthropic.com/en/docs/claude-code/skills
