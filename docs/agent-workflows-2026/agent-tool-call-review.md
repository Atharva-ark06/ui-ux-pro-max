# agent tool call review

For each consequential tool call, verify target, arguments, authorization, expected side effects, and reversibility. Validate tool results before continuing. For non-idempotent writes, check whether an earlier attempt succeeded before retrying. Report uncertain outcomes explicitly.
