# Lean

[![CI](https://github.com/irr123/lean/actions/workflows/ci.yml/badge.svg)](https://github.com/irr123/lean/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

Motivation https://bogomolov.work/blog/posts/rotten-specs/

## Install

```bash
npx skills add irr123/lean
```

## Skills

| Skill | Job | Side effect |
|---|---|---|
| `lean-research` | Research with cited findings | None |
| `lean-transfer` | Preserve selected context | One temporary handoff |
| `lean-niche` | Hunt niches from vendor trigger events | None |

`lean-transfer` and `lean-niche` require direct invocation (one for its write, one for its subagent fan-out cost); the model may reach for `lean-research` on its own. Each pre-approves only the tools its job needs. Pi and Claude Code read `disable-model-invocation`; Codex reads `policy.allow_implicit_invocation` from `agents/openai.yaml`. OpenCode ignores both fields, so gate the direct-invocation skills in `opencode.json`:

```json
{
  "permission": {
    "skill": { "lean-transfer": "ask", "lean-niche": "ask" }
  }
}
```

## Examples

```text
/skill:lean-research Investigate a deployment failure
/skill:lean-transfer Preserve context
do, verify, report @/tmp/<handoff>.md
/skill:lean-niche Find an indie SaaS niche from vendor trigger events
```

[MIT](LICENSE)
