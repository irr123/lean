---
name: lean-transfer
description: Write one Markdown handoff to a temp file.
allowed-tools: read write Read Write
disallowed-tools: mcp__custom-tools__write mcp__custom-tools__edit
disable-model-invocation: true
---

# Lean transfer

Write one Markdown handoff to the temp directory. Nothing else.

1. Preserve what a fresh agent needs to resume: scope, state, evidence, decisions, open questions, and goals. Cite sources; reference persisted artifacts by path. Separate evidence from assumptions.
2. Redact secrets and PII. Write one owner-only file.
3. Report the absolute path.
