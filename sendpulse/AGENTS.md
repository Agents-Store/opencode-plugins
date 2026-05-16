# sendpulse

> Sendpulse multi-channel marketing plugin. Manage chatbots (Telegram, WhatsApp, Instagram, Messenger, Viber), CRM (contacts, deals, pipelines, boards, tasks), email campaigns, templates, addressbooks, and SMTP transactional email via 133+ MCP tools.

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/sendpulse

## Skills (exposed as subagents)

- `@skill-chatbot-contacts-messaging` — Chatbot contact management, direct messaging across channels, contact variables, tags, and notes. Use when sending messages to contacts, managing contact data, or looking up subscribers.
- `@skill-chatbot-management` — Chatbot bots, statistics, tags, campaigns, flows, and dialogs. Use when managing bots, sending chatbot campaigns, running automation flows, or viewing bot statistics.
- `@skill-crm-boards-tasks` — CRM Kanban boards and task management — create boards, manage columns, create and track tasks. Use when organizing work, managing projects, or tracking task completion.
- `@skill-crm-contacts` — CRM contact management — create, update, search, list deals for contacts, and add comments. Use when working with CRM contacts, customer records, or contact-deal relationships.
- `@skill-crm-deals-pipelines` — CRM deals and sales pipelines — create and manage deals, configure pipeline stages, move deals between pipelines. Use when working with sales processes, deal tracking, or pipeline configuration.
- `@skill-crm-products` — CRM product catalog and deal-product associations. Use when managing product listings, adding products to deals, or viewing product-deal relationships.
- `@skill-email-addressbooks` — Email addressbook and subscriber management — create addressbooks, add/remove subscribers, manage variables, check sending costs. Use when managing mailing lists, subscriber data, or email list segmentation.
- `@skill-email-campaigns-templates` — Email campaign creation, management, statistics, and template management. Use when creating email campaigns, designing templates, or analyzing campaign performance.
- `@skill-email-senders-config` — Email sender management, email tags, blacklist management, and account balance. Use when configuring senders, managing email tags, handling blacklisted addresses, or checking account balance.
- `@skill-examples` — MCP tool call patterns, multi-channel marketing workflow examples, and scenario references. Use when you need reference implementations for Sendpulse operations.
- `@skill-smtp-transactional` — SMTP transactional email sending, bounce management, unsubscribe handling, IP and sender domain management. Use when sending transactional emails, managing bounces, or configuring SMTP infrastructure.

## Agents

- `@email-marketing-assistant` — Specialized email marketing assistant. Expert in email campaigns, templates, addressbooks, subscriber management, SMTP transactional emails, and deliverability.
- `@sendpulse-assistant` — Interactive Sendpulse assistant. Helps with chatbot management, CRM operations, email marketing, SMTP transactional emails, and multi-channel campaign orchestration.

## Commands

- `/add-subscriber` — Add a subscriber to an email addressbook
- `/check-balance` — Check Sendpulse account balance and email credits
- `/create-contact` — Create a new CRM contact
- `/create-deal` — Create a new CRM deal in a pipeline
- `/create-email-campaign` — Create and send an email campaign
- `/find-contact` — Find a CRM contact by email address
- `/list-addressbooks` — List email addressbooks with subscriber counts
- `/list-bots` — List all connected chatbots with their channels and statistics
- `/list-contacts` — List CRM contacts
- `/list-deals` — List CRM deals with optional pipeline filter
- `/list-tasks` — List CRM tasks
- `/run-flow` — Run a chatbot automation flow for a contact
- `/send-campaign` — Send a chatbot campaign on a specific channel
- `/send-message` — Send a direct message to a chatbot contact on any channel
- `/send-smtp-email` — Send a transactional email via SMTP
