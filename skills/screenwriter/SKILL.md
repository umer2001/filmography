---
name: screenwriter
description: Use when the human explicitly requests Screenwriter, or when a project needs story development, screenplay drafting, screenplay revision, or screenplay-derived scene files.
---

# Screenwriter

## Overview

Screenwriter develops and revises story materials for the project-level workflow. It owns story structure, character development, dialogue, narrative pacing, and the master screenplay that downstream scene work inherits.

The skill may be invoked manually whenever the human asks to run `screenwriter`, draft a screenplay, revise a screenplay, or produce screenplay-derived scene files.

## Required Inputs

Use the most specific available inputs:

- Human story concept, synopsis, narration, notes, or revision request
- `docs/story/foundation.md`, if available
- `docs/project/project-foundation.md`, if available
- `docs/story/screenplay.md`, if revising an existing screenplay
- `docs/story/screenplay-review-report.md`, if responding to reviewer notes
- Relevant character, environment, continuity, relationship, faction, motif, or prop docs when they already exist

## Outputs

Create or update whichever artifacts the request calls for:

- `docs/story/foundation.md` using [templates/story-foundation.md](/home/umer2001/projects/filmography/templates/story-foundation.md)
- `docs/story/screenplay.md` using [templates/screenplay.md](/home/umer2001/projects/filmography/templates/screenplay.md)
- `docs/story/scenes/<scene-id>.md` using [templates/story-scene.md](/home/umer2001/projects/filmography/templates/story-scene.md), after screenplay approval

## Workflow Use

- During project-level workflow, Screenwriter develops the full screenplay before `screenplay-reviewer`.
- If `screenplay-reviewer` returns `No` or `With revisions`, Screenwriter revises the screenplay against the review report.
- After the screenplay passes review and receives human approval, Screenwriter may derive per-scene screenplay files from the approved master screenplay.

## Manual Invocation

When the human asks to run `screenwriter`, perform the requested Screenwriter work even if the project is not currently at that automatic workflow step. If required upstream context is missing, ask for the smallest clarification needed or clearly mark assumptions before drafting.

## Hard Gates

- Do not create scene packages, shot plans, reference plans, sound design plans, or Veo prompt sheets.
- Do not treat a draft screenplay as approved just because Screenwriter created it.
- Do not bypass `screenplay-reviewer` before human screenplay approval.
- Do not generate per-scene screenplay files until the master screenplay has passed review and human approval.
- Preserve locked project foundation and continuity facts unless the human explicitly asks to revise them.

## Handoff

- To Screenplay Reviewer: full screenplay draft and any revision notes that explain intentional choices
- To Human: readable story or screenplay artifacts ready for review
- To Scene Packaging: approved per-scene screenplay files only after review and human approval gates
