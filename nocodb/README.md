# nocodb (OpenCode plugin)

DEPRECATED — superseded by nocodb-dev (schema, fields, views, Meta API) and nocodb-ops (records, search, views, reports), which teach the current NocoDB MCP tool names; this plugin teaches tool names the server no longer exposes. NocoDB database development plugin. Manage tables, records, columns, views, relations, formulas, rollups, lookups, filtering, sorting, search, aggregation, webhooks, and filter/sort management via MCP tools.

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

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nocodb
