# Sound-Design Input Contract

## Purpose
This contract defines how `sound-design` should interpret a scene package and shot plan before prompt generation.

## Required Inputs
- Scene package
- Shot plan

## What Is Locked
`sound-design` must preserve:
- locked dialogue
- emotional arc
- story-critical sound cues named in the scene package
- continuity-sensitive sounds already established upstream

## What Sound-Design Decides
`sound-design` may decide:
- ambience strategy
- sonic emphasis per beat or shot
- which cues need precise timing
- which lines should dominate the mix versus sit inside the environment
- how prompt style family changes the audio emphasis for each shot

## Forbidden Moves
`sound-design` must not:
- rewrite dialogue
- change the scene outcome through audio interpretation
- introduce sonic ideas that undermine the approved tone

## Expected Output
The output should make prompt-generation's job easier by clearly labeling:
- locked versus flexible audio needs
- dialogue-sensitive beats
- ambience bed
- cue timing risks
- style-specific audio guidance
- whether prompts should request no subtitles

## Style-Aware Audio Rule

Use the shot plan's prompt style family to decide what audio details must appear in prompts. Dialogue styles require exact lines, pauses, and clean speaker intent; atmospheric styles require ambience and restraint; product, food, action, transformation, and performance styles require tactile or timed cues; professional and social styles require speech clarity and low-noise directness.
