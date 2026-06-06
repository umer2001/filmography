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

## Output

Create `veo-prompt-sheet.md` using [templates/veo-prompt-sheet.md](/home/umer2001/projects/filmography/templates/veo-prompt-sheet.md).

Each shot should be classified as:
- `single-prompt shot`
- `stitched multi-prompt shot`
- `timestamped multi-beat sequence`

Use a base Veo structure of:
- cinematography
- subject
- action
- context
- style and ambiance

Also include:
- audio guidance
- negative constraints
- continuity anchors
- retry variants

## Hard Gates

- Do not write prompts before visual and sonic handoffs are ready.
- Prefer story continuity over flashy phrasing.
- If a shot is meant to read as one seamless editorial shot, specify stitch notes between prompt segments.
