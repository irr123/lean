# Lean

[![CI](https://github.com/irr123/lean/actions/workflows/ci.yml/badge.svg)](https://github.com/irr123/lean/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

Research returns cited findings. Transfer creates a handoff. Apply produces a validated change.

Three independent Agent Skills for user-directed, scoped coding work. Research answers a question without making changes. Transfer preserves selected context in one temporary handoff. Apply produces the requested outcome with the smallest complete change and validates it. Invoke any skill independently or combine them in the order the user chooses.

## Install

```bash
npx skills add irr123/lean
```

## Skills

| Skill | Job | Side effect |
|---|---|---|
| `lean-research` | Answer a question with cited findings | Reads the workspace and external sources without intentional changes |
| `lean-transfer` | Preserve selected context in one handoff | Writes one temporary Markdown file |
| `lean-apply` | Produce the requested outcome with a validated change | May edit files and run workspace commands |

Apply and Transfer are intended for explicit invocation. Some hosts may invoke skills differently.

## Language

A request is the user's current instruction; its scope defines what is included and excluded. Context is information relevant to a request; it is consulted, not implemented. Evidence supports Research findings. Selected context becomes a Transfer handoff. Apply produces a measurable outcome through the smallest complete change, then validates it.

## Examples

```text
/skill:lean-research Investigate why authentication occasionally fails
/skill:lean-transfer Preserve the selected context for a fresh session
/skill:lean-apply @/tmp/<handoff>.md
```

## License

[MIT](LICENSE)
