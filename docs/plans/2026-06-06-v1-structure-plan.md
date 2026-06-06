# Filmography V1 Structure Implementation Plan

> **For agentic workers:** Implement this plan by creating the scene-workflow structure, reusable artifacts, and example documents in small verifiable batches.

**Goal:** Build Filmography's initial end-to-end scene workflow structure.

**Architecture:** Add the core workflow skills, role agents, handoff contracts, reusable templates, and one worked example scene. Update the public repo description so the manifests and README match the files that actually exist.

**Tech Stack:** Markdown, plugin manifests, zero-dependency documentation workflow

---

## Task 1: Align the repo spine

**Files:**
- Modify: `README.md`
- Modify: `.codex-plugin/plugin.json`
- Modify: `.claude-plugin/plugin.json`
- Modify: `agents/screenwriter.md`
- Create: `agents/director.md`
- Create: `agents/cinematographer.md`
- Create: `agents/producer.md`

**Done when:**
- Public docs describe the AI-native scene workflow
- Manifests reference a real `skills/` directory
- Core scene agents exist

## Task 2: Add workflow skills

**Files:**
- Create: `skills/using-filmography/SKILL.md`
- Create: `skills/pre-production-planning/SKILL.md`
- Create: `skills/shot-generation/SKILL.md`
- Create: `skills/reference-planning/SKILL.md`
- Create: `skills/sound-design/SKILL.md`
- Create: `skills/prompt-generation/SKILL.md`

**Done when:**
- Each skill has valid frontmatter
- Each skill states when it should be used
- Each skill defines required inputs, outputs, and hard gates

## Task 3: Add reusable templates and contracts

**Files:**
- Create: `templates/project-foundation.md`
- Create: `templates/shot-plan.md`
- Create: `templates/reference-plan.md`
- Create: `templates/sound-design-plan.md`
- Create: `templates/veo-prompt-sheet.md`
- Create: `docs/contracts/reference-planning-input.md`
- Create: `docs/contracts/sound-design-input.md`
- Create: `docs/contracts/prompt-generation-input.md`

**Done when:**
- Every scene workflow stage has a template or contract
- Handoffs are explicit and human-readable

## Task 4: Add a worked example scene

**Files:**
- Create: `docs/examples/example-scene-package.md`
- Create: `docs/examples/example-shot-plan.md`
- Create: `docs/examples/example-reference-plan.md`
- Create: `docs/examples/example-sound-design-plan.md`
- Create: `docs/examples/example-veo-prompt-sheet.md`

**Done when:**
- The same scene flows through every stage
- The example demonstrates continuity-aware prompt decisions

## Task 5: Save design and implementation records

**Files:**
- Create: `docs/specs/2026-06-06-v1-structure-design.md`
- Create: `docs/plans/2026-06-06-v1-structure-plan.md`

**Done when:**
- The repo contains a durable record of the approved v1 structure
