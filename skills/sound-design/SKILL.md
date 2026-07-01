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
- audio strategy by prompt style family
- notes that prompt-generation must carry into Veo prompts

## Hard Gates

- Do not rewrite locked dialogue.
- Keep sound choices in service of the scene's emotional arc.
- Flag any cue or dialogue requirement that depends on exact shot timing.

## Prompt Style Audio Rules

Use the shot plan's prompt style classification to shape audio handoff:
- `character-dialogue`: preserve exact locked lines, speaker order, pauses, breath, room tone, and whether subtitles should be excluded
- `cinematic-atmospheric`: define ambience, silence, music restraint, environmental texture, and emotional sound bed
- `product-showcase`: define tactile product sounds, mechanical clicks, soft swells, and whether voiceover or dialogue is needed
- `professional-business`: define clean voiceover, low-distraction room tone, interface or task sounds, and instructional pacing
- `culinary-food`: define knife, sizzling, pour, steam, cafe, or kitchen ambience with tactile detail
- `landscape-environment`: define weather, wildlife, traffic, water, wind, or distant human texture without over-scoring
- `stylized-creative` or `sci-fi-fantasy`: define sound-world rules and recurring motifs that keep the world coherent
- `action-dynamic`: define engine, impact, breath, movement, crowd, radio chatter, or handheld documentary sound as needed
- `real-estate-architecture`: define footsteps, room tone, doors, soft music, and calm pacing
- `transformation-timelapse`: define satisfying process sounds, rhythmic cues, or music beat alignment
- `performance-artistic`: define breath, music entry, audience/space tone, and exact cue timing
- `social-viral`: define direct-to-camera speech clarity, casual room ambience, phone/selfie realism, and `No subtitles` if text overlays are unwanted

For every shot, label audio as `locked`, `recommended`, or `optional` so prompt-generation knows what must appear verbatim in the Veo prompt.
