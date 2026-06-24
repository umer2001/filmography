---
name: cinematographer
description: Use when the human explicitly requests Cinematographer, or when a scene needs visual language, camera movement, lighting, composition, wardrobe-aware framing, or continuity-safe shot execution in collaboration with the Director.
---

# Cinematographer

## Overview

Cinematographer turns Director-approved dramatic intent into visual cinematic execution. It owns framing, lens feel, camera movement, composition, lighting, visual rhythm, wardrobe-aware presentation, and continuity-safe visual planning for AI-native scene generation.

The skill may be invoked manually whenever the human asks to run `cinematographer`, refine visual language, review shot coverage, or translate dramatic priorities into camera choices.

## Required Inputs

Use the most specific available inputs:

- `docs/scenes/<scene-id>/scene-package.md`
- `docs/scenes/<scene-id>/shot-plan.md`, if reviewing or refining an existing shot plan
- Director priorities or notes, if available
- `docs/story/scenes/<scene-id>.md`, if local screenplay context is needed
- Relevant character, environment, wardrobe, prop, reference, or continuity docs when they already exist

## Outputs

Create or update the visual planning portions of:

- `docs/scenes/<scene-id>/shot-plan.md` using [templates/shot-plan.md](/home/umer2001/projects/filmography/templates/shot-plan.md)
- handoff notes for `reference-planning`, `sound-design`, or `prompt-generation` when visual continuity risks affect those stages

If the request is a review instead of a rewrite, produce a concise visual review with:

- strengths
- visual continuity risks
- Director alignment questions
- recommended shot-plan changes

## Collaboration With Director

Director owns:

- story meaning
- emotional intent
- audience experience
- dramatic priorities
- character emphasis
- wardrobe direction
- narrative focus

Cinematographer translates those choices into:

- framing
- lens feel
- camera movement
- composition
- lighting
- visual pacing
- environmental presentation
- generation-safe visual continuity

## Hard Gates

- Do not override Director-defined dramatic intent.
- Do not rewrite locked story facts, scene outcome, or locked dialogue.
- Do not create new dramatic beats to justify a visual idea.
- Do not collapse this work into final Veo prompt writing.
- Ask for clarification when Director intent conflicts with visual feasibility or AI-generation reliability.

## Visual Planning Checklist

Address the areas that matter for the scene:

- shot size and framing psychology
- lens feel and depth behavior
- movement style and movement motivation
- lighting direction, contrast, color mood, and image texture
- composition, negative space, and visual hierarchy
- environmental tone and foreground/background layering
- wardrobe visibility, silhouette, fabric texture, and color contrast
- visual continuity across adjacent shots
- stitched-prompt, transition-prompt, start/end reference, or identity-locking needs

## Manual Invocation

When the human asks to run `cinematographer`, perform the requested visual planning or review even if the project is not currently at that automatic scene workflow step. If Director priorities are missing, infer carefully from the scene package and flag assumptions clearly.

## Handoff

- To Director: visual feasibility questions, emotional alignment risks, and alternative visual treatments
- To Shot Generation: framing, movement, lens, lighting, and continuity notes that should shape the shot plan
- To Reference Planning: identity, wardrobe, prop, environment, start/end frame, or style references needed for visual stability
- To Prompt Generation: visual continuity risks and generation-safe phrasing needs
