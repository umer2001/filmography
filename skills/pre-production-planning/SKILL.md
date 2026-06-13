---
name: pre-production-planning
description: Use when starting an AI-native film or video project and the project foundation, continuity rules, visual bible, or delivery targets are not yet defined.
---

# Pre-Production Planning

## Overview

This skill creates the project foundation that all scene-level work inherits. It is for AI-native production pipelines, so it focuses on story, look, continuity, and generation constraints rather than physical shoot logistics.

## Inputs To Clarify

- Project goal and intended audience
- Runtime or format targets
- Story premise and tone
- Visual references and medium influences
- Character and world continuity needs
- Delivery targets such as aspect ratio, resolution, and platform variants

## Outputs

Create:
- `docs/project/project-foundation.md` using [templates/project-foundation.md](/home/umer2001/projects/filmography/templates/project-foundation.md)
- `docs/story/foundation.md` using [templates/story-foundation.md](/home/umer2001/projects/filmography/templates/story-foundation.md)
- `docs/story/screenplay.md` using [templates/screenplay.md](/home/umer2001/projects/filmography/templates/screenplay.md)

The project-level workflow should move through these phases:
1. concept intake and clarification
2. story foundation
3. early project foundation with a lightweight bible skeleton
4. full screenplay as a required gate
5. blocking screenplay-reviewer pass
6. screenwriter revision and re-review when needed
7. human screenplay approval
8. per-scene screenplay file generation
9. extraction proposal
10. reviewed and approved derived-doc generation
11. locked project foundation

## Hard Gates

- Do not start scene-level shot or prompt work until the project foundation and full screenplay exist.
- Treat the full screenplay as a required gate before any `scene-package.md` work.
- Do not send the screenplay to human approval until `screenplay-reviewer` has produced a review report, unless the human explicitly invokes an override.
- If `screenplay-reviewer` returns `No` or `With revisions`, route the report back to the Screenwriter and re-review after revisions.
- After screenplay approval, generate `docs/story/scenes/<scene-id>.md` automatically before the extraction proposal.
- Generate only `required` derived docs first; ask before expanding into `useful` docs.
- Exclude physical-production budgeting, location logistics, and crew scheduling unless the user explicitly asks for them.
- Favor reusable continuity rules over scene-specific improvisation.
