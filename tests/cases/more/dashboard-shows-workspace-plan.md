---
id: dashboard-shows-workspace-plan
title: Dashboard shows the Pro workspace plan
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
steps:
  - action: Open the dashboard
    expected: '"Pro workspace" is visible and "12 of 20 reports used" is visible'
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
