# stack-ads (OpenCode plugin)

Paid advertising stack for any project. Researches the product and its market, derives targeting, writes ad copy, generates images, video and voice-over, launches paused campaigns on Google Ads, Meta and TikTok from a reviewed dry-run plan with budget ceilings and a rollback ledger, and reports results. Walks the user through obtaining every key. Integrates Google Ads, Search Console, Meta, TikTok, Firecrawl, Apify, DataForSEO, OpenAI, Gemini and fal.ai via MCP and one dependency-free toolkit.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## MCP servers

Configured in `opencode.json`. Required environment variables:

- `APIFY_TOKEN`
- `DATAFORSEO_PASSWORD`
- `DATAFORSEO_USERNAME`
- `FIRECRAWL_API_KEY`
- `GOOGLE_APPLICATION_CREDENTIALS`
- `GOOGLE_CLOUD_PROJECT`
- `META_ACCESS_TOKEN`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-ads
