---
name: script-breakdown-reviewer
description: Use when a screenplay-derived extraction proposal lists characters, environments, important props, relationships, factions, or motifs and that proposal needs a coverage and priority review before files are generated.
---

# Script Breakdown Reviewer

## Overview

This skill reviews the proposed derived-doc breakdown against the approved screenplay. Its job is to catch missing coverage, trim unnecessary items, and assign doc priority before file generation begins.

## Required Inputs

- `docs/story/screenplay.md`
- proposed breakdown list using [templates/extraction-proposal.md](/home/umer2001/projects/filmography/templates/extraction-proposal.md)

## Review Scope

Check for:
- characters
- environments
- important recurring props
- relationships
- factions or groups
- recurring motifs

## Output

Review the proposal and label each item:
- `required`
- `useful`
- `optional`

Also flag:
- missing items
- unnecessary items
- items that should move between categories

## Hard Gates

- Do not approve the proposal if it misses continuity-relevant items.
- Generate only `required` docs after approval.
- Ask whether to expand into `useful` docs afterward.
