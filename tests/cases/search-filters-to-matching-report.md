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
    expected: The search box with placeholder "Search reports..." is visible and three report tiles are visible
  - action: Type Sales Report into the search box
    expected: Only the Sales Report tile is visible
    data: "Sales Report"
  - action: Replace the query with marketing
    expected: Only the Marketing Dashboard tile is visible
    data: "marketing"
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
