# stack-composable-stack-v1 (OpenCode plugin)

Composable Stack v1 dev plugin. Integrates PostgreSQL (direct MCP + PostgREST API), NocoDB, n8n, Trigger.dev, and NocoBase (prod + dev sandbox via nc-mcp) for building data-driven applications with low-code interfaces.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## MCP servers

Configured in `opencode.json`. Required environment variables:

- `N8N_API_KEY`
- `N8N_API_URL`
- `N8N_MCP_TOKEN`
- `N8N_NATIVE_MCP_URL`
- `NOCOBASE_DEV_API_KEY`
- `NOCOBASE_DEV_URL`
- `NOCODB_MCP_URL`
- `NOCODB_TOKEN`
- `POSTGRESQL_MCP_TOKEN`
- `POSTGRESQL_MCP_URL`
- `TRIGGER_API_URL`
- `TRIGGER_SECRET_KEY`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-composable-stack-v1
