# AI Agent Rules

This file provides workspace guidance for AI coding agents in this repository. Treat [README.md](../README.md) as the compact source of truth and [.github/copilot-instructions.md](copilot-instructions.md) as the always-on Copilot instructions.

## Workspace Layout

- `README.md` - workflow index and source of truth
- `.github/copilot-instructions.md` - always-on Copilot instructions
- `.github/AGENTS.md` - workspace rules file for agents
- `.github/prompts/` - slash-command prompts
- `.github/agents/` - specialist personas
- `.github/skills/` - reusable workflows
- `.github/references/` - orchestration notes and checklists

## Operating Rules

- If a task matches a skill, load the matching `SKILL.md` first.
- Use prompt files for `/spec`, `/plan`, `/build`, `/test`, `/review`, and `/ship`.
- Use custom agents for focused review, testing, and security passes.
- The user or a slash command orchestrates. Personas do not invoke other personas.
- `/ship` is the only built-in parallel fan-out pattern in this repository.
- Keep changes small, verified, and aligned with the conventions in the README and skill files.
- If instructions conflict, follow the root README and `.github/copilot-instructions.md`.

## References

- Use the root README for the high-level workflow map.
- Use `references/` for supporting checklists and orchestration patterns.
- Use `skills/` for the detailed workflows behind each phase.