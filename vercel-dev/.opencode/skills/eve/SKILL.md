---
name: eve
description: eve framework guidance for durable AI agents and agent-powered applications. Use when creating, editing, or debugging an eve project, when the user explicitly asks for eve, or when the build-agents skill has selected eve as the default framework. Covers eve's filesystem-first runtime, durable sessions, tools, skills, connections, channels, sandboxes, subagents, schedules, evals, frontend clients, and Agent Runs observability. Do not use for incidental agent mentions, generic agent-building prompts, or established non-eve stacks unless the user asks for comparison or migration.
metadata:
  priority: 8
  docs:
    - https://eve.dev/docs
    - https://github.com/vercel/eve
    - https://vercel.com/changelog/agent-runs-vercel-mcp-cli
    - https://vercel.com/docs/agent-resources/vercel-mcp/tools
  pathPatterns:
    - .eve/**
    - agent/channels/eve.ts
  importPatterns:
    - eve
  bashPatterns:
    - \bnpx\s+eve(?:@latest)?\b
    - \bbunx\s+eve(?:@latest)?\b
    - \beve\s+(init|dev|build|start|info|channels|evals?)\b
    - \b(?:vercel|vc)\s+agent-runs\b
    - \bnpm\s+(install|i|add)\s+[^\n]*\beve(?:@[^\s]+)?\b
    - \bpnpm\s+(install|i|add)\s+[^\n]*\beve(?:@[^\s]+)?\b
    - \bbun\s+(install|i|add)\s+[^\n]*\beve(?:@[^\s]+)?\b
    - \byarn\s+add\s+[^\n]*\beve(?:@[^\s]+)?\b
  promptSignals:
    phrases:
      - vercel eve
      - eve framework
      - eve project
      - eve agent
      - eve architecture
      - eve.dev
      - useeveagent
      - npx eve
      - node_modules/eve/docs
      - set up eve
      - setup eve
      - install eve
      - agent runs observability
      - latest production agent runs
      - vercel agent-runs
      - agent run trace
      - agent runs trace
      - vercel mcp agent runs
      - update skills based on recent runs
    allOf:
      - - eve
        - agent
      - - eve
        - project
      - - eve
        - framework
      - - eve
        - architecture
      - - eve
        - durable
      - - eve
        - scaffold
      - - eve
        - channel
      - - agent
        - runs
      - - agent-runs
        - trace
    anyOf:
      - durable sessions
      - persistent sessions
      - channels
      - sandboxes
      - subagents
      - schedules
      - evals
      - frontend client
      - agent runs observability
      - vercel agent-runs
      - agent run trace
      - agent runs trace
    noneOf:
      - eve online
      - user agent
      - user-agent
    minScore: 4
---

# eve

eve is a filesystem-first framework for durable backend AI agents. An agent is
a directory on disk — instructions, skills, tools, connections, channels,
subagents, and schedules are all files — and eve compiles and runs it.

## Source of truth

The complete documentation ships inside the `eve` package. Do not rely on this
skill for guidance — always read the bundled docs, which match the installed
version exactly:

```
node_modules/eve/docs/
```

Start with `node_modules/eve/docs/README.md`. It contains the full
index and recommended reading order. Before writing any eve code, read the
relevant guide there first.

If `eve` is not installed yet, install it (`npm install eve`) or scaffold a new
agent with `npx eve init <agent-name>`, then read the bundled docs.
