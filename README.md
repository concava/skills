# concava

A Claude Code plugin that bundles the skills I use day to day. Each skill is
invoked as `/concava:<skill>`, or loaded by Claude automatically when its
description matches the task.

I did not write these skills. Each one is copied from its original publisher,
credited below, and kept here so I can install and update them as one plugin.

## Skills

| Skill | What it does | Original publisher | Source | License |
|---|---|---|---|---|
| `improve-codebase-architecture` | Scans a codebase for deepening opportunities, reports them as HTML, then grills you on the one you pick | Matt Pocock | [mattpocock/skills](https://github.com/mattpocock/skills/tree/main/skills/engineering/improve-codebase-architecture) | MIT |
| `codebase-design` | Shared vocabulary for designing deep modules: module, interface, depth, seam, adapter | Matt Pocock | [mattpocock/skills](https://github.com/mattpocock/skills/tree/main/skills/engineering/codebase-design) | MIT |
| `code-review` | Reviews changes since a fixed point on two axes, repo standards and the originating spec, in parallel sub-agents | Matt Pocock | [mattpocock/skills](https://github.com/mattpocock/skills/tree/main/skills/engineering/code-review) | MIT |
| `grill-me` | A relentless interview to sharpen a plan or design | Matt Pocock | [mattpocock/skills](https://github.com/mattpocock/skills/tree/main/skills/productivity/grill-me) | MIT |
| `better-ui` | Exact values for border radius, optical alignment, shadows, icon states and animation | Jakub Krehel | [jakubkrehel/skills](https://github.com/jakubkrehel/skills/tree/main/skills/better-ui) | MIT |
| `motion-design` | Timing, easing, choreography and animation principles for UI motion | LottieFiles | [LottieFiles/motion-design-skill](https://github.com/LottieFiles/motion-design-skill) | MIT |
| `codex` | Runs the OpenAI Codex CLI (`codex exec`, `codex resume`) for analysis, refactoring or edits | skills-directory | [skills-directory/skill-codex](https://github.com/skills-directory/skill-codex) | MIT |
| `ste` | Rewrites text in ASD-STE100 Simplified Technical English so an agent cannot misread it | Dustin Yuchen Teng (danyuchn) | [danyuchn/asd-ste100-skill](https://github.com/danyuchn/asd-ste100-skill) | MIT |
| `agentation` | Adds the Agentation visual feedback toolbar to a Next.js project | Benji Taylor | [benjitaylor/agentation](https://github.com/benjitaylor/agentation/tree/main/skills/agentation) | PolyForm Shield 1.0.0 |

### Changes from the originals

- `improve-codebase-architecture`: references to `codebase-design` now say
  `concava:codebase-design`, so the skill finds its sibling inside this plugin.
- `ste`: renamed from `asd-ste100` to `ste`.

Every other skill is unchanged from its source.

## Install

```
/plugin marketplace add concava/skills
/plugin install concava@concava
```

## Update a skill

1. Edit the skill under `skills/<name>/SKILL.md`, or copy in a newer version
   from its source above.
2. Bump `version` in `.claude-plugin/plugin.json`.
3. Push, then run `/plugin marketplace update concava`.

## Licenses

Each skill keeps the license of its source, listed in the table. The full
license text and copyright notice for every source is in
[NOTICES.md](NOTICES.md). `agentation` is under the PolyForm Shield License
1.0.0, which permits use but not in a product that competes with Agentation.
