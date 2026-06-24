# Filmography V1 Structure Design

## Goal

Create a usable v1 structure for Filmography as an AI-native film and video production plugin adapted from the workflow discipline of Superpowers.

## Scope

Filmography v1 focuses on a single end-to-end scene workflow rather than a full production stack. The plugin should help an agent move from project planning to a structured scene package, then through shot planning, reference planning, sound design, and Veo-aware prompt generation.

## Workflow

1. `pre-production-planning`
2. `screenwriter` produces a `scene-package.md`
3. `shot-generation`
4. `reference-planning`
5. `sound-design`
6. `prompt-generation`

## Core Decisions

- The plugin is AI-native and software-based, not physical-shoot logistics oriented.
- Work happens one scene at a time in v1.
- `shot-generation` and `prompt-generation` are separate skills.
- The Director and Cinematographer collaborate during scene interpretation and shot planning: Director owns dramatic intent, performance, wardrobe, staging, and audience experience; Cinematographer owns visual execution.
- `reference-planning` and `sound-design` are separate collaborating skills.
- `prompt-generation` is explicitly Veo-aware.
- Veo prompt output is primarily human-readable prompt sheets, not machine-first JSON.
- Prompt-generation must decide between:
  - single-prompt shots
  - stitched multi-prompt shots
  - timestamped multi-beat sequences

## Artifacts

V1 should include:
- core workflow skills
- role agents for the scene workflow
- reusable templates
- explicit handoff contracts
- one worked example scene
- updated README and plugin manifests aligned with the actual workflow

## Acceptance Criteria

- The repo contains a real `skills/` directory referenced by the manifest.
- The manifest does not point at missing required files.
- The README accurately describes the AI-native scene workflow.
- A scene can move conceptually from screenwriter handoff to Veo prompt sheet using repo artifacts alone.
- Each stage has a readable template or contract.
