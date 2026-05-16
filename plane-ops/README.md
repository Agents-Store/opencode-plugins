# plane-ops (OpenCode plugin)

Plane Agile Ops knowledge plugin. Full coverage of the Plane MCP surface: sprint planning, task decomposition, estimation, backlog management, velocity tracking, retrospectives, standups, intake triage, modules, epics, initiatives, milestones, roadmaps, dependencies, burndown, pages (sprint reports, retros, ADRs, runbooks, specs, meeting notes), labels, workflow states, work item types, custom properties, comments, links, work logs, relations, history, bulk edits, search, members, and assignment. Tool- and instance-agnostic: works with any Plane MCP server or connector via a bootstrap skill that discovers tools across naming conventions.

## Install

Project-scoped: copy contents into your project.

```bash
cp opencode.json /path/to/your-project/
cp AGENTS.md /path/to/your-project/
cp -r .opencode /path/to/your-project/
```

User-global: copy `.opencode/agents/` and `.opencode/commands/` into `~/.config/opencode/`.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/plane-ops
