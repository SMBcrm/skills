# SMBcrm Skills

Skill files for AI agents and Claude Code users working with SMBcrm. Skills are structured reference guides that teach AI assistants how to help you use SMBcrm's advanced tooling correctly and efficiently.

## What are Skills?

A skill is a markdown file that gives an AI assistant (like Claude) deep, platform-specific knowledge about a particular domain. When a skill is loaded, the assistant knows the right terminology, correct API patterns, and best practices — without you having to explain them.

Skills in this repo are designed for use with [Claude Code](https://claude.ai/code) and other MCP-compatible AI clients.

## Available Skills

| Skill | Description |
|---|---|
| [`skills/smbcrm-skill.md`](skills/smbcrm-skill.md) | Advanced tools: Private Integration Tokens, REST API v2, Workflows, Webhooks, MCP, and Agent Studio |

## Using a Skill

### Option 1 — Claude Code (recommended)

Add this repo as a skill source in your Claude Code settings, or copy the skill file into your project's `.claude/skills/` directory.

### Option 2 — Manual

Paste the contents of a skill file into your AI assistant's system prompt or context window before starting your session.

### Option 3 — MCP

If your AI client supports MCP, point it at `https://services.smbcrm.com/mcp/` using your Private Integration Token. The `smbcrm-skill.md` skill explains the full setup.

## What the SMBcrm Advanced Tools Skill Covers

- **Private Integration Tokens** — how to create, scope, and rotate them
- **REST API v2** — correct headers, base URL, and implementation patterns for all 16 API products
- **Workflows** — native automation design patterns (intake, SLA, scheduling, AI handoff)
- **Webhooks** — outbound and custom webhook patterns with security best practices
- **MCP** — connecting AI clients directly to SMBcrm tools
- **Agent Studio API** — executing agents programmatically from external apps
- **Troubleshooting** — common errors (401, 403, 404, 422) and how to resolve them

## API Reference

Full REST API documentation is available at:

**[https://developers.smbcrm.com/](https://developers.smbcrm.com/)**

All API endpoints use the base URL `https://services.smbcrm.com`.

## Contributing

1. Fork this repo
2. Add or update a skill in the `skills/` directory
3. Keep skills focused and single-purpose
4. Open a pull request with a short description of what changed and why

## License

MIT
