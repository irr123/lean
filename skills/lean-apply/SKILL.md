---
name: lean-apply
description: Produce the user's requested outcome in a trusted workspace. Use a supplied handoff as context when present, verify current workspace state, make the smallest complete change within the requested scope, validate it, and report the results. Explicit invocation required.
---

# Lean apply

Use only in a trusted workspace. The request is the user's current instruction; its scope defines what is included and excluded. Context informs implementation but is not itself implemented. The outcome is the measurable state the request asks Apply to produce.

Read any supplied handoff and applicable instruction files in full. Current workspace state is authoritative. Verify material handoff claims, paths, and decisions before editing.

Execute directly without follow-up questions for normal workspace edits and checks. Preserve or request confirmation before destructive, publishing, deployment, credential, or irreversible operations. For missing low-risk, reversible details, state the smallest assumption and continue. Ask when ambiguity changes behavior, success criteria, security, data, or irreversible outcomes. When instructions conflict, name both sides, choose one, explain why, and continue.

State the measurable outcome within scope, then:

1. Make the smallest complete change that produces it using established patterns. Leave adjacent work untouched.
2. Add or update checks and documentation needed to prove the outcome, following existing practice.
3. Run the narrowest relevant checks during implementation, then the workspace's prescribed final validation. Do not report a check as passing unless it was run fresh in this turn.
4. Review the change for correctness, regressions, accidental scope, and unnecessary complexity; fix concrete issues.
5. Report changed files, validation results, skipped or failed checks, and remaining risks.

Keep durable guidance in the workspace's existing instruction files when the task calls for it. Lean itself adds no project documents. In a repository, commit only when the user asks.
