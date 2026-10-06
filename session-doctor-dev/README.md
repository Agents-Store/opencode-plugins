# session-doctor-dev (OpenCode plugin)

Read-only audit of a Claude Code session: where it runs, what context it loaded, which model and effort it used, the skills it invoked, every HTTP request with its status code, and the status of each API token seen in the session — with concrete fixes.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/session-doctor-dev
