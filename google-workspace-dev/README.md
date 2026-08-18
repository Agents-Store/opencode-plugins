# google-workspace-dev (OpenCode plugin)

Google Workspace plugin powered by the official googleworkspace/cli (gws) Agent Skills. ~95 skills for Gmail, Drive, Calendar, Sheets, Docs, Chat, Meet, Tasks, Slides, Forms, Classroom and Admin — plus role personas and ready-made recipes — all driving the gws CLI. Vendored from upstream and auto-synced weekly. Requires the gws CLI (npm i -g @googleworkspace/cli) and a one-time OAuth setup.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/google-workspace-dev
