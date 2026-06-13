# Filmography

Filmography is an AI-native film and video production workflow plugin, adapted from the structure of Superpowers. It helps agents turn story ideas into screenplay-ready project foundations and then into scene-ready generation materials through reusable skills, role-specific agents, and explicit handoffs between creative stages.

## What Filmography Focuses On

The current v1 structure is designed for software-based production workflows that use tools such as Google Flow, Veo, and Nano Banana. Instead of planning physical shoots, Filmography focuses on:

1. **Project-level pre-production** - Build story foundations, screenplay, project bibles, and continuity rules
2. **Screenplay review** - Audit the full screenplay before human approval
3. **Scene packaging** - Turn one approved scene into a handoff-ready scene package
4. **Shot generation** - Turn scenes into continuity-aware cinematic coverage
5. **Reference planning** - Decide what character, style, or start/end references are needed
6. **Sound design** - Define dialogue treatment, ambience, and sonic cues
7. **Prompt generation** - Create Veo-aware, human-readable prompt sheets for one scene at a time
8. **Post-production** - Guide editing, continuity repair, and final delivery

## Current V1 Workflows

Filmography now has two main workflows:

### 1. Project-Level Workflow

1. `pre-production-planning`
2. `screenwriter` develops the full story and master screenplay
3. `screenplay-reviewer` performs a blocking story-quality review
4. `screenwriter` revises if the review returns blocking issues
5. human screenplay approval gate
6. auto-generate `docs/story/scenes/<scene-id>.md`
7. propose screenplay breakdown artifacts
8. `script-breakdown-reviewer` checks coverage and priority
9. human breakdown approval
10. generate `required` derived docs first
11. optionally expand into `useful` docs
12. lock the project foundation for scene work

### 2. Scene Workflow

1. choose `docs/story/scenes/<scene-id>.md`
2. `scene-packaging` creates a short interpretation preview
3. preview approval gate
4. `scene-package.md`
5. `shot-generation`
6. `reference-planning`
7. `sound-design`
8. `prompt-generation`

The prompt-generation stage is intentionally **Veo-aware**. It can choose between:
- a single prompt for a shot
- multiple prompts stitched into one seamless editorial shot
- timestamped multi-beat prompts for short sequences

## Repo Structure

- `skills/` contains workflow skills
- `agents/` contains role-specific agent briefs
- `templates/` contains reusable human-readable documents
- `docs/contracts/` defines handoffs between workflow stages
- `docs/examples/` shows an end-to-end example scene workflow
- `help/superpowers/` is the local reference copy of the upstream framework this project is adapting

## Core V1 Skills

- `using-filmography` - Entry skill that routes work into the right workflow
- `pre-production-planning` - Create project foundations and screenplay gates before scene work
- `screenplay-reviewer` - Run a blocking screenplay quality review before human approval, or manually when requested
- `scene-packaging` - Preview and package one screenplay scene for downstream planning
- `shot-generation` - Build continuity-aware shot plans from scene packages
- `reference-planning` - Decide which reference assets are required
- `sound-design` - Define sonic intent and dialogue/audio requirements
- `prompt-generation` - Write Veo-aware prompt sheets from approved scene inputs
- `script-breakdown-reviewer` - Review screenplay-derived doc proposals for coverage and priority
- `writing-skills` - Create or refine Filmography skills with explicit handoffs

## Agents

- `screenwriter` - Produces story-ready screenplay artifacts
- `screenplay-reviewer` - Audits full screenplays for structure, hook, retention, visual storytelling, and emotional pacing
- `director` - Owns scene interpretation and dramatic clarity
- `cinematographer` - Owns framing, movement, and visual continuity
- `producer` - Keeps the workflow scoped, coordinated, and handoff-safe
- `script-breakdown-reviewer` - Checks screenplay-derived doc coverage and priority
- `post-production-lead` - Oversees editing, continuity repair, and final finishing

## Templates And Contracts

Important handoff artifacts in this repo include:

- `templates/screenplay.md`
- `templates/screenplay-review-report.md`
- `templates/story-scene.md`
- `templates/scene-interpretation-preview.md`
- `templates/scene-package.md`
- `templates/shot-plan.md`
- `templates/reference-plan.md`
- `templates/sound-design-plan.md`
- `templates/veo-prompt-sheet.md`
- `templates/extraction-proposal.md`
- `templates/project-continuity-anchors.md`
- `templates/character-profile.md`
- `templates/character-continuity.md`
- `templates/environment-description.md`
- `templates/environment-continuity.md`
- `docs/contracts/shot-generation-input.md`
- `docs/contracts/reference-planning-input.md`
- `docs/contracts/sound-design-input.md`
- `docs/contracts/prompt-generation-input.md`

Example screenplay-review output:

- `docs/examples/example-screenplay-review-report.md`

## Installation

### Claude Code

```bash
/plugin install filmography@umer2001/filmography
```

### Cursor

```bash
/add-plugin filmography
```

### Other Harnesses

Register the marketplace and install:

```bash
plugin marketplace add umer2001/filmography
plugin install filmography@filmography-marketplace
```

## Basic Workflow

### Project-Level

1. **Concept intake and clarification** - Start from narration, story concept, synopsis, tone, or references
2. **Story foundation** - Build the logline, premise, synopsis, and early project foundation
3. **Full screenplay** - Write the entire screenplay as a required gate before scene workflow
4. **Screenplay review** - Run `screenplay-reviewer` as a blocking story-quality gate before human approval
5. **Screenwriter revisions** - Resolve blocking review notes and re-review when needed
6. **Screenplay approval** - Lock the story before downstream doc generation
7. **Per-scene screenplay files** - Auto-generate `docs/story/scenes/<scene-id>.md`
8. **Breakdown proposal and review** - Propose characters, environments, important props, relationships, factions, and motifs; review for coverage and doc priority
9. **Derived docs generation** - Create `required` docs first, then optionally expand into `useful` docs
10. **Locked project foundation** - Finalize continuity anchors and downstream project docs

### Scene-Level

1. **Scene selection** - Pick an approved per-scene screenplay file
2. **Scene interpretation preview** - Preview the intended downstream emphasis before package creation
3. **Scene packaging** - Create the approved `scene-package.md`
4. **Shot generation**
5. **Reference planning**
6. **Sound design**
7. **Prompt generation**

## Philosophy

- **Systematic over ad-hoc** - Process over guessing
- **Collaboration over siloing** - Clear communication between departments
- **Specification before execution** - Planning before generation
- **Evidence over claims** - Review and verify before approving
- **Incremental validation** - Get approval after each phase

## The Production Agents

### Screenwriter
Focuses on story structure, character development, dialogue, and narrative pacing. Produces the full screenplay and the story artifacts that scene-level workflows inherit.

### Screenplay Reviewer
Audits the full screenplay before human approval. It checks transformation, structure, hook strategy, retention loops, visual storytelling, and emotional pacing, then returns actionable directives to the Screenwriter. It can also be invoked manually when a human wants an additional screenplay review pass.

### Director
Coordinates the overall creative vision for a scene. Plans dramatic coverage, performance emphasis, and scene flow while protecting story intent.

### Cinematographer
Plans camera movement, composition, visual language, and lighting feel. Works with the Director to turn scene intent into usable shot design.

### Producer
Coordinates the workflow, scope, handoffs, and approval flow across both project-level and scene-level departments in an AI-native production pipeline.

### Post-Production Lead
Oversees editing, color grading, sound design, and final delivery. Ensures post-production work aligns with the original creative vision.

## Status

This repository now contains the v1 workflow structure, templates, contracts, and worked examples for both project-level and scene-level workflows. It is still early-stage and should be treated as a framework under active validation rather than a fully battle-tested plugin.

## Contributing

Contributions are welcome! Please follow these guidelines:

1. Fork the repository
2. Create a branch for your work
3. Follow the `writing-skills` skill for creating production skills
4. Submit a pull request with a clear description

See `CLAUDE.md` for detailed contributor guidelines.

## License

MIT License - see LICENSE file for details

## Community

Filmography is built for creative professionals using AI agents to coordinate complex productions.

- **GitHub Issues**: https://github.com/umer2001/filmography/issues
- **Discussions**: https://github.com/umer2001/filmography/discussions
- **Documentation**: https://github.com/umer2001/filmography
