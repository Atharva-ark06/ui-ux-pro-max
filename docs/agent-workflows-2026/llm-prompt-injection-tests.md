# llm prompt injection tests

Use synthetic tests for attempts to exfiltrate secrets, alter tasks, trigger unauthorized tools, override constraints, or exploit indirect instructions in retrieved documents. Expected behavior: treat retrieved content as data, scope tools, require authorization for sensitive actions, and report suspicious instructions. Never use real secrets in fixtures.
