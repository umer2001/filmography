---
name: scene-packaging
description: Use when an approved per-scene screenplay file exists and the scene needs a short interpretation preview plus an approved scene package before shot generation.
---

# Scene Packaging

## Overview

Scene-packaging turns a screenplay-derived scene file into a downstream planning artifact. It does not rewrite the screenplay. It previews the intended interpretation first, then creates `scene-package.md` only after approval.

## Required Inputs

- `docs/story/scenes/<scene-id>.md`
- project-level continuity anchors and relevant character/environment docs

## Output Sequence

1. Create `docs/scenes/<scene-id>/scene-interpretation-preview.md` using [templates/scene-interpretation-preview.md](/home/umer2001/projects/filmography/templates/scene-interpretation-preview.md)
2. Ask for approval
3. Create `docs/scenes/<scene-id>/scene-package.md` using [templates/scene-package.md](/home/umer2001/projects/filmography/templates/scene-package.md)

## Preview Content

The preview should summarize:
- scene purpose
- emotional arc
- likely visual priorities
- continuity-sensitive elements
- what the eventual scene package will emphasize

## Hard Gates

- Do not create `scene-package.md` before preview approval.
- Do not rewrite the scene's story meaning, outcome, or locked dialogue.
- Use the per-scene screenplay file as the local source of truth and the master screenplay when global continuity needs checking.
