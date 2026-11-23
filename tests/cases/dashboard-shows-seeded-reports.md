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
    expected: The heading "Welcome back, Test User!" is visible, Active reports shows 12, Total views (30d) shows 8,420, Scheduled refreshes shows 36, and Connected sources shows 7 with the Healthy badge
  - action: Click the Reports link
    expected: The report tiles Sales Report, Marketing Dashboard, and Finance Overview are visible
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
