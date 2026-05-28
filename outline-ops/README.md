# outline-ops (OpenCode plugin)

Outline knowledge-base ops plugin. Drive the full Outline REST API by curl — documents (create, search, move, archive, trash, import/export, AI answers, memberships), collections (CRUD, user/group permissions, export), comments, stars, views, shares & access requests, users & groups, attachments & file operations, revisions, templates, events (audit log), OAuth clients, and data attributes. Authenticates with a Bearer OUTLINE_API_KEY against OUTLINE_API_URL.

## Install

Project-scoped: copy contents into your project.

```bash
cp opencode.json /path/to/your-project/
cp AGENTS.md /path/to/your-project/
cp -r .opencode /path/to/your-project/
```

User-global: copy `.opencode/agents/` and `.opencode/commands/` into `~/.config/opencode/`.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/outline-ops
