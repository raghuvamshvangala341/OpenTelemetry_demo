---
id: login-shows-email-and-password
title: Login page shows the Email and Password labels
preconditions:
  - "Mock app is reachable at the staging base URL"
  - "The visitor is not signed in"
steps:
  - action: Open the login page
    expected: The "Email" label is visible and the "Password" label is visible
tags:
  - regression
  - auth
  - web
target: web
priority: p1
---
