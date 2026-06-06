---
name: reference-planning
description: Use when an approved shot plan exists and a scene needs consistent character, style, prop, or start-end references before Veo-aware prompt writing.
---

# Reference Planning

## Overview

Reference-planning decides which supporting visual assets should exist before prompt-generation. It does not write final Veo prompts. It reduces continuity drift by identifying what later stages should reuse.

## Required Inputs

- A scene package
- A shot plan
- The rules in [docs/contracts/reference-planning-input.md](/home/umer2001/projects/filmography/docs/contracts/reference-planning-input.md)

## Output

Create `reference-plan.md` using [templates/reference-plan.md](/home/umer2001/projects/filmography/templates/reference-plan.md).

The plan should identify:
- required references versus optional references
- which shots consume each reference
- continuity anchors each reference must preserve
- whether a reference is for character, style, prop, environment, or start/end framing
- what can be reused across the whole scene

## Hard Gates

- Do not collapse this work into prompt-writing.
- Ask for missing visual identity details instead of fabricating them.
- Keep the output human-readable and scoped to one scene.
