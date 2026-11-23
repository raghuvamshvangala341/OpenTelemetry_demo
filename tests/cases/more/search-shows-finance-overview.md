---
id: search-shows-finance-overview
title: Search for Finance shows Finance Overview
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
  - "Finance Overview is listed"
steps:
  - action: Open the dashboard
    expected: The heading "Finance Overview" is visible
  - action: Enter Finance in the search box
    expected: The heading "Finance Overview" is visible
    data: "Finance"
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
