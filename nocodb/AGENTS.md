# nocodb

> NocoDB database development plugin. Manage tables, records, columns, views, relations, formulas, rollups, lookups, filtering, sorting, search, aggregation, webhooks, and filter/sort management via MCP tools.

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nocodb

## Skills (exposed as subagents)

- `@skill-advanced-queries` — Advanced data queries — search, aggregate, group by, complex filters. This skill should be used when the user asks to perform complex queries, aggregate data, group records, or search with advanced filter logic.
- `@skill-column-field-management` — Column/field types, relations, lookups, rollups, formulas. This skill should be used when the user asks to add columns, configure field types, set up relations, lookups, rollups, or formulas.
- `@skill-examples` — Tool call patterns, end-to-end workflow examples, and scenario references. This skill should be used when the user needs reference implementations, complete examples, or tool call patterns.
- `@skill-record-operations` — Record CRUD, filtering, sorting, bulk operations. This skill should be used when the user asks to create, read, update, or delete records, filter or search data, bulk import, or aggregate values.
- `@skill-schema-design` — Schema design best practices — entity modeling, relation patterns, creation order, formulas, views. This skill should be used when the user asks to design a database schema, plan tables and relationships, or build CRM/ERP/project databases.
- `@skill-table-management` — Table CRUD operations — create, list, get, delete tables. This skill should be used when the user asks to create a table, list existing tables, or manage table structure.
- `@skill-view-management` — View types — Grid, Kanban, Gallery, Form, Calendar. This skill should be used when the user asks to create or configure views, set up a kanban board, build a form, or manage view filters and sorts.
- `@skill-webhook-management` — Webhook management — create, list, delete, and test webhooks for table events. This skill should be used when the user asks to set up webhooks, configure event notifications, or integrate with external systems.

## Agents

- `@nocodb-assistant` — Interactive NocoDB database assistant. Helps with table management, record operations, column configuration, view setup, relations, formulas, and schema design.

<example>
user: "Create a contacts table in NocoDB with name, email, and phone fields"
</example>
<example>
user: "Show me all records in the Orders table"
</example>
<example>
user: "Help me set up relations between Contacts and Deals tables"
</example>

- `@nocodb-schema-designer` — Specialized NocoDB schema design agent. Designs database schemas with proper table structure, relations, lookups, rollups, formulas, and views. Use when planning multi-table NocoDB structures.

<example>
user: "Design a CRM database schema with contacts, companies, and deals"
</example>
<example>
user: "Plan a project management database with tasks, teams, and milestones"
</example>


## Commands

- `/bulk-update` — Bulk update records in a NocoDB table
- `/create-column` — Add a column to a NocoDB table
- `/create-record` — Create a new record in a NocoDB table
- `/create-table` — Create a new table in NocoDB
- `/create-view` — Create a new view for a NocoDB table
- `/list-columns` — List columns in a NocoDB table
- `/list-records` — List records from a NocoDB table with optional filters
- `/list-tables` — List all tables in the NocoDB base
- `/list-views` — List views for a NocoDB table
- `/search-records` — Search records in a NocoDB table
