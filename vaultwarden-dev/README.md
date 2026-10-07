# vaultwarden-dev (OpenCode plugin)

Vaultwarden dev plugin for Agents Store. Script and integrate a self-hosted Vaultwarden (Bitwarden-compatible) server: what the client API can and cannot do under end-to-end encryption, the identity token flows, organization member management, the /admin panel API, the Bitwarden CLI (bw, bw serve), python-vaultwarden and Terraform, client/server version compatibility, troubleshooting, and a guard hook that asks before a command prints decrypted secrets into the chat. File-based knowledge, no MCP, no stored credentials.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/vaultwarden-dev
