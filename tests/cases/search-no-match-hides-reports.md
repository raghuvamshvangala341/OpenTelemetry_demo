---
id: search-no-match-hides-reports
title: A search with no match hides every report tile
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
  - "Sales Report, Marketing Dashboard, and Finance Overview are listed"
steps:
  - action: Open the dashboard
    expected: Sales Report, Marketing Dashboard, and Finance Overview are visible
  - action: Enter does-not-exist in the search box
    expected: No report tiles are visible and the Your reports heading remains
    data: "does-not-exist"
  - action: Enter e in the search box
    expected: Sales Report, Marketing Dashboard, and Finance Overview are visible
    data: "e"
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
