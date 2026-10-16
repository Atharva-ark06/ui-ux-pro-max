---
name: api-contract-design
description: Design, review, or evolve HTTP and event API contracts with clear schemas, errors, compatibility, and examples. Use when creating endpoints, changing payloads, documenting APIs, or coordinating service integrations.
---

# API Contract Design

## Contract-first workflow
1. Identify consumers, authentication model, data sensitivity, latency expectations, and versioning constraints.
2. Define resources and user actions before choosing route names. Prefer consistent nouns, HTTP semantics, and predictable pagination/filter conventions.
3. Specify request fields, types, requiredness, constraints, defaults, response shape, and examples.
4. Define error behavior for validation, authentication, authorization, missing resources, conflicts, rate limits, and unexpected failures.
5. Decide how the contract evolves and what compatibility guarantees consumers need.
6. Add executable schema validation or contract tests when the stack supports it.

## HTTP design
- Use safe methods for read-only operations and appropriate mutation methods for changes.
- Return status codes that reflect the outcome; do not encode every failure as a successful response.
- Make pagination explicit and stable. Document sorting and filtering semantics.
- Use idempotency keys or equivalent safeguards for retry-sensitive operations when appropriate.
- Keep internal stack traces, secrets, and sensitive implementation details out of client-facing errors.
- Avoid ambiguous fields whose meaning changes based on the caller or context.

## Schema quality
- Prefer explicit names and stable types.
- Distinguish omitted, null, empty, and default values.
- Specify timestamp format, timezone assumptions, identifier semantics, units, and enum behavior.
- Decide whether unknown fields are rejected, ignored, or preserved.
- Include realistic examples and boundary cases.
- Keep sensitive values out of logs and sample payloads.

## Compatibility review
For every change, classify it as additive, behavior-changing, or breaking. Consider removing or renaming fields, narrowing accepted values, changing defaults, changing ordering, and altering error codes as potentially breaking. Search consumers and generated clients before changing a shared contract.

## Security review
- Enforce authorization on the server for every protected resource and action.
- Validate input at trust boundaries; client validation is not a security boundary.
- Apply rate limits and size limits where abuse or resource exhaustion is plausible.
- Avoid exposing whether a sensitive account or record exists when that distinction creates risk.
- Document scopes, ownership checks, and audit requirements.

## Deliverables
Provide the contract, sample success and error responses, compatibility notes, validation plan, and any migration steps. Label assumptions that require confirmation.
