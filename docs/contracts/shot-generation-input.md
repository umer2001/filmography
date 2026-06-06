# Shot-Generation Input Contract

## Purpose
This contract defines how `shot-generation` must interpret a `Scene Package`.

## Required Input
`shot-generation` requires these sections from the scene package:
- Scene Identity
- Scene Purpose
- Story Context
- Scene Summary
- Emotional Arc
- Characters In Scene
- Setting And World Context
- Action Beats
- Dialogue
- Story Continuity Requirements
- Visual Story Priorities
- Non-Negotiables
- Creative Freedom For Shot Generation
- Output Request To Shot Generation

## What Is Locked
`shot-generation` must preserve:
- Story meaning
- Scene outcome
- Locked dialogue
- Character objectives
- Required emotional turns
- Story continuity facts
- Required props, actions, and reveals marked as essential
- Any item listed in `Non-Negotiables`

## What Is Flexible
`shot-generation` may interpret:
- Coverage design
- Framing
- Shot size
- Lens feel
- Camera movement
- Blocking emphasis
- Visual rhythm
- Whether a moment is shown directly or implied, unless marked must-show
- Beat expansion/compression, only if story meaning is preserved

## Forbidden Changes
`shot-generation` must not:
- Rewrite story events
- Change the emotional destination of the scene
- Invent new characters unless explicitly allowed
- Remove required story information
- Contradict continuity notes
- Change locked dialogue
- Introduce visual choices that undermine stated tone or scene purpose

## Expected Output
`shot-generation` should output:
- Scene coverage strategy
- Emotional coverage approach
- Continuity-aware shot list
- Identification of must-cover beats
- Identification of optional coverage
- Notes for handoff to `reference-planning`
- Notes for handoff to `sound-design`
- Notes for handoff to `prompt-generation`

## Output Quality Standard
The resulting shot plan should make it clear:
- What the scene is trying to make the audience feel
- Which beats must be visually explicit
- How continuity is maintained across shots
- Where the shot design has creative freedom
- What later skills need in order to continue the workflow

## Escalation Rule
If the scene package is missing key information, `shot-generation` should not invent major story facts. It should flag the gap clearly and request clarification.

## Interpretation Rule
When there is tension between cinematic elegance and story fidelity, story fidelity wins.

## Handoff Rule
`shot-generation` should produce outputs that are readable by:
- `reference-planning`
- `sound-design`
- `prompt-generation`

This means it should clearly label:
- continuity anchors
- visual priorities
- beat boundaries
- dialogue-sensitive moments
- intended transitions
- moments likely to require stitched multi-prompt execution later
