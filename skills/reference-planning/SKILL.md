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
- which prompt style families increase the need for references

## Hard Gates

- Do not collapse this work into prompt-writing.
- Ask for missing visual identity details instead of fabricating them.
- Keep the output human-readable and scoped to one scene.

## Prompt Style Reference Rules

Use the shot plan's prompt style classification to decide which references matter most:
- `character-dialogue`: prioritize character identity, wardrobe, eyeline, facial expression range, and continuity-safe two-shot or over-the-shoulder frames
- `product-showcase`: prioritize clean prop or product references, surface details, label orientation, and close-up reference frames
- `real-estate-architecture`: prioritize environment layout, room-to-room continuity, architectural style, and start/end frames for walkthrough movement
- `landscape-environment`: prioritize approved environment/style frames, time of day, weather, palette, and camera-height references when scale matters
- `stylized-creative` or `sci-fi-fantasy`: prioritize style frames and world rules so the look stays coherent across shots
- `action-dynamic`: prioritize start/end poses, motion bridge frames, wardrobe state, vehicle/prop continuity, and spatial orientation
- `transformation-timelapse`: prioritize before/after frames and any fixed camera or layout anchor
- `culinary-food`: prioritize food state, plating, hand/tool continuity, texture, steam, and surface references
- `performance-artistic`: prioritize costume, pose language, stage/space layout, lighting state, and expression references
- `social-viral` or `professional-business`: prioritize consistent subject presentation, room identity, device/desk/product placement, and readable direct-to-camera setup

If a shot uses stitched multi-prompt execution or a timed internal transformation, explicitly evaluate whether first/last frames or bridge frames are required before prompt-generation.
