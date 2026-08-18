# nocodb-ops (OpenCode plugin)

NocoDB ops plugin for Agents Store. Record management, views, reports, filtering, search, and data import/export for business users via MCP tools and CLI.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## MCP servers

Configured in `opencode.json`. Required environment variables:

- `NOCODB_MCP_TOKEN`
- `NOCODB_MCP_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nocodb-ops
