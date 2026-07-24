---
name: lean-apply
description: Apply supplied context immediately in the active session using the workspace's own instructions and conventions. Intended for invocation in a fresh receiving session.
disable-model-invocation: true
---

# Lean apply

Read the supplied context in full. Read applicable instruction files when present, then inspect the workspace's existing materials, conventions, and validation methods.

Execute directly without follow-up questions. When details are missing, state the smallest assumption and continue. When instructions conflict, name both sides, choose one, explain why, and continue.

State the measurable outcome, then:

1. Implement the smallest complete change that produces it using established patterns.
2. Update accompanying checks or documentation only where existing practice requires them.
3. Run the workspace's applicable checks (tests, dry-runs, previews, proofread) during work and its final validation.
4. Review the resulting changes for correctness, regressions, accidental scope, and unnecessary complexity; fix concrete issues.
5. Report changed files, validation performed, skipped or failed checks, and remaining risks.

Keep durable guidance in the workspace's existing instruction files when the task calls for it. Lean itself adds no project documents. In a repository, commit only when the user asks.
