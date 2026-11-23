---
id: open-report-updates-title
title: Opening Sales Report leaves the Sales Report heading visible
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
  - "Sales Report is present with id 1"
steps:
  - action: Open the dashboard
    expected: The heading "Sales Report" is visible
  - action: Click Sales Report
    expected: The heading "Sales Report" is visible
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
