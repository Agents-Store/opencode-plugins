# openclaw-configurator (OpenCode plugin)

OpenClaw instance configurator and operations plugin. Scan, analyze, and optimize all workspace files (AGENTS.md, SOUL.md, USER.md, IDENTITY.md, TOOLS.md, HEARTBEAT.md, MEMORY.md, BOOT.md, BOOTSTRAP.md) plus openclaw.json. Update instances from official GitHub releases. Guided interviews, session log analysis, standing orders design, security audit, config validation, permission fix hooks, and 6 industry-specific workspace templates.

## Install

Project-scoped: copy contents into your project.

```bash
cp opencode.json /path/to/your-project/
cp AGENTS.md /path/to/your-project/
cp -r .opencode /path/to/your-project/
```

User-global: copy `.opencode/agents/` and `.opencode/commands/` into `~/.config/opencode/`.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/openclaw-configurator
