# UI/UX Pro Max — Claude Super Skills

Reusable skill guides for designing, building, reviewing, and securing better software with AI-assisted workflows.

![Claude Code](https://img.shields.io/badge/Claude%20Code-Skills-D97757?style=for-the-badge&logo=anthropic&logoColor=white) ![Open Source](https://img.shields.io/badge/Open%20Source-Community-181717?style=for-the-badge&logo=github)

## Overview

This repository brings together focused `SKILL.md` guides for Claude Code and compatible agent-skill workflows.

Each skill describes when it is useful and provides a practical process, checks, and recommendations for a specific task.

Use the catalog to choose individual skills rather than loading every guide into every project.

## What’s inside

- **UI/UX design:** layout, responsive interfaces, navigation, typography, motion, and design systems.
- **Product experience:** onboarding, forms, empty states, error recovery, checkout, and settings.
- **Quality and accessibility:** usability testing, design QA, accessibility review, and visual regression.
- **Engineering workflows:** project setup, API contracts, automated testing, React performance, and database migrations.
- **Security and AI:** secure code review, incident-response triage, MCP server development, and LLM feature evaluation.

## Skill catalog

Browse [`skills/README.md`](skills/README.md) for the complete list of available skills.

Each skill lives in its own directory and is defined by a `SKILL.md` file.

## Repository structure

```text
ui-ux-pro-max/
├── README.md
├── docs/                         # Supporting documentation
├── examples/                     # Examples and demonstrations
├── skills/
│   ├── README.md                 # Complete skill catalog
│   ├── accessibility-review/
│   ├── design-system/
│   ├── frontend-design/
│   ├── secure-code-review/
│   ├── ...                        # Additional focused skill directories
│   └── <skill-name>/SKILL.md
├── claude-seo-main/              # Bundled source snapshot
├── claude-seo-main.zip
├── ui-ux-pro-max-skill-main/     # Bundled source snapshot
└── ui-ux-pro-max-skill-main.zip
```

The tree is a high-level guide; `skills/README.md` is the source of truth for the skill catalog.

## Installation

Clone the repository:

```bash
git clone https://github.com/Atharva-ark06/ui-ux-pro-max.git
cd ui-ux-pro-max
```

To use an individual skill, copy its directory into your Claude skills directory:

```bash
cp -r skills/<skill-name> ~/.claude/skills/
```

Replace `<skill-name>` with the directory you want to use. Check your installed Claude Code version and environment for any setup-specific requirements.

## Usage

1. Choose a skill from [`skills/README.md`](skills/README.md).
2. Read its `SKILL.md` to understand its scope and workflow.
3. Copy or install the skill in the appropriate skills directory for your environment.
4. Ask Claude to perform a task that matches the skill’s description.
5. Review the output and validate changes before using them in a real project.

Skills provide guidance; they do not replace code review, testing, or human judgment.

## Creating a skill

1. Create a directory under `skills/` using a short, descriptive name.
2. Add a `SKILL.md` file with YAML frontmatter containing `name` and `description`.
3. Explain the skill’s purpose, when it should be used, and its recommended workflow.
4. Include concrete checks and examples where they improve reliability.
5. Add the skill to [`skills/README.md`](skills/README.md).

Minimal example:

```markdown
---
name: my-skill
description: Explain what this skill does and when to use it.
---

# My Skill

## Workflow
