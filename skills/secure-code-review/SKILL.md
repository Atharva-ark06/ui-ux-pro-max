---
name: secure-code-review
description: Review code changes for security weaknesses, trust-boundary mistakes, and unsafe data handling. Use when reviewing authentication, authorization, file handling, APIs, dependencies, secrets, or security-sensitive refactors.
---

# Defensive Secure Code Review

## Review approach
1. Establish the intended behavior and assets being protected.
2. Trace untrusted input from entry points to sensitive operations.
3. Identify trust boundaries, privilege changes, data storage, network calls, and external dependencies.
4. Prioritize exploitable impact and realistic attack paths over speculative style concerns.
5. Confirm findings against code and tests; do not report a vulnerability based on a keyword alone.

## Areas to inspect
- **Authentication:** session lifecycle, token validation, expiration, logout, reset flows, and multi-factor checks.
- **Authorization:** object-level ownership, role and tenant boundaries, privilege escalation, and server-side enforcement.
- **Input handling:** injection, unsafe deserialization, path traversal, template injection, malformed encodings, and size limits.
- **Web protections:** CSRF, XSS, redirect validation, security headers, and cookie attributes as applicable.
- **Secrets and privacy:** hard-coded credentials, tokens in logs, overbroad data access, and unnecessary retention.
- **Files and uploads:** type and size validation, path handling, storage isolation, and safe processing of untrusted content.
- **Dependencies and builds:** vulnerable or untrusted packages, lockfile changes, exposed build secrets, and risky install scripts.
- **Failure paths:** verbose errors, fail-open behavior, incomplete cleanup, and unsafe retries.

## Finding format
For each credible issue report:
- Title and severity.
- Affected file and exact code location.
- Preconditions and required attacker capability.
- Concrete path from input to impact.
- Evidence and reproduction steps safe for the authorized environment.
- Recommended fix and regression test.
- Confidence and any uncertainty.

## Safe boundaries
Only perform active testing against systems the user owns or is explicitly authorized to assess. Prefer static review and local test environments. Do not retrieve, expose, or reproduce real secrets; redact them and recommend rotation if a secret appears exposed. Do not execute suspicious code merely to inspect it.

## Verification
Check whether existing controls already mitigate the suspected issue. Run relevant tests or static analyzers if available. Separate confirmed vulnerabilities from hardening recommendations and hypothetical concerns. Never claim a clean security audit from a limited diff review.
