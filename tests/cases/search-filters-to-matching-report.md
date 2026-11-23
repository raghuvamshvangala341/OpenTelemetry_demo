---
id: search-filters-to-matching-report
title: Search shows only the report whose name matches
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
  - "Sales Report, Marketing Dashboard, and Finance Overview are listed"
steps:
  - action: Open the dashboard
    expected: "Search reports" is visible and "Sales Report" is visible
  - action: Enter Sales Report in the search box
    expected: "Sales Report" is visible
    data: "Sales Report"
  - action: Enter marketing in the search box
    expected: "Marketing Dashboard" is visible
    data: "marketing"
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
