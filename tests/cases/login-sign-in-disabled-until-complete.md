---
id: login-sign-in-disabled-until-complete
title: Sign In stays disabled until both email and password have a value
preconditions:
  - "Mock app is reachable at the staging base URL"
  - "The visitor is not signed in"
steps:
  - action: Open the login page
    expected: The Email field, Password field, and Sign In button are visible, and Sign In is disabled
  - action: Enter only an email and leave the password empty
    expected: Sign In stays disabled
    data: "testuser@example.com"
  - action: Clear the email and enter only a password
    expected: Sign In stays disabled
    data: "env:QZTESTING_AGENTQA_PASSWORD"
  - action: Replace both fields with spaces only
    expected: Sign In stays disabled
  - action: Enter the email
    expected: Sign In stays disabled
    data: "env:QZTESTING_AGENTQA_USERNAME"
  - action: Enter the password
    expected: Sign In becomes enabled
    data: "env:QZTESTING_AGENTQA_PASSWORD"
tags:
  - regression
  - auth
  - web
target: web
priority: p1
---
