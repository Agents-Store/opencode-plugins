# chatwoot-dev (OpenCode plugin)

Chatwoot dev plugin for Agents Store. Full REST API coverage (Application, Platform, and Public/Client APIs) with bundled OpenAPI specs, official chatwoot CLI recipes, webhook & agent-bot automation, and troubleshooting for developers building on Chatwoot. Authenticates with the api_access_token header via CHATWOOT_API_KEY against CHATWOOT_BASE_URL.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/chatwoot-dev
