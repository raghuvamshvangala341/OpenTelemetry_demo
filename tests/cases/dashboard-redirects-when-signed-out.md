---
id: dashboard-redirects-when-signed-out
title: Signed-out visitor is sent from the dashboard to login
preconditions:
  - "Mock app is reachable at env: BASE_URL"
  - "No auth token is stored for this session"
steps:
  - action: Open the dashboard
    expected: The heading "Sign in" is visible
tags:
  - smoke
  - auth
  - web
target: web
priority: p0
---
