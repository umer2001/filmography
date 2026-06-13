---
name: screenplay-reviewer
description: Use when a full screenplay draft needs a blocking story-quality review before human approval, or when the human explicitly requests a screenplay review pass.
---

# Screenplay Reviewer

## Overview

Screenplay-reviewer audits the full screenplay before it reaches human approval. It is a blocking project-level quality gate that gives the Screenwriter actionable feedback without rewriting the script.

The skill may also be invoked manually whenever the human asks for a screenplay review, extra audit, or second pass.

## Required Inputs

- `docs/story/screenplay.md`
- `docs/story/foundation.md`, if available
- `docs/project/project-foundation.md`, if available
- Existing `docs/story/screenplay-review-report.md`, if this is a re-review
- Relevant continuity anchors, character notes, or environment notes when they already exist

## Output

Create or update:

- `docs/story/screenplay-review-report.md` using [templates/screenplay-review-report.md](/home/umer2001/projects/filmography/templates/screenplay-review-report.md)

The report must give a verdict:

- `Ready for human approval: Yes`
- `Ready for human approval: No`
- `Ready for human approval: With revisions`

## Review Framework

Evaluate the screenplay through these lenses:

1. **Skeleton: structural framework**
   - Does the story show a clear transformation from Point A to Point B?
   - Are identity, conflict, choice, and change all present and legible?

2. **Muscles and fat: engagement mechanics**
   - Are pacing and attention loops strong enough to keep viewers watching?
   - Does the screenplay answer why the story matters, how change manifests, and what payoff the viewer receives?

3. **Blood vessels: hook strategy**
   - Does the opening create immediate psychological interest?
   - Does it target a real emotional root or curiosity gap?
   - Is there a clear expectation, promise, or tension that pulls the viewer forward?

4. **Skin: visual perspective and metaphor**
   - Does the script show rather than explain?
   - Are important emotions, stakes, and world details made visual?
   - Are there pattern breaks that prevent autopilot viewing?

5. **Nervous system: emotional pacing**
   - Does the emotional curve vary between tension, relief, humor, seriousness, intimacy, or surprise as appropriate?
   - Is there a reason to keep watching from the start?
   - Does the journey create empathy or bonding with the central character or subject?

## Blocking Gate

- Do not send the screenplay to human approval until this review report exists.
- If the verdict is `No` or `With revisions`, route the report back to the Screenwriter for revision.
- Re-run screenplay-reviewer after revisions when the prior report contains blocking issues.
- Human approval should only happen after the reviewer verdict is `Yes`, unless the human explicitly chooses to override the gate.

## Manual Invocation

When the human asks to run `screenplay-reviewer`, perform the same review even if the project is not currently at the automatic pre-approval gate. If the screenplay is incomplete, review what exists and clearly label missing inputs or limits in the report.

## Forbidden Moves

- Do not rewrite the screenplay.
- Do not create new scenes, dialogue, plot turns, or character motivations.
- Do not approve a structurally weak screenplay just because it is complete.
- Do not replace human approval; this skill prepares the screenplay for that approval.
- Do not perform the later extraction-proposal review. Use `script-breakdown-reviewer` for screenplay-derived document coverage.

## Handoff

- To Screenwriter: revision directives, blocking issues, and focused story-quality feedback
- To Producer: approval-readiness verdict and unresolved risks
- To Human: a concise report that makes the approval decision easier
- To Script Breakdown Reviewer: only after human screenplay approval, when derived-doc coverage is being proposed
