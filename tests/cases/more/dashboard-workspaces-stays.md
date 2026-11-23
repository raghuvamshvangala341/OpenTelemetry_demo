---
id: dashboard-workspaces-stays
title: Workspaces link leaves the welcome heading visible
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
steps:
  - action: Open the dashboard
    expected: The heading "Welcome back, Test User!" is visible
  - action: Click Workspaces
    expected: The heading "Welcome back, Test User!" is visible
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
