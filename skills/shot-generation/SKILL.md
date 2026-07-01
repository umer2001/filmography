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
- director dramatic priorities when available
- continuity anchors
- scene and shot use-case classification for prompt style selection
- shot-by-shot coverage
- likely execution risks for prompt-generation
- handoff notes for reference-planning, sound-design, and prompt-generation

## Hard Gates

- Preserve locked dialogue, scene outcome, and continuity facts.
- Do not invent major story beats to make coverage easier.
- If input is incomplete, request clarification instead of guessing.

## Collaboration

Shot-generation should leave clear notes for:
- `director` about unresolved dramatic emphasis or story-meaning questions
- `cinematographer` about framing, movement, lens feel, lighting, and continuity-sensitive visual choices
- `reference-planning` about where supporting assets are needed
- `sound-design` about dialogue-sensitive or cue-driven moments
- `prompt-generation` about which shots are likely single-prompt, stitched multi-prompt, or timestamped multi-beat candidates

## Prompt Style Intelligence

Shot-generation should classify the scene and each shot by its practical generation use case so downstream prompt-generation can choose an effective Veo prompt style instead of using one generic cinematic voice.

Use these prompt style families when they apply:
- `cinematic-atmospheric`: emotional realism, mood, intimacy, suspense, melancholy, establishing atmosphere
- `character-dialogue`: speaking characters, performance beats, subtext, reaction timing, locked dialogue
- `professional-business`: workplace, training, explainer, corporate, instructional content
- `product-showcase`: e-commerce, object reveal, rotating product, feature montage, assembly or demo
- `culinary-food`: cooking, food prep, cafe, restaurant, tactile food detail
- `landscape-environment`: travel, nature, city, weather, aerial, environment-led b-roll
- `stylized-creative`: anime, period, surreal, vintage, graphic, art-directed looks
- `sci-fi-fantasy`: speculative worlds, magical environments, futuristic or otherworldly settings
- `action-dynamic`: sports, chase, rally, handheld energy, fast physical movement
- `real-estate-architecture`: property walkthroughs, interiors, architecture, spatial flow
- `transformation-timelapse`: before/after, process, cleanup, construction, growth, time compression
- `performance-artistic`: dance, music, stage, artistic preparation, expressive body movement
- `social-viral`: selfie, vlog, punchy direct-to-camera, relatable short-form content

For each shot, identify:
- primary prompt style family
- secondary style family, if useful
- why the style fits the shot's purpose
- prompt formula emphasis: camera, subject, action, setting, aesthetics, audio, timing, references

When a scene is dramatic fiction, do not default every shot to `cinematic-atmospheric`. Use `character-dialogue` for dialogue and reaction beats, `product-showcase` for story-critical object inserts, `landscape-environment` for establishing shots, or `transformation-timelapse` when the shot depends on visible change over time.
