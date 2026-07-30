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
| `lean-apply` | Make a checked change | Edits and commands |

All three require direct invocation, and pre-approve only the tools their job needs. Pi and Claude Code read `disable-model-invocation`; Codex reads `policy.allow_implicit_invocation` from `agents/openai.yaml`. OpenCode ignores both fields, so gate them in `opencode.json`:

```json
{
  "permission": {
    "skill": { "lean-*": "ask" }
  }
}
```

## Examples

```text
/skill:lean-research Investigate a deployment failure
/skill:lean-transfer Preserve context
/skill:lean-apply @/tmp/<handoff>.md
```

[MIT](LICENSE)
