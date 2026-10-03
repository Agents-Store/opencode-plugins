# sqlalchemy-dev (OpenCode plugin)

SQLAlchemy dev plugin for Agents Store. Typed SQLAlchemy 2.0 style (Mapped, mapped_column, select) with a SQLAlchemy 2.1 section: model definition patterns, relationship mapping, query optimization, Alembic migrations, and troubleshooting.

## Install

Copy this directory's contents into your project (or `~/.config/opencode/` for a global install):

```bash
cp -r .opencode opencode.json AGENTS.md /path/to/your-project/
```

Skills under `.opencode/skills/` are discovered natively by OpenCode (native skill support, Feb 2026) — no manual registration needed.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/sqlalchemy-dev
