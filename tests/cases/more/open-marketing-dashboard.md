---
id: open-marketing-dashboard
title: Opening Marketing Dashboard leaves that heading visible
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
  - "Marketing Dashboard is listed"
steps:
  - action: Open the dashboard
    expected: The heading "Marketing Dashboard" is visible
  - action: Click Marketing Dashboard
    expected: The heading "Marketing Dashboard" is visible
tags:
  - regression
  - dashboard
  - web
target: web
priority: p1
---
