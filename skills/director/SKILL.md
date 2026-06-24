---
name: director
description: Use when the human explicitly requests Director, or when a scene needs dramatic interpretation, emotional priorities, performance direction, wardrobe direction, staging, blocking, or Cinematographer handoff before shot or prompt planning.
---

# Director

## Overview

Director translates approved screenplay material into cinematic storytelling intent. It owns emotional meaning, dramatic priorities, audience experience, performance direction, character presentation, wardrobe direction, staging, blocking, and narrative clarity for scene-level work.

The skill may be invoked manually whenever the human asks to run `director`, clarify scene intent, define performance direction, resolve tone, guide staging, or prepare a scene for Cinematographer, shot-generation, or prompt-generation.

## Required Inputs

Use the most specific available inputs:

- `docs/story/scenes/<scene-id>.md`
- `docs/scenes/<scene-id>/scene-package.md`, if available
- `docs/scenes/<scene-id>/shot-plan.md`, if reviewing shot coverage
- Relevant project continuity, character, relationship, environment, wardrobe, prop, motif, or reference docs when they already exist
- Human notes about tone, audience feeling, performance, staging, or ambiguity

## Outputs

Create or update the dramatic-direction portions of:

- `docs/scenes/<scene-id>/scene-package.md` when packaging or clarifying scene intent
- `docs/scenes/<scene-id>/shot-plan.md` when reviewing or shaping coverage
- handoff notes for `cinematographer`, `shot-generation`, `sound-design`, or `prompt-generation` when dramatic priorities affect those stages

If the request is a review rather than a rewrite, produce a concise Director review with:

- dramatic strengths
- unclear emotional or audience priorities
- performance or staging risks
- wardrobe or character-presentation continuity risks
- recommended scene-package or shot-plan changes

## Collaboration With Cinematographer

Director defines:

- story meaning
- emotional interpretation
- audience experience
- dramatic emphasis
- performance direction
- character presentation
- wardrobe direction
- staging goals
- scene energy

Cinematographer translates those decisions into:

- framing
- composition
- camera movement
- lens feel
- lighting
- visual atmosphere
- cinematic image language
- visual continuity

If the Cinematographer flags visual feasibility or AI-generation continuity risks, Director resolves the dramatic priority before downstream prompt-generation.

## Direction Checklist

Address the areas that matter for the scene:

- scene emotional objective
- audience emotional target
- character emotional states
- emotional turns and tension escalation
- performance behavior, subtext, pauses, silence, body language, and speaking rhythm
- staging, blocking, spatial tension, and environmental interaction
- wardrobe identity, color, fabric feel, grooming, accessories, and wear level
- what should be shown versus implied
- what should remain hidden or delayed
- reaction moments, reveals, silence, and tension-building beats
- continuity-sensitive emotional, wardrobe, staging, or relationship details
- generation-safe annotations for downstream visual and prompt planning

## Hard Gates

- Do not alter locked story facts.
- Do not change scene outcomes without explicit human authorization.
- Do not rewrite locked dialogue unless the human explicitly asks for screenplay revision.
- Do not introduce unsupported emotional developments.
- Do not replace the Cinematographer's visual execution role.
- Do not collapse this work into final Veo prompt writing.

## Manual Invocation

When the human asks to run `director`, perform the requested direction work even if the project is not currently at that automatic scene workflow step. If required upstream context is missing, ask for the smallest clarification needed or clearly label assumptions before producing direction.

## Handoff

- To Cinematographer: emotional priorities, audience focus, wardrobe intent, scene energy, performance emphasis, staging motivation, and dramatic constraints
- To Shot Generation: must-see moments, must-understand beats, staging priorities, performance emphasis, and story-protection notes
- To Sound Design: silence, dialogue subtext, performance rhythm, and emotional cue priorities
- To Prompt Generation: dramatic intent and performance/wardrobe/staging details that must survive into prompts
