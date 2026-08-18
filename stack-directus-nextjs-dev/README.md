# stack-directus-nextjs-dev (OpenCode plugin)

Directus + Next.js stack dev plugin. Integrates Directus headless CMS with Next.js App Router for content-driven applications.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## MCP servers

Configured in `opencode.json`. Required environment variables:

- `DIRECTUS_ADMIN_TOKEN`
- `NEXT_PUBLIC_DIRECTUS_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-directus-nextjs-dev
