# agent failure recovery

Plan for unavailable tools, expired authentication, rate limits, partial writes, malformed output, and ambiguous targets. Use bounded retries for transient failures. Check state before retrying non-idempotent writes. Preserve user work and report completed, failed, and unknown states separately.
