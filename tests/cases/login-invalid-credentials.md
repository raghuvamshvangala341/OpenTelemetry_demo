---
id: login-invalid-credentials
title: Unknown credentials stay on the login page with an error
preconditions:
  - "Mock app is reachable at the staging base URL"
  - "The visitor is not signed in"
steps:
  - action: Open the login page
    expected: Login form is visible and the Sign In button is disabled
  - action: Enter an email that is not a known user
    expected: The Email field accepts the value
    data: "invalid@example.com"
  - action: Enter a password that does not match any known user
    expected: The Password field accepts the value and Sign In becomes enabled
    data: "WrongPassword!"
  - action: Click Sign In
    expected: The error "Invalid email or password. Please try again." is visible and the login form is still shown
tags:
  - regression
  - auth
  - web
target: web
priority: p0
---
