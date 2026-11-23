---
id: dashboard-shows-your-reports
title: Dashboard shows the Your reports heading and Sales Report
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
  - "Sales Report is listed"
steps:
  - action: Open the dashboard
    expected: The heading "Your reports" is visible and the heading "Sales Report" is visible
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
