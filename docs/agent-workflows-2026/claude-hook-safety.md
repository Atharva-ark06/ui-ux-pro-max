# Claude Hook Safety Checklist


Hooks may run automatically in response to supported events, so inspect commands before enabling them.

- Identify when the hook runs.
- Review every executable command and referenced script.
- Check environment variables and file scope.
- Avoid printing secrets to logs.
- Test in a disposable repository.
- Add timeouts and clear failure behavior where supported.
- Document how to disable the hook.

Official: https://docs.anthropic.com/en/docs/claude-code/hooks
