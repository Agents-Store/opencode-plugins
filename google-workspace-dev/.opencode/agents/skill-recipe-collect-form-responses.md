---
description: Retrieve and review responses from a Google Form.
mode: subagent
model: anthropic/claude-sonnet-4-5
temperature: 0.2
permission:
  edit: allow
  bash: allow
---

# Check Form Responses

> **PREREQUISITE:** Load the following skills to execute this recipe: `gws-forms`

Retrieve and review responses from a Google Form.

## Steps

1. List forms: `gws forms forms list` (if you don't have the form ID)
2. Get form details: `gws forms forms get --params '{"formId": "FORM_ID"}'`
3. Get responses: `gws forms forms responses list --params '{"formId": "FORM_ID"}' --format table`

