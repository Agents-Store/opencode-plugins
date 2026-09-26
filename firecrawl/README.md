# firecrawl (OpenCode plugin)

DEPRECATED — superseded by web-search-dev, which covers the current Firecrawl MCP tools and REST API v2 alongside Exa, Perplexity, Jina and Context7; this plugin teaches tool names the official Firecrawl MCP server does not expose. Firecrawl web scraping and search plugin. Scrape URLs, crawl sites, search the web, map site structures, extract structured data, batch scraping, autonomous research agents, and cloud browser sessions via MCP tools.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## MCP servers

Configured in `opencode.json`. Required environment variables:

- `FIRECRAWL_MCP_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/firecrawl
