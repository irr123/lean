---
name: lean-transfer
description: Transfer the relevant context from the current session through one self-contained Markdown file under $TMPDIR. Use when work needs to continue in a fresh session or move to another agent.
disable-model-invocation: true
---

# Lean transfer

Sole write: one Markdown handoff file under $TMPDIR.

1. Establish what the receiving session must continue; use the active objective when no narrower focus is supplied.
2. Compact the relevant context into a self-contained brief. Include the goal and scope, current state, decisions and evidence, workspace instructions and relevant paths, completed and remaining work, success criteria, validation information, assumptions, unresolved questions, and the next action when applicable.
3. Redact secrets and personally identifiable information, then save the brief under a unique, descriptive `$TMPDIR` filename.
4. Report the absolute path and stop.

The transfer is complete when a fresh session can continue without this conversation and exactly one temporary artifact was created. Perform no implementation or validation run.
