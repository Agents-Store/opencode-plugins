# multi-bank (OpenCode plugin)

Multi-Bank Account Manager with broadcast architecture pattern. Aggregates financial data from Monobank and PrivatBank via MCP tools, broadcasts balance updates and budget alerts to subscribed components, categorizes transactions, and exports financial reports in CSV/PDF.

## Install

Project-scoped: copy contents into your project.

```bash
cp opencode.json /path/to/your-project/
cp AGENTS.md /path/to/your-project/
cp -r .opencode /path/to/your-project/
```

User-global: copy `.opencode/agents/` and `.opencode/commands/` into `~/.config/opencode/`.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/multi-bank
