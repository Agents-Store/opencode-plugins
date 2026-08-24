# macstack-dev (OpenCode plugin)

MACSTACK dev plugin for Agents Store. Creates and maintains the macstack/ folder of a Claude project: macstack.json — the standardized business + technical stack specification — plus the working documents around it: user cases per role, test cases derived from their acceptance bullets, milestones and tasks reconciled with the team's own task tracker, a typed development journal and its client-facing changelog, business logic in plain words, the decision log with cost-if-wrong, open questions split into what the client owes and what the team deferred, and an immutable inbox for client material. Init in existing projects, generate from scratch (result-first), discover context plugins and prototypes, scaffold project files in the prototype → stack plugins → dev plugins order, merge incoming client edits through a gated delta/rulings loop, report where the project stands and what to run next, wire Infisical env, install best-practice rules and commands.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/macstack-dev
