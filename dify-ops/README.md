# dify-ops (OpenCode plugin)

Dify self-hosted update operations plugin. Pull upstream changes, merge into local dev branch, sync .env variables, detect Docker project names, and rebuild containers for Dify Docker deployments.

## Install

Project-scoped: copy contents into your project.

```bash
cp opencode.json /path/to/your-project/
cp AGENTS.md /path/to/your-project/
cp -r .opencode /path/to/your-project/
```

User-global: copy `.opencode/agents/` and `.opencode/commands/` into `~/.config/opencode/`.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/dify-ops
