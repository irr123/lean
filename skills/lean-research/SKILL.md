---
name: lean-research
description: Research a task, question, or problem through read-only investigation, using parallel subagents when there are multiple independent angles, then synthesize only relevant findings into the current session. Use before acting or when evidence is needed without intentional changes.
---

# Lean research

Operate read-only: inspect and synthesize without intentionally changing the workspace or external systems.

1. Read applicable instruction files when present, then identify the request's distinct research angles.
2. Decompose into non-overlapping tasks. For multiple independent angles, delegate them to read-only agents in one parallel `subagent` call; runtime manages actual concurrency. Make every delegated prompt self-contained and require evidence in its response rather than a file.
3. Investigate any gaps (or, without subagent, all angles) inline with read-only tools. Use external sources only when needed, preferring official documentation, specifications, source code, and first-party APIs.
4. Distill the returned evidence into the current session: relevant local paths and line ranges, external links, constraints, risks, unknowns, likely touchpoints for the change, and available ways to validate it.

Research is complete when every material finding is supported, contradictions and assumptions are explicit, and the current session contains enough relevant context for a decision or transfer. Produce no deliverable artifact and perform no implementation or workspace-mutating validation run.
