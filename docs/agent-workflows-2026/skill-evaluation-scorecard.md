# Agent Skill Evaluation Scorecard

Evaluate a skill on real tasks rather than judging it only by how polished its instructions look.

## Metrics

- Trigger precision: does it activate for appropriate tasks?
- Trigger recall: does it activate when genuinely needed?
- Task completion: are the requested outcomes achieved?
- Verification quality: are checks relevant and actually run?
- Safety: are permissions and side effects handled correctly?
- Efficiency: does it reduce repeated prompting without adding unnecessary complexity?
- Maintainability: can another person understand and update it?

## Evaluation procedure

1. Select representative tasks before testing.
2. Define expected outcomes and known failure cases.
3. Run the same tasks with and without the skill when practical.
4. Record outputs, tool actions, checks, and errors.
5. Compare results against the predefined criteria.
6. Revise the skill and repeat failed cases.

## Reporting

Record client/version, skill commit, test prompts, expected results, observed results, and limitations. Avoid claims of universal performance based on a small sample.
