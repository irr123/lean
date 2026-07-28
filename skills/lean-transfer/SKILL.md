---
name: lean-transfer
description: Create one temporary Markdown handoff from selected context. Explicit invocation required.
---

# Lean transfer

Write one Markdown handoff in the system temporary directory. Nothing else.

1. Use the active topic when the user gives no narrower context.
2. Preserve scope, state, evidence, decisions, unresolved questions, and stated follow-up, including imperative goals. Keep citations. Separate observations from assumptions. Reference persisted artifacts by path or URL.
3. Redact secrets and PII. Mark loss. Resolve temp directory. Atomically create one unique owner-only file where supported. Clean partial files; abort on creation or permission failure.
4. Reread without history. Verify recoverability, material claims, decisions, assumptions, questions, Markdown, one file, absolute path, and permissions. Report path. Stop.
