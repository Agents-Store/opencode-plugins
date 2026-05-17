# payloadcms-dev

> PayloadCMS dev plugin for Agents Store. Covers collections, fields, hooks, access control, queries, adapters, Lexical rich text, jobs queue, plugin development, Next.js integration, CLI, migrations, and end-to-end scenarios for TypeScript developers building with Payload v3.

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/payloadcms-dev

## Skills (exposed as subagents)

- `@skill-access-control` — This skill should be used when the user asks about "Payload access control", "RBAC in Payload", "row-level security", "isAdmin function", "field access control", "global access control", "overrideAccess", "multi-tenant Payload", "filter by user role", "Payload Access function", or needs to decide who can create/read/update/delete documents.
- `@skill-adapters` — This skill should be used when the user asks about "Payload database adapter", "Postgres in Payload", "MongoDB Payload setup", "SQLite Payload", "S3 storage adapter", "Cloudflare R2 Payload", "Vercel Blob upload", "Payload email Resend", "Payload Nodemailer SMTP", "Payload transactions", or needs to wire Payload to a database, file storage, or email provider.
- `@skill-api-reference` — This skill should be used when the user asks for "PayloadCMS REST endpoint", "Payload curl example", "Payload GraphQL query syntax", "Payload Local API method signature", "Payload login endpoint", "Payload auth headers", or needs the exact HTTP/method signature for a Payload API call.
- `@skill-cli-recipes` — This skill should be used when the user asks about "payload migrate", "payload generate:types", "payload generate:importmap", "payload migrate:create", "payload migrate:down", "payload migrate:reset", "payload migrate:refresh", "payload migrate:status", "Payload CLI commands", or needs to run the Payload command-line tool for schema migrations or codegen.
- `@skill-cms-migration` — This skill should be used when the user asks to "migrate WordPress to Payload", "move content from Contentful to Payload", "import Strapi data into Payload", "migrate Sanity to PayloadCMS", "Webflow CMS to Payload", "design Payload collections from CMS export", or needs a structured workflow for moving content from another CMS into Payload.
- `@skill-collections` — This skill should be used when the user asks to "create a Payload collection", "define a CollectionConfig", "set up an auth collection", "build an upload collection", "add drafts/versions", "configure admin panel for a collection", "enable live preview", "set defaultColumns", or needs to model any content type in PayloadCMS v3.
- `@skill-examples` — This skill should be used when the user asks "show me a complete Payload example", "give me a working Payload blog", "Payload ecommerce example", "Payload auth-only API example", "Payload jobs worker example", "Payload multi-tenant example", or wants end-to-end scenario walkthroughs instead of isolated snippets.
- `@skill-fields` — This skill should be used when the user asks about "Payload field types", "add a relationship field", "blocks field", "array field", "rich text field", "upload field", "virtual field", "conditional fields", "field validation", "join field", "point/geolocation field", "slug field helper", or needs to design any field inside a PayloadCMS collection or global.
- `@skill-hooks` — This skill should be used when the user asks about "Payload hooks", "beforeChange", "afterChange", "afterRead", "beforeDelete", "field hooks", "global hooks", "prevent hook loops", "Next.js revalidation in Payload", "transaction safe hooks", "auto-set author from req.user", or needs to wire up lifecycle automation in PayloadCMS.
- `@skill-jobs-queue` — This skill should be used when the user asks about "Payload jobs queue", "Payload background tasks", "Payload workflows", "Payload cron scheduling", "Payload task retries", "Payload runJobs", "Payload autoRun", "queue a job in Payload", or needs to run any background or scheduled work in PayloadCMS.
- `@skill-lexical-editor` — This skill should be used when the user asks about "Payload rich text", "Lexical editor in Payload", "custom Lexical feature", "richText blocks", "richText link/upload/relationship", "custom Lexical node", "render Payload Lexical to JSX", "convert Lexical to HTML", or needs to customize the editor inside `richText` fields.
- `@skill-nextjs-integration` — This skill should be used when the user asks about "Payload with Next.js", "getPayload in server component", "Payload App Router", "Payload route groups", "Payload live preview Next.js", "revalidate Payload page", "Payload server actions", "Payload draft mode", "Payload Next.js cache", or needs to wire PayloadCMS into a Next.js v14/v15 frontend.
- `@skill-plugin-development` — This skill should be used when the user asks to "build a Payload plugin", "create payload-plugin package", "write a Payload plugin from scratch", "add fields via plugin", "preserve hooks in plugin", "publish payload-plugin to npm", "plugin architecture in Payload", or needs to author or maintain a reusable PayloadCMS plugin.
- `@skill-queries` — This skill should be used when the user asks about "Payload Local API", "payload.find", "payload.findByID", "where query", "Payload query operators", "depth and populate", "filter Payload by relationship", "sort and paginate Payload results", "Payload REST API query string", "GraphQL queries", or needs to read or write data with Payload.
- `@skill-setup` — This skill should be used when the user asks to "install PayloadCMS", "create a Payload project", "set up Payload v3", "scaffold Payload app", "initialize Payload with Next.js", "pick a Payload database adapter", "configure payload.config.ts", or needs to bootstrap a fresh Payload project from zero to a running admin panel.
- `@skill-troubleshoot` — This skill should be used when the user asks about "Payload error", "Payload not working", "Payload TypeError", "access bypass in Local API", "Payload hook infinite loop", "Payload transaction rollback", "Cannot find module payload", "Payload import map missing", "Payload type generation fails", "Could not resolve component", or sees a stack trace from Payload they want decoded.

## Agents

- `@payloadcms-developer` — Use this agent when the user is actively building, debugging, or extending a PayloadCMS v3 project — designing collections and fields, wiring hooks and access control, integrating Payload with Next.js, building third-party Payload plugins, migrating from another CMS, or troubleshooting a Payload error.

<example>
Context: The user is starting a new Payload-backed project.
user: "Help me design collections for a SaaS that has projects, project members, and timesheet entries."
assistant: "I'll use the payloadcms-developer agent to design the data model end-to-end."
<commentary>This is multi-collection schema design with access control implications — the developer agent loads the right Payload skills and proposes a typed, tenant-aware design.</commentary>
</example>

<example>
Context: A hook is misbehaving in production.
user: "My afterChange hook keeps firing in a loop and exhausting DB connections."
assistant: "Let me use the payloadcms-developer agent to diagnose the loop and apply the context-flag pattern."
<commentary>The agent invokes the troubleshoot and hooks skills, then proposes a targeted fix with the req.context guard pattern.</commentary>
</example>

<example>
Context: The user is authoring a reusable Payload plugin.
user: "I want to publish a payload-plugin-sentry package that adds error reporting to every collection's afterError hook."
assistant: "I'll use the payloadcms-developer agent — this needs the plugin-development conventions and the right (options) => (config) pattern."
<commentary>Plugin authoring has specific structural rules (SWC build, multi-export entrypoints, hook-array preservation) that the agent enforces via the plugin-development skill.</commentary>
</example>


## Commands

- `/scaffold` — Scaffold a fresh PayloadCMS v3 project with create-payload-app, walking through database adapter, template, and package manager choices.
