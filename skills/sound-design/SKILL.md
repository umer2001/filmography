---
name: sound-design
description: Use when a scene package and shot plan exist and the scene needs dialogue, ambience, and cue planning before Veo-aware prompt generation.
---

# Sound Design

## Overview

This skill defines how the scene should sound before prompts are written. It clarifies what dialogue is locked, what ambience shapes the scene, and which sonic beats need to survive into prompt-generation.

## Required Inputs

- A scene package
- A shot plan
- The rules in [docs/contracts/sound-design-input.md](/home/umer2001/projects/filmography/docs/contracts/sound-design-input.md)

## Output

Create `sound-design-plan.md` using [templates/sound-design-plan.md](/home/umer2001/projects/filmography/templates/sound-design-plan.md).

The plan should define:
- dialogue priorities
- ambience bed
- key sound cues
- sound continuity across shots
- moments that need precise timing
- notes that prompt-generation must carry into Veo prompts

## Hard Gates

- Do not rewrite locked dialogue.
- Keep sound choices in service of the scene's emotional arc.
- Flag any cue or dialogue requirement that depends on exact shot timing.
