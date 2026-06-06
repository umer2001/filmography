# Filmography Project-Level Workflow Plan

**Goal:** Represent the screenplay-first project workflow in repo docs, skills, templates, and examples.

**Architecture:** Keep `screenplay.md` as the project source of truth, derive per-scene screenplay files automatically, review breakdown proposals before doc generation, and gate scene packaging behind an interpretation preview.

**Tech Stack:** Markdown, plugin manifests, zero-dependency documentation workflow

---

## Task 1: Update routing and public docs

- Update README to describe the two main workflows
- Update routing skills to enforce screenplay and scene-preview gates
- Update manifests to mention screenplay and scene-packaging flow

## Task 2: Add project-level workflow skills

- Add `scene-packaging`
- Add `script-breakdown-reviewer`
- Update `pre-production-planning`

## Task 3: Add project-level templates

- Add templates for story foundation, screenplay, per-scene screenplay files, extraction proposals, continuity anchors, character docs, and environment docs
- Update project foundation template to reflect early/locked states

## Task 4: Add example artifacts

- Add example project-level docs that lead into the existing scene workflow examples

## Task 5: Verify internal consistency

- Check manifests parse
- Check referenced skill files exist
- Check README and routing docs align on artifact paths and gates
