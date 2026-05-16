# teleshop

> Teleshop store management plugin. Manage products, orders, categories, attributes, customers, webhooks, and addons for your Telegram store via 50 MCP tools.

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/teleshop

## Skills (exposed as subagents)

- `@skill-addon-management` — Addon and workflow management — listing, toggling, executing, scheduling, and configuring variables. Use when managing store addons, running automation workflows, or configuring addon schedules.
- `@skill-attribute-management` — Attribute CRUD, adding attribute values, and variant configuration. Use when creating product attributes like color, size, or material, or managing attribute values.
- `@skill-catalog-import` — Full catalog import with categories and products from JSON. Use when importing a complete catalog, migrating from another platform, or bulk-loading products.
- `@skill-category-management` — Category CRUD, batch operations, and hierarchy management. Use when creating, updating, deleting, or listing categories in a Teleshop store.
- `@skill-customer-management` — Customer listing and details with order history. Use when viewing customer information, searching customers, or checking a customer's order history.
- `@skill-examples` — MCP tool call patterns, end-to-end workflow examples, code templates, and scenario references. Use when you need reference implementations for Teleshop operations.
- `@skill-order-management` — Order listing, filtering, status updates, payment management, and tracking. Use when viewing orders, changing order status, updating payment, or adding tracking numbers.
- `@skill-product-management` — Product CRUD, batch operations, image and attribute management, variants, filtering and sorting. Use when creating, updating, deleting, or listing products in a Teleshop store.
- `@skill-webhook-management` — Webhook CRUD, event types, testing, delivery logs, statistics, and toggle. Use when setting up webhooks for order/payment notifications or debugging webhook delivery.

## Agents

- `@teleshop-assistant` — Interactive Teleshop store management assistant. Helps merchants manage products, orders, categories, attributes, customers, webhooks, and addons for their Telegram store.
- `@teleshop-catalog-manager` — Specialized catalog management agent for Teleshop. Focused on products, categories, attributes, catalog import, and customer data.

## Commands

- `/create-category` — Create a new product category
- `/create-product` — Create a new product in the store
- `/create-webhook` — Create a new webhook for event notifications
- `/import-catalog` — Import a full catalog of categories and products from JSON data
- `/list-addons` — List all available store addons and their status
- `/list-attributes` — List all product attributes with their values
- `/list-categories` — List all product categories with optional search
- `/list-customers` — List store customers with optional search
- `/list-orders` — List orders with optional status, payment type, and search filters
- `/list-products` — List products with optional search, category, status, and limit filters
- `/list-webhooks` — List all configured webhooks with their status
- `/run-addon` — Manually execute a store addon workflow
- `/update-order-status` — Update the status of an order (created, processing, shipped, completed, etc.)
