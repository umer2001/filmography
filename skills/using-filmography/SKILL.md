---
name: using-filmography
description: Use when starting a film or video production conversation, or when an agent needs to route work into the correct Filmography workflow before planning shots, references, sound, or prompts.
---

# Using Filmography

## Overview

Filmography is a workflow plugin for AI-native film and video production. It helps agents move from story to generation through explicit creative handoffs instead of jumping straight to prompts.

## Routing Rules

- If the project foundation or screenplay does not exist, use `pre-production-planning`.
- If the human explicitly asks for story development, screenplay drafting, screenplay revision, or `screenwriter`, use `screenwriter`.
- If the full screenplay exists but has not passed review, use `screenplay-reviewer` before human screenplay approval.
- If the human explicitly asks for screenplay review, use `screenplay-reviewer` even outside the automatic approval flow.
- If the screenplay exists but per-scene files do not, derive `docs/story/scenes/<scene-id>.md` before any scene workflow.
- If screenplay-derived project docs are being proposed, use `script-breakdown-reviewer` before generating them.
- If a scene exists but is not packaged for downstream work, use `scene-packaging`.
- If a scene package exists, use `shot-generation` before reference, sound, or prompt work.
- Use `reference-planning` and `sound-design` after shot-generation.
- Use `prompt-generation` last, after visual and sonic handoffs are ready.

## Hard Gates

- Work one scene at a time for v1.
- Do not begin scene workflow until the full screenplay exists, has passed screenplay-reviewer, and is approved by the human.
- Do not send the screenplay to human approval before screenplay-reviewer has produced a verdict, unless the human explicitly overrides the gate.
- Do not generate derived project docs from the screenplay without a reviewed extraction proposal.
- Do not create `scene-package.md` until a scene interpretation preview has been approved.
- Do not skip directly to prompt-generation without a scene package and shot plan.
- Do not let downstream skills rewrite locked story facts, scene outcome, or locked dialogue.

## Preferred Artifact Paths

- Project foundation: `docs/project/project-foundation.md`
- Story foundation: `docs/story/foundation.md`
- Master screenplay: `docs/story/screenplay.md`
- Screenplay review report: `docs/story/screenplay-review-report.md`
- Per-scene screenplay: `docs/story/scenes/<scene-id>.md`
- Project continuity: `docs/continuity/anchors.md`
- Character docs: `docs/characters/<character-slug>/profile.md`
- Environment docs: `docs/environments/<environment-slug>/description.md`
- Scene interpretation preview: `docs/scenes/<scene-id>/scene-interpretation-preview.md`
- Scene package: `docs/scenes/<scene-id>/scene-package.md`
- Shot plan: `docs/scenes/<scene-id>/shot-plan.md`
- Reference plan: `docs/scenes/<scene-id>/reference-plan.md`
- Sound design plan: `docs/scenes/<scene-id>/sound-design-plan.md`
- Veo prompt sheet: `docs/scenes/<scene-id>/veo-prompt-sheet.md`

## Core Principle

Story fidelity comes first. Every downstream document should make the next step easier without forcing that step to rediscover the scene from scratch.
