# Repository Onboarding Workflow for Agents

Before making changes in an unfamiliar repository, build a small, accurate map of the project.

## Inspect
- README and contribution guidelines
- Package/build configuration and lockfiles
- Source and test directory structure
- Formatting, lint, type-check, and test scripts
- Environment variable names without revealing their values
- CI workflows and branch conventions
- Existing architecture and component patterns

## Report
Summarize the framework, key entry points, test commands, coding conventions, and risks. Mark anything not verified.

## Before editing
Choose the smallest relevant set of files, identify acceptance criteria, and establish how the change will be tested. Do not run deployment commands or inspect secret values merely because they exist in the repository.