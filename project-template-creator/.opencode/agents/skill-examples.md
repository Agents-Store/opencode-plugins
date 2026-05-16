---
description: |
  Use this skill when the user asks for "examples", "how does template feedback work", "show me a walkthrough", "demo the template workflow", or needs to see end-to-end scenario walkthroughs for the project-template-creator plugin.
mode: subagent
model: anthropic/claude-sonnet-4-5
temperature: 0.2
permission:
  edit: allow
  bash: allow
---

# Examples — Project Template Creator Walkthroughs

Scenario walkthroughs demonstrating the core workflows.

## Available Scenarios

- @references/scenarios/feedback-flow.md — Push an improvement from a client project to a parent template
- @references/scenarios/create-level1.md — Create a new Level 1 stack template from project-template
- @references/scenarios/wrap-up-session.md — End-of-session review discovering template improvements
