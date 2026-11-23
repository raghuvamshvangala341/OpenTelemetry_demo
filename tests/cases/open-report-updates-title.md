---
id: open-report-updates-title
title: Opening a report tile updates the page title and stays on the dashboard
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
  - "Sales Report is present with id 1"
steps:
  - action: Open the dashboard
    expected: The Sales Report tile is visible and the page title is "Dashboard - Demo App"
  - action: Click the Sales Report tile, not its Delete button
    expected: The page title becomes "Report 1 - Demo App" and the address remains on the dashboard
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
