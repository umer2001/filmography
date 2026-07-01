---
name: prompt-generation
description: Use when a scene package, shot plan, reference plan, and sound design plan are ready and the scene needs Veo-aware prompt sheets with continuity-preserving execution choices.
---

# Prompt Generation

## Overview

Prompt-generation turns approved scene planning into human-readable Veo prompt sheets. It is explicitly Veo-aware and should optimize for multi-shot narrative continuity within one scene.

## Required Inputs

- A scene package
- A shot plan
- A reference plan
- A sound design plan
- The rules in [docs/contracts/prompt-generation-input.md](/home/umer2001/projects/filmography/docs/contracts/prompt-generation-input.md)
- The distilled Veo rules in [docs/references/veo-prompting-principles.md](/home/umer2001/projects/filmography/docs/references/veo-prompting-principles.md), if available

## Output

Create `veo-prompt-sheet.md` using [templates/veo-prompt-sheet.md](/home/umer2001/projects/filmography/templates/veo-prompt-sheet.md).

Each shot should be classified as:
- `single-prompt shot`
- `stitched multi-prompt shot`
- `timestamped multi-beat sequence`

Use a base Veo structure of:
- shot composition
- subject details
- action
- setting / environment
- aesthetics / mood
- audio

Also include:
- prompt style family
- audio guidance
- negative constraints
- continuity anchors
- retry variants

## Hard Gates

- Do not write prompts before visual and sonic handoffs are ready.
- Prefer story continuity over flashy phrasing.
- If a shot is meant to read as one seamless editorial shot, specify stitch notes between prompt segments.

## Veo Prompt Formula

Every base prompt should be built from this sequence unless the shot has a strong reason to deviate:

`[Shot Composition] + [Subject Details] + [Action] + [Setting/Environment] + [Aesthetics/Mood] + [Audio]`

For each prompt, make sure:
- shot composition includes camera angle, framing, motion, and shot size
- subject details identify the character, object, product, food, environment, or performer with continuity-safe descriptors
- action states the visible behavior or transformation clearly
- setting/environment names the location, time, weather, spatial markers, or world rules
- aesthetics/mood defines lighting, palette, lens feel, realism/stylization level, and emotional tone
- audio includes dialogue, ambience, sound effects, music, silence, and `No subtitles` when text overlays are unwanted

Most full descriptive prompts should land around 100-150 words when the shot has enough complexity. Shorter prompts are acceptable for simple inserts, reaction beats, or tightly constrained variants.

## Prompt Style Selection

Do not use one generic prompt voice for every shot. Infer the prompt style from the shot plan, scene package, reference plan, sound design plan, and the shot's real use case.

Available prompt style families:
- `cinematic-atmospheric`: mood-forward cinematic scenes, emotional b-roll, suspense, loneliness, intimacy, weather, reflective shots
- `character-dialogue`: speaking characters, reaction beats, subtext, direct performance, locked dialogue
- `professional-business`: corporate, educational, technical, instructional, workplace, explainer
- `product-showcase`: e-commerce, product reveal, feature demo, object montage, assembly
- `culinary-food`: food prep, cafe, restaurant, cooking, tactile food texture
- `landscape-environment`: travel, city, nature, weather, aerial, environment-led establishing shots
- `stylized-creative`: anime, vintage, surreal, period, graphic, art-directed or non-naturalistic looks
- `sci-fi-fantasy`: alien worlds, futuristic spaces, fantasy environments, magical or speculative content
- `action-dynamic`: racing, sports, handheld energy, physical conflict, chase, impact, fast movement
- `real-estate-architecture`: property tours, interiors, architectural walkthroughs, spatial reveals
- `transformation-timelapse`: process, before/after, cleanup, construction, growth, time-lapse
- `performance-artistic`: dance, music, stage, rehearsal, expressive body or artistic preparation
- `social-viral`: selfie, vlog, direct-to-camera, casual apartment/phone realism, punchy short-form speech

Selection rules:
- Start with the shot's editorial purpose and visible action, not the genre label of the whole project.
- Let object-heavy inserts use `product-showcase` even inside dramatic fiction.
- Let dialogue and reaction beats use `character-dialogue` even inside visually atmospheric scenes.
- Let establishing or weather-led shots use `landscape-environment`.
- Let a scene-wide visual style become the secondary style when needed.
- When two styles apply, name a primary and secondary style and explain the choice briefly.

## Style-Specific Prompt Emphasis

Emphasize different formula parts by style:
- `cinematic-atmospheric`: composition, environment, lighting, mood, ambience, restrained movement
- `character-dialogue`: subject identity, performance, eyeline, pauses, locked lines, room tone, no subtitles
- `professional-business`: clarity, task action, clean setting, readable process, voiceover or practical sound
- `product-showcase`: object details, surface/material, camera orbit or montage beats, tactile/mechanical audio
- `culinary-food`: hand/tool action, texture, steam, close-up composition, kitchen/cafe ambience
- `landscape-environment`: scale, camera path, weather/time change, natural sound, atmosphere
- `stylized-creative`: style rules, palette, period/design details, music or texture that reinforces the look
- `sci-fi-fantasy`: world rules, unusual environment details, coherent sound world, avoid generic fantasy blur
- `action-dynamic`: physical geography, motion direction, impact timing, kinetic camera, intense but readable audio
- `real-estate-architecture`: route through space, stable layout, daylight/interior lighting, footsteps/soft music
- `transformation-timelapse`: before/after state, fixed camera or split screen, beat timing, satisfying process sounds
- `performance-artistic`: body movement, emotional preparation, stage/light state, music cue timing, breath
- `social-viral`: direct gaze, phone/selfie framing, casual authenticity, concise spoken line, no subtitles

## Prompt Quality Gate

Before finalizing each prompt, check:
- camera/framing/movement are explicit
- subject identity or object identity is anchored
- action is visible and specific
- setting/environment is stable
- aesthetics/mood are bounded, not vague
- audio is explicit and aligned with the sound design plan
- references are named where mandatory
- negative constraints prevent the most likely drift
- stitched shots include entry/exit frames, motion bridge, and carry-over continuity
- timestamped sequences include beat timing for action, dialogue, and sound cues
