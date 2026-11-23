---
id: login-shows-sign-in-heading
title: Login page shows the Sign in heading
preconditions:
  - "Mock app is reachable at the staging base URL"
  - "The visitor is not signed in"
steps:
  - action: Open the login page
    expected: The heading "Sign in" is visible
tags:
  - smoke
  - auth
  - web
target: web
priority: p0
---
