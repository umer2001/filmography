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
