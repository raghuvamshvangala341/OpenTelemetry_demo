---
id: dashboard-loads
title: Authenticated dashboard shows primary navigation
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
steps:
  - action: Navigate to the dashboard
    expected: Dashboard heading is visible
  - action: Inspect primary navigation
    expected: Expected nav items from the existing page object are present
tags:
  - smoke
  - dashboard
  - web
target: web
priority: p1
---

Seeded AgentQA case for the Playwright-TS sandbox (AQ-110). Intended to exercise page-object reuse later.
