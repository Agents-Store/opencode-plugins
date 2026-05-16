# stack-composable-stack-v1

> Composable Stack v1 dev plugin. Integrates PostgreSQL (direct MCP + PostgREST API), NocoDB, n8n, Trigger.dev, and NocoBase (prod + dev sandbox via nc-mcp) for building data-driven applications with low-code interfaces.

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-composable-stack-v1

## Skills (exposed as subagents)

- `@skill-background-job` — This skill should be used when the user wants to "create a background job", "run async task", "process data in background", "schedule recurring task", "set up a queue", or needs patterns for background processing using Trigger.dev and n8n in the Composable Stack.
- `@skill-full-feature` — This skill should be used when the user wants to "build a complete feature", "create end-to-end functionality", "implement a full feature across all layers", "build feature with data model and automation", or needs a step-by-step recipe for building features that span the Data, Logic, and Interface layers of the Composable Stack.
- `@skill-init-project` — This skill should be used when the user asks to "set up composable stack", "initialize project", "configure environment", "connect MCP services", or needs to set up all MCP connections and environment variables for the Composable Stack v1.
- `@skill-nocobase-to-n8n` — This skill should be used when the user wants to "trigger n8n from NocoBase", "connect NocoBase UI to n8n", "automate NocoBase actions with n8n", "create NocoBase workflow that calls n8n", or needs to integrate NocoBase interface events with n8n workflow automation.
- `@skill-nocodb-to-n8n` — This skill should be used when the user wants to "trigger n8n workflow from NocoDB", "connect NocoDB data to n8n", "create webhook from NocoDB to n8n", "automate NocoDB with n8n", or needs to integrate NocoDB data events with n8n workflow automation.
- `@skill-nocodb-to-trigger` — This skill should be used when the user wants to "trigger background task from NocoDB", "connect NocoDB to Trigger.dev", "process NocoDB data with Trigger.dev", "run background job on NocoDB change", or needs to integrate NocoDB data events with Trigger.dev background tasks.
- `@skill-postgresql-api` — This skill should be used when the user wants to "query PostgreSQL directly", "use PostgREST API", "make REST calls to PostgreSQL", "use postgresql-mcp tools", "run SQL via MCP", "check database status", "inspect database schema", "analyze query performance", or needs to perform direct database operations via PostgreSQL MCP tools or PostgREST REST API in the Composable Stack.

## Agents

- `@stack-orchestrator` — Use this agent when the user needs help coordinating work across PostgreSQL, NocoDB, n8n, Trigger.dev, and NocoBase — building features that span multiple services, debugging cross-service issues, or planning multi-layer operations in the Composable Stack.

<example>
Context: User is building a feature that spans Data and Logic layers
user: "Build an automated order processing flow that creates a NocoDB record and triggers an n8n payment workflow"
assistant: "I'll use the stack-orchestrator agent to coordinate the implementation across NocoDB and n8n."
<commentary>Feature spans Data and Logic layers — orchestrator plans the data model, webhook, and workflow.</commentary>
</example>

<example>
Context: User is debugging a cross-service integration issue
user: "My NocoDB webhook isn't triggering the n8n workflow — records are created but nothing happens"
assistant: "I'll use the stack-orchestrator agent to diagnose the NocoDB-to-n8n connection."
<commentary>Cross-service debugging requires checking both NocoDB webhook config and n8n workflow trigger.</commentary>
</example>

<example>
Context: User wants to plan a full-stack feature
user: "I need a user onboarding system with a NocoBase form, NocoDB data storage, n8n email automation, and Trigger.dev background processing"
assistant: "I'll use the stack-orchestrator agent to design the full-stack implementation plan."
<commentary>Full-stack feature spanning all 5 services — orchestrator coordinates the design across all layers.</commentary>
</example>

