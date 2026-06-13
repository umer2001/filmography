# Filmography Project-Level Workflow Design

## Goal

Extend Filmography beyond the scene workflow so it supports a screenplay-first project-level workflow that is efficient for agents and explicit about approval gates.

## Main Workflows

Filmography has two main workflows:

1. project-level workflow
2. scene workflow

## Project-Level Workflow

1. user idea intake
2. concept clarification
3. story foundation
4. early project foundation with a lightweight bible skeleton
5. full screenplay
6. screenplay-reviewer checks story quality and approval readiness
7. screenwriter revises and re-runs review when needed
8. human screenplay approval gate
9. auto-generate per-scene screenplay files
10. extraction proposal
11. script-breakdown-reviewer checks coverage and doc priority
12. human breakdown approval
13. generate `required` derived docs
14. ask whether to expand into `useful` docs
15. lock project foundation

## Key Decisions

- The full screenplay is a required gate before any scene workflow begins.
- The screenplay-reviewer is a blocking gate before human screenplay approval, unless the human explicitly overrides it.
- The screenplay-reviewer may also be invoked manually by the human for an extra screenplay audit at any time.
- Per-scene screenplay files are derived automatically after screenplay approval.
- `scene-package.md` is generated later from a per-scene screenplay file, not directly from the master screenplay.
- Scene-packaging must show a short interpretation preview and get approval before generating `scene-package.md`.
- The breakdown reviewer checks characters, environments, important props, relationships, factions/groups, and motifs when they affect continuity.
- The reviewer also recommends `required`, `useful`, or `optional` priority for each proposed derived doc.
- Derived docs are generated in two passes: `required` first, `useful` only after a follow-up approval.

## Agent-Optimized File Strategy

- `docs/story/screenplay.md` is the canonical master screenplay
- `docs/story/scenes/<scene-id>.md` provides compact local context for downstream scene agents
- project docs live in targeted folders so agents can pull only what they need

## Derived Doc Structure

- `docs/characters/<character-slug>/profile.md`
- `docs/characters/<character-slug>/continuity.md`
- `docs/environments/<environment-slug>/description.md`
- `docs/environments/<environment-slug>/continuity.md`
- `docs/continuity/anchors.md`
- `docs/story-elements/relationships/<slug>.md`
- `docs/story-elements/factions/<slug>.md`
- `docs/story-elements/motifs/<slug>.md`

Important props stay inside character/environment docs unless they are especially important and recurring.
