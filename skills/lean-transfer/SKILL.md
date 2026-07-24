---
name: lean-transfer
description: Preserve context selected by the user in one self-contained Markdown handoff in the system temporary directory. Report the absolute path and stop. Explicit invocation required; in-chat summaries stay in chat.
---

# Lean transfer

Sole write: one Markdown handoff file in the system temporary directory. Selected context is the information the user chose to preserve. The handoff contains that context for a fresh session or another agent.

1. Establish the selected context; use the active topic when the user supplies no narrower scope.
2. Compact that context so a fresh session can recover the user's scope, current state, supporting evidence, decisions, and unresolved questions. Include intended follow-up only when the user stated one; an imperative goal ("do one more review pass", "fix X") is that follow-up, not a signal to switch skills and act on it now. Add instructions, validation details, assumptions, and risks only when relevant. Preserve citations for material facts and separate observations from assumptions. Reference already-persisted artifacts (specs, plans, ADRs, issues, diffs) by path or URL instead of duplicating their content.
3. Redact secrets and personally identifiable information. Mark any context lost to redaction. Resolve the system temporary directory through the runtime or platform. Create one unique handoff atomically with owner-only permissions where supported. Remove partial files and abort if creation or restrictive permissions fail.
4. Reread the handoff without relying on conversation history. Verify that the receiver can understand the selected context, trace material claims, distinguish decisions from assumptions, and see unresolved questions without inferring a course of action. Confirm readable Markdown, exactly one handoff, an absolute path, and restrictive permissions where supported. Report the absolute path and stop.

Transfer is complete when a fresh session has the selected context without this conversation and exactly one temporary handoff exists. Validate only the handoff. Perform no implementation or workspace validation run.
