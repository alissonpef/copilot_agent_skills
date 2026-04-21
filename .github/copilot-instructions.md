# Copilot Instructions

This is the always-on instruction file for GitHub Copilot in VS Code.

Treat [README.md](../README.md) as the compact workflow index and [.github/AGENTS.md](AGENTS.md) as the workspace rules file.

## Workspace layout

- `.github/copilot-instructions.md` - project-wide instructions
- `.github/AGENTS.md` - workspace rules file for AI agents
- `.github/prompts/` - slash commands for repeatable workflows
- `.github/agents/` - specialist personas
- `.github/skills/` - reusable workflows and capabilities
- `.github/references/` - orchestration notes and checklists

## Operating rules

- If a task matches a skill, load the matching `SKILL.md` first.
- Use prompt files for slash commands like `/spec`, `/plan`, `/build`, `/test`, `/review`, and `/ship`.
- Use custom agents for specialist roles like review, testing, and security.
- Keep changes small, verified, and aligned with the repository's conventions.
