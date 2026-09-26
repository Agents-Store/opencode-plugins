# n8n (OpenCode plugin)

DEPRECATED — superseded by n8n-dev (building, validating and debugging workflows against both current n8n MCP servers) and n8n-provision (template discovery and batch import). Use those two instead. n8n workflow automation plugin. Manage workflows, execute automations, configure nodes, handle credentials, monitor executions, expression syntax, node configuration patterns, and code node best practices via MCP tools.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## MCP servers

Configured in `opencode.json`. Required environment variables:

- `N8N_MCP_TOKEN`
- `N8N_MCP_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/n8n
