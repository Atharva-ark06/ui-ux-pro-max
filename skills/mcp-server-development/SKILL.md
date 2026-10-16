---
name: mcp-server-development
description: Design, implement, and review Model Context Protocol servers and tools with clear schemas, bounded permissions, and robust error handling. Use when exposing APIs, files, or workflows to an AI client through MCP.
---

# MCP Server Development

## Design the tool surface
1. Identify the exact user workflow and smallest set of tools needed.
2. Give each tool a specific name, concise description, typed input schema, and predictable output.
3. Separate read operations from state-changing operations.
4. Validate inputs at the server boundary; never rely on the model to enforce constraints.
5. Return useful structured errors without exposing secrets, stack traces, or internal filesystem details.

## Security and permissions
- Apply least privilege to credentials, filesystem paths, and network destinations.
- Enforce authorization in the server for every operation.
- Restrict file access to approved roots and normalize paths to prevent traversal.
- Validate URLs and destinations to reduce server-side request forgery risks.
- Require confirmation or a separate explicit workflow for destructive or externally visible actions.
- Treat tool arguments and resource contents as untrusted input.
- Never place API keys in tool descriptions, sample outputs, logs, or repository files.

## Reliability
- Set sensible timeouts, output limits, and cancellation behavior.
- Make retries safe; use idempotency controls for operations that may mutate state.
- Distinguish expected user errors from service failures.
- Avoid returning huge payloads when a summary plus pagination or resource reference is enough.
- Keep logs useful while redacting tokens and sensitive data.

## Implementation and tests
- Follow the current official SDK and protocol version used by the project.
- Validate schemas and error cases.
- Test missing fields, wrong types, oversized inputs, denied permissions, timeouts, and dependency failures.
- Test that tools cannot access paths or resources outside their authorized scope.
- Document setup, configuration, required permissions, and example invocations.

## Completion criteria
A consumer can discover each tool, understand its effects, supply valid arguments, and recover from failures. Security controls are enforced by code, not merely described in the prompt. Confirm protocol and SDK details against current official documentation before relying on version-specific APIs.
