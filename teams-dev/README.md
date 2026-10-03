# teams-dev (OpenCode plugin)

Microsoft Teams SDK dev plugin for Agents Store. TypeScript guidance for building Teams bots, message extensions, tabs, dialogs and AI agents on Teams SDK 2.1 and Teams Developer CLI 3. Vendors the official microsoft/teams-sdk skill (scaffold, bot registration, SSO setup) and adds skills for the App framework and turn state, Adaptive Cards, openai/MCP/A2A agents, Microsoft Graph, SSO with addOAuthFlow, deployment, sovereign clouds and the Agents Playground.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/teams-dev
