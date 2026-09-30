# nocobase (OpenCode plugin)

DEPRECATED — superseded by nocobase-dev, which bundles the official nocobase/skills library and works through the nb CLI and REST API. Its MCP server package (@nocobase/mcp-server) was withdrawn from npm and is no longer wired; the MCP commands and agents work only if you register your own server named `nocobase`. NocoBase platform development plugin. Expert guidance on collections, fields, relations, workflows, UI blocks, plugin development, MCP-powered page management, data operations, and collection inspection for NocoBase applications.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nocobase
