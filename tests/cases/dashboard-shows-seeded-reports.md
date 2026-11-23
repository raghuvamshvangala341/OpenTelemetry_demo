---
id: dashboard-shows-seeded-reports
title: Dashboard shows the workspace summary and the three seeded reports
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
  - "The mock reports list still contains Sales Report, Marketing Dashboard, and Finance Overview"
steps:
  - action: Open the dashboard
    expected: The heading "Welcome back, Test User!" is visible
  - action: Read the workspace summary
    expected: Active reports shows 12, Total views (30d) shows 8,420, Scheduled refreshes shows 36, and Connected sources shows 7 with the Healthy badge
  - action: Read the Your reports section
    expected: Three report tiles are visible, named Sales Report, Marketing Dashboard, and Finance Overview
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
