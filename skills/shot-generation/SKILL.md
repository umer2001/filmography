---
name: shot-generation
description: Use when a scene package exists and the scene needs continuity-aware cinematic coverage before reference planning, sound design, or prompt generation.
---

# Shot Generation

## Overview

Shot-generation turns a completed scene package into a shot plan. Its job is to interpret how the scene should be seen without changing what the scene means.

## Required Inputs

- A scene package using [templates/scene-package.md](/home/umer2001/projects/filmography/templates/scene-package.md)
- The rules in [docs/contracts/shot-generation-input.md](/home/umer2001/projects/filmography/docs/contracts/shot-generation-input.md)

## Output

Create `shot-plan.md` using [templates/shot-plan.md](/home/umer2001/projects/filmography/templates/shot-plan.md).

The shot plan should include:
- scene coverage strategy
- locked story beats
- must-see and must-understand moments
- continuity anchors
- shot-by-shot coverage
- likely execution risks for prompt-generation
- handoff notes for reference-planning, sound-design, and prompt-generation

## Hard Gates

- Preserve locked dialogue, scene outcome, and continuity facts.
- Do not invent major story beats to make coverage easier.
- If input is incomplete, request clarification instead of guessing.

## Collaboration

Shot-generation should leave clear notes for:
- `reference-planning` about where supporting assets are needed
- `sound-design` about dialogue-sensitive or cue-driven moments
- `prompt-generation` about which shots are likely single-prompt, stitched multi-prompt, or timestamped multi-beat candidates
