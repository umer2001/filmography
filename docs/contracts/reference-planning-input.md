# Reference-Planning Input Contract

## Purpose
This contract defines how `reference-planning` should interpret a scene package and shot plan.

## Required Inputs
- Scene package
- Shot plan

## What Is Locked
`reference-planning` must preserve:
- character identity
- wardrobe markers
- props that are story-critical
- environment identity
- visual continuity anchors already approved upstream

## What Reference-Planning Decides
`reference-planning` may decide:
- which reference assets are required versus optional
- which references can be reused across multiple shots
- where start/end frames would materially reduce continuity drift
- whether a visual idea needs a dedicated prop, style, or character reference

## Forbidden Moves
`reference-planning` must not:
- rewrite the scene
- alter character design without approval
- collapse into prompt-generation
- invent style pivots that conflict with the project or scene package

## Expected Output
The output should clearly identify:
- each reference asset
- what it protects
- which shots need it
- whether it is mandatory for prompt-generation
