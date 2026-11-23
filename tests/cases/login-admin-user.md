---
id: login-admin-user
title: Admin demo user can sign in
preconditions:
  - "Mock app is reachable at the staging base URL"
  - "A valid demo user exists"
steps:
  - action: Open the login page
    expected: Login form is visible
  - action: Enter the email
    expected: The Email field accepts the username
    data: "env:QZTESTING_AGENTQA_USERNAME"
  - action: Enter the password
    expected: The Password field accepts the password
    data: "env:QZTESTING_AGENTQA_PASSWORD"
  - action: Click Sign In
    expected: The dashboard is shown and the heading "Welcome back, Test User!" is visible
tags:
  - regression
  - auth
  - web
target: web
priority: p1
---
