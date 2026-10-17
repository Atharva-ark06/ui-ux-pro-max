# Cross-Client Skill Installation Checklist

Use this checklist before adding a skill to Claude Code, Codex, or another compatible agent.

## Preparation

- [ ] Identify the agent/client and version.
- [ ] Confirm the skill format and supported installation path.
- [ ] Read source instructions and license.
- [ ] Inspect scripts, dependencies, and network access.
- [ ] Decide whether the skill belongs to one user or the project.
- [ ] Check that the skill does not duplicate an existing workflow.

## Installation

- [ ] Use an official installer or copy the complete reviewed directory.
- [ ] Preserve relative references and required resources.
- [ ] Avoid copying secrets, local settings, or unrelated files.
- [ ] Record the source URL and review date.
- [ ] Restart or open a fresh session if required by the client.

## Verification

- [ ] Confirm the skill is discoverable.
- [ ] Ask the agent when it should use the skill.
- [ ] Run a small, safe test.
- [ ] Review generated edits and any tool actions.
- [ ] Confirm expected validation steps were followed.

## Maintenance

- [ ] Review updates before replacing a known-good version.
- [ ] Re-test after significant changes to the agent or tool.
- [ ] Remove unused or untrusted skills.
- [ ] Keep project-level skills documented and version-controlled.

## Remember

A skill file gives instructions; it does not automatically provide integrations, credentials, or tools. MCP connections, account access, and product permissions are configured separately.
