# concava skills

Personal Claude Code plugin. Skills are invoked as `/concava:<skill>`.

| Skill | What it does |
|---|---|
| `improve-codebase-architecture` | Scans a codebase for deepening opportunities, reports them as HTML, then grills through the one you pick |
| `codebase-design` | Shared vocabulary for designing deep modules |
| `code-review` | Reviews changes since a fixed point against repo standards and the originating spec |
| `grill-me` | A relentless interview to sharpen a plan or design |
| `codex` | Runs the OpenAI Codex CLI for analysis or edits |
| `motion-design` | Motion design principles for UI animation |
| `better-ui` | Exact values for radius, alignment, shadows, icon states and animation |
| `agentation` | Adds the Agentation feedback toolbar to a Next.js project |
| `ste` | Rewrites text in Simplified Technical English |

## Install

```
/plugin marketplace add concava/skills
/plugin install concava@concava
```

## Update

Edit a skill under `skills/`, bump `version` in `.claude-plugin/plugin.json`, push, then run `/plugin marketplace update concava`.
