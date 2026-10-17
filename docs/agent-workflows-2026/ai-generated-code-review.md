# AI-Generated Code Review Checklist

Review AI-generated code with the same standards as human-written code.

## Correctness
- Does the change meet the acceptance criteria?
- Are edge cases and error paths handled?
- Does it preserve existing contracts and behavior?
- Are tests meaningful and not tailored only to the implementation?

## Security and privacy
- Is input validated at the appropriate boundary?
- Are authorization checks enforced server-side?
- Are secrets and personal data protected?
- Are dependencies and generated scripts understood?

## Maintainability
- Does the code follow local conventions?
- Is complexity justified?
- Are comments and docs accurate?
- Were unrelated files changed?

## Verification
Run relevant tests and checks, inspect the diff, and state what was not tested. Do not merge based solely on a confident explanation from the agent.