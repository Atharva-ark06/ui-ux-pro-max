# Agent Tool Permission Matrix

| Action | Default handling |
| --- | --- |
| Read files in task scope | Usually allowed |
| Propose edits | Allowed |
| Modify local files | Requires task authorization |
| Install packages | Review purpose and lockfile impact |
| Access external services | Requires configured access and a clear purpose |
| Publish content or send messages | Explicit authorization required |
| Delete or overwrite shared data | Confirm exact target and impact |
| Deploy to production | Separate explicit authorization |

## Scope questions

- What repository, workspace, file, or account is in scope?
- Is this read-only, local-edit, or external-write work?
- Which actions need confirmation?
- What should happen if the target is ambiguous?
- Which checks must pass before reporting success?

Grant only the permissions needed. A skill describes a workflow; client and service permissions determine what actions are actually possible.
