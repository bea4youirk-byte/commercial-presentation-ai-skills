# Compatibility

Reviewed: 2026-08-05.

The repository follows the open Agent Skills structure: one directory per skill, a required `SKILL.md` with `name` and `description` frontmatter, and optional `references/`.

## OpenAI ChatGPT and Codex

OpenAI documents the same progressive-disclosure model: the host discovers name and description first, then loads `SKILL.md` and supporting resources as needed. Install through the Skills interface, Codex skill workflow, OpenAI API skill upload, or a compatible Agent Skills installer.

Official references:

- https://learn.chatgpt.com/docs/build-skills
- https://developers.openai.com/api/docs/guides/tools-skills

## Anthropic Claude and Claude Code

Anthropic custom skills use self-contained directories with `SKILL.md` and optional resources. These skills add task logic and QA; use Claude's available PPTX capability for file operations.

Official reference:

- https://github.com/anthropics/skills

Do not copy proprietary PPTX implementation files from Anthropic's source-available document skills into this repository.

## Google Gemini and Antigravity

Google recommends portable skills via skills.sh. Managed agents discover skills under `.agents/skills/<skill-name>/SKILL.md`; Gemini CLI exposes skill discovery and listing commands.

Official references:

- https://ai.google.dev/gemini-api/docs/coding-agents
- https://ai.google.dev/gemini-api/docs/custom-agents

## Runtime boundary

These are reasoning and workflow skills, not a bundled PowerPoint engine. Each host must supply a safe editable-presentation capability. If a host cannot inspect, render, and export the source deck faithfully, the skill must report the limitation instead of rebuilding a misleading approximation.
