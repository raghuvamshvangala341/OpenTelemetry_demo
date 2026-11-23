---
id: login-admin-user
title: Admin demo user can sign in
preconditions:
  - "Mock app is reachable at the staging base URL"
  - "The admin demo user from the mock app is available"
steps:
  - action: Open the login page
    expected: Login form is visible
  - action: Enter the admin email
    expected: The Email field accepts the email
    data: "admin@example.com"
  - action: Enter the admin password
    expected: The Password field accepts the password and Sign In becomes enabled
    data: "AdminPassword123!"
  - action: Click Sign In
    expected: The dashboard is shown and the heading "Welcome back, Test User!" is visible
tags:
  - regression
  - auth
  - web
target: web
priority: p1
---
