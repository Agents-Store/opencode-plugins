# outline-ops (OpenCode plugin)

Outline knowledge-base ops plugin. Drive the full Outline REST API by curl — documents (create, search, move, archive, trash, import/export, AI answers, memberships), collections (CRUD, archive, duplicate, import, user/group permissions, export), comments & reactions, pins, subscriptions, notifications, stars, views, shares & access requests, webhook subscriptions, users & groups, attachments & file operations, revisions, templates, events (audit log), API keys, OAuth clients, and data attributes (154 operations). Also points to Outline's built-in MCP server. Authenticates with a Bearer OUTLINE_API_KEY against OUTLINE_API_URL.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/outline-ops
