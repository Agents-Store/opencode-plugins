# dataforseo-dev (OpenCode plugin)

DataForSEO data analysis plugin. Keyword research, competitor analysis, backlink auditing, SERP monitoring, on-page audits, content analysis, and AI optimization via 70+ MCP tools.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## MCP servers

Configured in `opencode.json`. Required environment variables:

- `DATAFORSEO_PASSWORD`
- `DATAFORSEO_USERNAME`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/dataforseo-dev
