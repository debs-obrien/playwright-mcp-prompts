---
mode: test-generator
description: This prompt is used to generate a Playwright test from a manual test plan.
tools: ['edit', 'search', 'runCommands', 'runTasks', 'problems', 'changes', 'testFailure', 'todos', 'playwright']
---
# Generate Playwright Test from Manual Test Plan

## Objective
Convert a manual test plan into:

1. A fully automated Playwright test file.
2. Take a screenshot for each step.

## High-Level Workflow

Parse the test plan into discrete actionable steps (each with an intent verb: open, click, fill, select, assert).

For each step:
1. Perform the UI interaction (or assertion).
Immediately verify expected state with a Playwright web-first assertion.

2. Capture a screenshot after the state has stabilized.

3. Assemble a Playwright test using one test() with nested test.step() blocks mirroring the plan steps (or split into multiple tests if the plan has clearly independent scenarios).

4. Prefer resilient, accessibility-driven locators (roles, names, labels). Add comments only when a locator choice is non-obvious.

5. Ensure the test runs headless and passes before finalizing.
