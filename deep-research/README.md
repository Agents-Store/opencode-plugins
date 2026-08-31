# deep-research (OpenCode plugin)

Deep Research plugin. Comprehensive web research using 4 providers (Exa, Firecrawl, Jina, Perplexity) with capability-based CONNECTORS pattern and automatic FALLBACK chains. Search, scrape, crawl, extract — each action tries multiple providers until one succeeds.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## MCP servers

Configured in `opencode.json`. Required environment variables:

- `MCPWARE_MCP_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/deep-research
