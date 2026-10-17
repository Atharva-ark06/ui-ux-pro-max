# Agent Output Verification Protocol

Treat generated output as a proposal until it passes checks appropriate to the task.

## Code
- Inspect the diff for unrelated edits.
- Run relevant formatters, linters, type checks, tests, and builds.
- Review dependency changes and error handling.
- Check for secrets and scope violations.

## Design
- Compare with the source at matching viewports.
- Check typography, spacing, tokens, and component states.
- Verify keyboard access, focus, and contrast.
- Report remaining visual differences.

## Research and documentation
- Verify important claims against primary sources.
- Check links, dates, versions, and licensing.
- Separate facts from recommendations and uncertainty.

## External actions
- Verify target and authorization before publishing, deleting, or deploying.
- Confirm completion before reporting success.

## Final report
1. Changed
2. Verified (with actual results)
3. Not verified
4. Known risks
5. Next required step
