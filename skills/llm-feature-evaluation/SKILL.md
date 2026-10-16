---
name: llm-feature-evaluation
description: Evaluate LLM-powered features with representative datasets, explicit rubrics, safety checks, and regression tracking. Use when adding prompts, RAG, agents, model changes, or AI-generated user-facing content.
---

# LLM Feature Evaluation

## Define the task
Specify intended users, inputs, acceptable outputs, failure costs, latency and cost constraints, and what the model must never do. Convert broad goals such as “better answers” into observable criteria.

## Build a representative evaluation set
- Sample realistic inputs, including common, difficult, ambiguous, and adversarial cases.
- Include empty, malformed, multilingual, long-context, and out-of-scope inputs where relevant.
- Remove personal or confidential information unless there is a justified, authorized need.
- Keep a held-out set to reduce tuning against the same examples.
- Version the dataset, prompt, model, retrieval configuration, and evaluation rubric.

## Evaluate multiple dimensions
- **Task quality:** correctness, completeness, relevance, and instruction adherence.
- **Grounding:** whether claims are supported by provided context or trusted sources.
- **Safety:** refusal quality, sensitive-data handling, prompt-injection resistance, and tool-use boundaries.
- **Robustness:** paraphrases, noisy input, edge cases, and conflicting context.
- **Operations:** latency, token usage, failure rate, and cost per successful task.

Use exact checks for deterministic requirements and human-reviewed rubrics for nuanced judgments. Model-based graders can help scale review but must themselves be validated against human judgments.

## RAG and tool-using systems
Test retrieval separately from generation. Include missing evidence, misleading retrieved passages, stale documents, and instructions embedded in untrusted content. Verify that tools enforce authorization independently of model instructions and that the model cannot treat retrieved text as privileged commands.

## Release gates
Set thresholds based on risk and establish a baseline before changing prompts or models. Inspect regressions by category, not only the aggregate score. Use staged rollout and monitoring for high-impact features.

## Report
Record evaluation set version, configuration, metrics, representative failures, human-review notes, latency/cost, and release decision. Do not describe a small or unrepresentative benchmark as proof of general reliability.
