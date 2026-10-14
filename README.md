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
| `lean-extract` | Summarize raw material and map distinct positions | None |
| `lean-research` | Research a question with testable hypotheses | None |
| `lean-transfer` | Preserve selected context | One temporary handoff |

`lean-transfer` requires direct invocation because it writes a handoff. The remaining skills can be invoked when relevant. Pi and Claude Code read `disable-model-invocation`; Codex reads `policy.allow_implicit_invocation` from `agents/openai.yaml`. OpenCode ignores both fields, so gate the direct-invocation skill in `opencode.json`:

```json
{
  "permission": {
    "skill": { "lean-transfer": "ask" }
  }
}
```

## Examples

```text
/skill:lean-research Find an indie SaaS niche from vendor trigger events
/skill:lean-transfer
```

[MIT](LICENSE)
