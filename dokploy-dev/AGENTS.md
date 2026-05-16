# dokploy-dev

> Dokploy self-hosted PaaS development plugin. Deploy applications, provision databases (Postgres, MySQL, MariaDB, MongoDB, Redis, LibSQL), manage domains, Docker Compose stacks, backups, and server operations via the official @dokploy/mcp server (500+ tools across 49 categories), 463 REST API endpoints, and CLI.

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/dokploy-dev

## Skills (exposed as subagents)

- `@skill-api-reference` — This skill should be used when making direct HTTP/curl calls to the Dokploy API, looking up endpoint parameters, or building integrations that bypass the MCP server. Triggers: "dokploy API", "curl dokploy", "REST endpoint", "HTTP request to dokploy".
- `@skill-cli-recipes` — This skill should be used when running Dokploy operations from the terminal, deploying via CLI, managing environment variables with env push/pull, or provisioning databases via command line. Triggers: "dokploy cli", "dokploy command", "env push", "env pull", "dokploy deploy cli".
- `@skill-examples` — This skill should be used when learning how to deploy apps, provision databases, or set up Docker Compose stacks on Dokploy. Provides end-to-end workflow walkthroughs. Triggers: "dokploy example", "how to deploy on dokploy", "dokploy tutorial", "dokploy walkthrough", "show me how to use dokploy".
- `@skill-mcp-patterns` — This skill should be used when deploying applications, managing projects, provisioning databases, configuring domains, working with Docker Compose, or performing any Dokploy operation via MCP tools. Triggers: "deploy app", "create project", "add domain", "provision database", "dokploy compose", "manage dokploy".
- `@skill-setup` — This skill should be used when verifying Dokploy MCP connection, CLI installation, and API access. Use when user says "set up dokploy", "verify dokploy connection", "check dokploy", "test dokploy access", or enables the dokploy-dev plugin for the first time.
- `@skill-troubleshoot` — This skill should be used when diagnosing Dokploy deployment failures, domain issues, database connection problems, or Docker/Traefik errors. Use when a deployment fails, domain is not resolving, database cannot connect, app returns 502, or MCP tools return errors. Triggers: "dokploy error", "deployment failed", "domain not working", "502 bad gateway", "database connection refused", "dokploy debug".

## Agents

- `@dokploy-assistant` — Dokploy development assistant for deploying applications, managing projects, provisioning databases, and configuring domains on a self-hosted Dokploy PaaS instance.

<example>
Context: User wants to deploy a web application from GitHub
user: "Deploy my Next.js app from github.com/myorg/myapp to Dokploy with a custom domain"
assistant: "I'll create a project, set up the application with your GitHub repo, configure the domain, and deploy it."
<commentary>Full deployment workflow: create project, create app, connect git, set build type, add domain, deploy.</commentary>
</example>

<example>
Context: User needs to debug a failed deployment
user: "My deployment is failing with a build error, can you check what's wrong?"
assistant: "I'll check the deployment logs and application configuration to diagnose the issue."
<commentary>Diagnostic workflow: check deployment logs, verify environment, check build type and app configuration.</commentary>
</example>

<example>
Context: User wants to provision a database with backups
user: "Set up a PostgreSQL database for my project with daily backups"
assistant: "I'll create a PostgreSQL instance, deploy it, configure external access, and set up automated backups."
<commentary>Database provisioning workflow: create instance, deploy, configure external port, set up automated backup schedule.</commentary>
</example>


## Commands

- `/add-domain` — Add a custom domain to a Dokploy application
- `/create-app` — Create a new application in a Dokploy project
- `/create-db` — Create and deploy a database in a Dokploy project
- `/create-project` — Create a new Dokploy project
- `/deploy` — Deploy or redeploy a Dokploy application or Docker Compose service
- `/list-apps` — List all applications and services in a Dokploy project
- `/list-projects` — List all Dokploy projects
- `/status` — Check Dokploy application or deployment status
