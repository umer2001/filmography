# Prompt-Generation Input Contract

## Purpose
This contract defines how `prompt-generation` should translate approved scene planning into Veo-aware prompt sheets.

## Required Inputs
- Scene package
- Shot plan
- Reference plan
- Sound design plan

## Execution Modes

### 1. Single-Prompt Shot
Use when one prompt can cleanly cover the intended editorial shot inside Veo's time limits.

### 2. Stitched Multi-Prompt Shot
Use when one editorial shot is too long or too complex for a single generation, but the result must still read as one seamless uninterrupted shot.

For stitched shots, specify:
- segment boundary
- entry and exit frame intent
- carry-over continuity
- motion bridge
- stitch notes

### 3. Timestamped Multi-Beat Sequence
Use when a short timed sequence with multiple internal beats is better expressed inside one prompt than split into separate generations.

## What Is Locked
`prompt-generation` must preserve:
- story meaning
- scene outcome
- shot intent
- continuity anchors
- locked dialogue and sound cues

## Output Standard
The output should be a human-readable prompt sheet that clearly shows:
- which execution mode each shot uses
- which prompt style family each shot uses
- why that mode was chosen
- why that prompt style was chosen
- the base prompt text
- audio guidance
- negative constraints
- continuity notes
- retry variants

## Forbidden Moves
`prompt-generation` must not:
- invent new story beats
- change the emotional destination of the scene
- ignore mandatory references or locked dialogue

## Decision Rule
When there is tension between visual flair and continuity reliability, continuity reliability wins.

## Veo Prompt Formula

Every base prompt should cover:
- shot composition
- subject details
- action
- setting / environment
- aesthetics / mood
- audio

Use 100-150 words as a useful target for full descriptive prompts when the shot is complex. Shorter prompts are acceptable for simple inserts, reaction shots, or retry variants.

## Prompt Style Selection Rule

Prompt-generation must select a prompt style family from the shot's use case:
- `cinematic-atmospheric`
- `character-dialogue`
- `professional-business`
- `product-showcase`
- `culinary-food`
- `landscape-environment`
- `stylized-creative`
- `sci-fi-fantasy`
- `action-dynamic`
- `real-estate-architecture`
- `transformation-timelapse`
- `performance-artistic`
- `social-viral`

If shot-generation already assigned a style, preserve it unless the reference plan or sound design plan reveals a better fit. If changing the style, state the reason in the prompt sheet.

## Prompt Quality Gate

Before final output, each prompt should show:
- explicit camera/framing/movement
- continuity-safe subject or object identity
- visible action
- stable setting/environment
- bounded aesthetics/mood
- explicit audio
- mandatory references
- negative constraints
- stitch or timestamp notes when needed
