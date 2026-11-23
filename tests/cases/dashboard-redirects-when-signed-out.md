---
id: dashboard-redirects-when-signed-out
title: Signed-out visitor is sent from the dashboard to login
preconditions:
  - "Mock app is reachable at env: BASE_URL"
  - "No auth token is stored for this session"
steps:
  - action: Open the dashboard
    expected: The login form is visible and the heading "Welcome back, Test User!" is not shown
tags:
  - smoke
  - auth
  - web
target: web
priority: p0
---
