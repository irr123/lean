---
name: lean-transfer
description: Write one Markdown handoff to a temp file. Use when ending a session or handing work to a fresh agent.
allowed-tools: read write Read Write
disallowed-tools: mcp__custom-tools__write mcp__custom-tools__edit
disable-model-invocation: true
---

# Lean transfer

1. Write `$TMPDIR/handoff-<YYYYmmdd-HHMM>.md`, mode 600.
2. Sections, in order: session log path (absolute), scope, state, evidence, decisions, open questions, goals. Cite sources; reference artifacts by path. Mark assumptions apart from evidence.
3. Redact secrets and PII.
4. Report the absolute path.
