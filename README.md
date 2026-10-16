# 🧠 Claude Super Skills

<p align="center">

<img src="https://img.shields.io/badge/Claude%20Code-Super%20Skills-D97757?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Code">

<img src="https://img.shields.io/badge/AI-Agent%20Skills-7C3AED?style=for-the-badge&logo=probot&logoColor=white" alt="Agent Skills">

<img src="https://img.shields.io/badge/Automation-00A67E?style=for-the-badge&logo=robotframework&logoColor=white" alt="Automation">

<img src="https://img.shields.io/badge/Open%20Source-000000?style=for-the-badge&logo=github&logoColor=white" alt="Open Source">

</p>

<p align="center">
  <strong>⚡ Upgrade Claude from a general-purpose AI into a specialized development powerhouse.</strong>
</p>

<p align="center">
  Reusable skills • Structured workflows • Better reasoning • Consistent output
</p>

<p align="center">
  <a href="#-overview">Overview</a> •
  <a href="#-features">Features</a> •
  <a href="#-skills">Skills</a> •
  <a href="#-installation">Installation</a> •
  <a href="#-usage">Usage</a> •
  <a href="#-creating-a-skill">Create Skills</a>
</p>

---

## 🚀 Overview

**Claude Super Skills** is a collection of reusable, modular skills designed to extend the capabilities of **Claude Code**.

Instead of repeatedly explaining how you want Claude to approach a task, skills provide structured instructions, workflows, conventions, and reusable knowledge that Claude can apply automatically when the situation matches.

> **One skill = one specialized capability.**

The goal is simple:

```text
Generic Claude
      │
      ▼
┌──────────────────────┐
│   Claude Super Skills │
├──────────────────────┤
│ Development           │
│ Debugging             │
│ Research              │
│ Writing               │
│ Automation            │
│ Architecture          │
│ Productivity          │
└──────────────────────┘
      │
      ▼
Specialized AI Workflow
      │
      ▼
Better • Faster • Consistent Results
```

---

# ✨ Why Super Skills?

Claude is powerful out of the box.

But complex tasks often require more than a simple prompt.

Super Skills turn repeated instructions into **reusable AI capabilities**.

### Without Skills

```text
User
 ↓
Prompt
 ↓
Claude
 ↓
Generic solution
 ↓
Repeat instructions again
```

### With Skills

```text
User
 ↓
Task detected
 ↓
Relevant Skill activated
 ↓
Specialized workflow
 ↓
Context-aware reasoning
 ↓
Higher-quality result
```

---

# 🧩 Features

| Feature                         | Description                                     |
| ------------------------------- | ----------------------------------------------- |
| 🧠 **Specialized Intelligence** | Give Claude expertise for specific tasks        |
| ⚡ **Reusable Workflows**        | Stop repeating the same instructions            |
| 🧱 **Modular Architecture**     | Each skill is independent and easy to maintain  |
| 🔄 **Automatic Activation**     | Skills can be used when their context matches   |
| 🛠️ **Developer Focused**       | Designed around practical development workflows |
| 📚 **Knowledge Driven**         | Store conventions, patterns and procedures      |
| 🎯 **Consistent Output**        | Reduce variation across repeated tasks          |
| 🔌 **Extensible**               | Easily create and add your own skills           |

---

# 🗂️ Skill Architecture

Each skill follows a simple structure:

```text
skill-name/
│
├── SKILL.md
│
├── references/
│   └── documentation.md
│
├── scripts/
│   └── helper.py
│
└── examples/
    └── example.md
```

At the heart of every skill is:

```text
SKILL.md
```

This file defines what the skill does, when it should be used, and the workflow Claude should follow.

A basic skill can look like:

```yaml
---
name: frontend-development
description: Build modern, accessible and responsive frontend interfaces.
---

# Frontend Development

## Purpose

Provide production-quality frontend development guidance.

## Workflow

1. Understand the requirements
2. Analyze the existing code
3. Plan the implementation
4. Implement the solution
5. Validate the result
6. Improve accessibility and performance

## Guidelines

- Prefer maintainable code
- Follow project conventions
- Avoid unnecessary dependencies
- Consider responsive design
- Validate the final implementation
```

---

# 🧠 Skills

The repository includes focused, task-oriented guides. Browse the [complete skill catalog](skills/README.md), or start with one of these core guides:

### 💻 Development

```text
Frontend Development
Backend Development
API Development
Code Review
Debugging
Refactoring
Software Architecture
```

### 🤖 AI & Automation

```text
AI Engineering
Prompt Engineering
Agent Workflows
Automation
AI Application Development
LLM Integration
```

### 🎨 Design

```text
UI/UX Design
Frontend Design
Responsive Design
Design Systems
Landing Pages
```

### 📊 Research & Productivity

```text
Deep Research
Technical Documentation
Project Planning
Problem Solving
Technical Writing
```

---

---

## 📁 Current Repository Structure

The tree below reflects the current `main` branch. The `skills/` directory contains the maintained skill guides; `docs/` and `examples/` provide supporting material.

```text
ui-ux-pro-max/
├── README.md
├── docs/
├── examples/
├── skills/
│   ├── README.md
│   ├── accessibility-review/
│   ├── api-contract-design/
│   ├── automated-test-strategy/
│   ├── claude-code-project-setup/
## 🧰 Engineering & Agent Workflows

Practical, task-focused guides for building, testing, securing, and maintaining software with AI-assisted workflows.

- [Claude Code Project Setup](skills/claude-code-project-setup/SKILL.md) — establish project context, conventions, and safe working rules.
- [Automated Test Strategy](skills/automated-test-strategy/SKILL.md) — choose a balanced test pyramid and prioritize high-value coverage.
- [API Contract Design](skills/api-contract-design/SKILL.md) — define clear, versionable API contracts and predictable errors.
- [Secure Code Review](skills/secure-code-review/SKILL.md) — review trust boundaries, input handling, authorization, and secrets.
- [React Performance Review](skills/react-performance-review/SKILL.md) — find measurable rendering and bundle bottlenecks.
- [Playwright E2E Testing](skills/playwright-e2e-testing/SKILL.md) — build reliable end-to-end tests around user-critical journeys.
- [Database Migration Review](skills/database-migration-review/SKILL.md) — assess migration safety, rollout order, and rollback plans.
- [LLM Feature Evaluation](skills/llm-feature-evaluation/SKILL.md) — evaluate AI features with datasets, rubrics, and regression checks.
- [MCP Server Development](skills/mcp-server-development/SKILL.md) — design useful, secure Model Context Protocol tools and resources.
- [Incident Response Triage](skills/incident-response-triage/SKILL.md) — structure initial incident assessment, containment, and evidence handling.

Browse the [complete skill catalog](skills/README.md) for all available guides.

---

# ⚡ Installation

## Option 1 — Clone the Repository

```bash
git clone https://github.com/Atharva-ark06/ui-ux-pro-max.git
```

Then enter the project:

```bash
cd ui-ux-pro-max
```

---

## Option 2 — Use Individual Skills

Copy the skill you need into your Claude skills directory:

```bash
cp -r skills/<skill-name> ~/.claude/skills/
```

For example:

```bash
cp -r skills/frontend-development ~/.claude/skills/
```

Restart Claude Code if necessary.

---

# 🧑‍💻 Usage

Once installed, simply work normally with Claude Code.

Instead of writing:

```text
"Please behave like a senior frontend developer,
follow accessibility standards, use responsive design,
review my existing architecture and then implement..."
```

You can simply ask:

```text
Build a responsive dashboard for this project.
```

The relevant skill can provide Claude with the specialized workflow needed for the task.

---

# 🛠️ Creating Your Own Skill

Creating a new skill is intentionally simple.

## 1. Create a directory

```bash
mkdir -p skills/my-skill
```

## 2. Create `SKILL.md`

```bash
touch skills/my-skill/SKILL.md
```

## 3. Add the skill definition

```yaml
---
name: my-skill
description: Describe what this skill does and when Claude should use it.
---

# My Skill

## Purpose

Explain the purpose of the skill.

## Workflow

1. Analyze the request
2. Understand the context
3. Execute the workflow
4. Validate the result
5. Provide the final output

## Guidelines

- Follow project conventions
- Prefer maintainable solutions
- Avoid unnecessary complexity
- Validate before finishing
```

---

# 🧱 Recommended Skill Design

A good skill should answer four questions:

```text
┌───────────────────────────────┐
│          SKILL                │
├───────────────────────────────┤
│                               │
│  1. WHAT does it do?          │
│                               │
│  2. WHEN should it activate?  │
│                               │
│  3. HOW should it work?       │
│                               │
│  4. WHAT rules must it follow?│
│                               │
└───────────────────────────────┘
```

### Good Skills Are

* 🎯 Focused
* 🧩 Modular
* 📖 Well documented
* 🔄 Reusable
* 🛡️ Predictable
* ⚡ Practical

---

# 🔥 Example Workflow

Imagine you have a **Code Review Skill**.

Claude receives:

```text
Review this authentication system.
```

The skill can guide Claude through:

```text
                 USER REQUEST
                      │
                      ▼
              ┌───────────────┐
              │ Understand    │
              │ Codebase      │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │ Security      │
              │ Analysis      │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │ Code Quality  │
              │ Analysis      │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │ Performance   │
              │ Analysis      │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │ Suggestions   │
              └───────┬───────┘
                      │
                      ▼
               FINAL REVIEW
```

This makes the workflow **repeatable instead of prompt-dependent**.

---

# 📁 Suggested Repository Structure

```text
Claude-super-skills/
│
├── 📁 skills/
│   │
│   ├── 📁 development/
│   ├── 📁 frontend/
│   ├── 📁 backend/
│   ├── 📁 ai/
│   ├── 📁 research/
│   ├── 📁 writing/
│   └── 📁 productivity/
│
├── 📁 examples/
│
├── 📁 docs/
│
├── 📄 README.md
├── 📄 LICENSE
└── 📄 CONTRIBUTING.md
```

---

# 🌐 Agent Skills Ecosystem

Claude Skills are part of a broader ecosystem of **agent skills** designed to give AI systems reusable capabilities.

Anthropic's official skills repository describes skills as folders containing instructions, scripts, and resources that Claude can load dynamically for specialized tasks.

This project follows the same general philosophy:

```text
                 AI MODEL
                    │
                    ▼
            ┌──────────────┐
            │ Skill System  │
            └──────┬───────┘
                   │
        ┌──────────┼──────────┐
        ▼          ▼          ▼
   Development   Research   Automation
        │          │          │
        └──────────┼──────────┘
                   ▼
            Specialized AI
```

---

# 🛡️ Best Practices

When creating skills:

### ✅ Do

* Keep each skill focused
* Clearly define activation conditions
* Use concise instructions
* Include practical workflows
* Document assumptions
* Add examples when useful
* Validate outputs

### ❌ Avoid

* Huge unrelated instruction files
* Repeating the same information
* Ambiguous activation criteria
* Unnecessary dependencies
* Hidden destructive actions
* Overly rigid workflows

---

# 🤝 Contributing

Contributions are welcome.

### 1. Fork the repository

```bash
git fork
```

### 2. Create a branch

```bash
git checkout -b feature/my-skill
```

### 3. Add your skill

```text
skills/
└── my-skill/
    └── SKILL.md
```

### 4. Test it with Claude

Make sure the skill behaves consistently across different prompts.

### 5. Commit

```bash
git add .
git commit -m "feat: add my-skill"
```

### 6. Push

```bash
git push origin feature/my-skill
```

Then open a Pull Request.

---

# 📜 License

This project is released under the **MIT License**.

See [`LICENSE`](LICENSE) for details.

---

# 👨‍💻 Author

<p align="center">

<strong>ATHARVA KULKARNI</strong>

<br>

Computer Science • AI/ML • Cyber Security • Full-Stack Development

<br><br>

<a href="https://github.com/Atharva-ark06">
<img src="https://img.shields.io/badge/GitHub-Atharva--ark06-181717?style=for-the-badge&logo=github" />
</a>

</p>

---

# ⭐ Support

If this project helped you build better workflows with Claude:

**⭐ Star the repository**
**🍴 Fork it**
**🧠 Create your own skills**
**🚀 Share it with other developers**

---

<p align="center">


**Claude Super Skills**

</p>

<p align="center">
  <sub>Built for developers who want to get more out of AI.</sub>
</p>