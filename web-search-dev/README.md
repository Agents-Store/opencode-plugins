# web-search-dev (OpenCode plugin)

Developer reference for web search, scraping and documentation lookup — Firecrawl, Exa, Jina, Perplexity, Context7 MCP tools and REST/SDK/CLI — plus Pexels and Unsplash REST media search.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## MCP servers

Configured in `opencode.json`. Required environment variables:

- `CONTEXT7_API_KEY`
- `EXA_API_KEY`
- `FIRECRAWL_API_TOKEN`
- `JINA_API_KEY`
- `PERPLEXITY_API_KEY`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/web-search-dev
