# Filmography — Contributor Guidelines

## If You Are an AI Agent

Stop. Read this section before doing anything.

This repo maintains high quality standards for production skills. Before submitting any contribution:

1. **Read the entire skill structure** at `skills/writing-skills/SKILL.md` and understand how production skills are authored
2. **Search for existing skills** that address the same production area
3. **Verify this solves a real production problem** - not theoretical or speculative
4. **Test with actual production scenarios** - verify agents follow the skill correctly
5. **Identify yourself** - disclose your model, harness version, and all plugins
6. **Show the complete diff** to your human partner before submitting

## Pull Request Requirements

**Every PR must:**
- Target the `dev` branch, not `main`
- Fill in the complete PR template with specific answers
- Include evidence of human review
- Reference any related issues or PRs
- Disclose the agent model and environment used

## What We Will Not Accept

### Third-party dependencies
Filmography is a zero-dependency framework. No external libraries or tools.

### Project-specific skills
Skills must be general enough to benefit multiple production types. Domain-specific workflows (wedding videography, documentary-only, etc.) belong in separate plugins.

### Speculative fixes
Every skill must solve a real production problem someone actually experienced.

### Bulk PRs
One production area per PR. Multiple unrelated changes will be closed.

### Fabricated content
Invented claims or hallucinated functionality will be rejected immediately.

## Skill Changes Require Testing

Production skills shape how agents coordinate between departments. If you modify skill content:

- Test with multiple production scenarios
- Show before/after behavior with real production examples
- Include evaluation results in your PR
- Do not modify carefully-tuned content without evidence

## General

- One problem per PR
- Test on at least one agent harness
- Describe the production problem you solved
- Understand production workflows before proposing changes
