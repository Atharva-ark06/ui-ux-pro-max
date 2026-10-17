# Agent Skill Quality Rubric

Use this rubric to evaluate whether a skill is worth keeping and sharing.

Score each category from 0 to 2: 0 = missing, 1 = partial, 2 = clear and tested.

| Category | 0 | 1 | 2 |
| --- | --- | --- | --- |
| Trigger | Unclear | Broad or incomplete | Specific use cases and boundaries |
| Workflow | Vague | Some actionable steps | Ordered, repeatable steps |
| Inputs/outputs | Not defined | Implied | Explicitly documented |
| Verification | None | Generic | Observable checks or tests |
| Safety | Missing | General warning | Concrete permissions and stop conditions |
| Modularity | Monolithic | Some separation | Focused instructions with linked references |
| Portability | Machine-specific | Some assumptions | Clear prerequisites and portable paths |
| Maintenance | No owner/source | Partial metadata | Source, license, version/review date |

Maximum score: 16.

## Interpretation

- 14–16: Ready to share after security review.
- 10–13: Useful draft; address weak categories before broad adoption.
- 0–9: Rework the scope, workflow, or safety guidance.

A high score is not a security guarantee. Scripts, dependencies, and external actions still require review.

## Test plan

Test at least:
1. One task that should trigger the skill.
2. One similar task that should not trigger it.
3. One task with missing inputs.
4. One task that might cause side effects.
5. One failure or edge case.

Document the results so future maintainers can reproduce them.
