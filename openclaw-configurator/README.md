# openclaw-configurator (OpenCode plugin)

OpenClaw instance configurator and operations plugin. Scan, analyze, and optimize all workspace files (AGENTS.md, SOUL.md, USER.md, IDENTITY.md, TOOLS.md, HEARTBEAT.md, MEMORY.md, BOOT.md, BOOTSTRAP.md) plus openclaw.json. Update instances from official GitHub releases and reconcile config against new releases (recommend new features, migrate legacy settings, run openclaw doctor). Set up model-provider authentication with an OAuth/CLI-backend-first, cost-saving bias (Claude CLI, Codex OAuth). Migrate .env secrets into self-hosted Infisical. Guided interviews, session log analysis, standing orders design, security audit, config validation, permission fix hooks, centralized doc research, and 6 industry-specific workspace templates.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/openclaw-configurator
