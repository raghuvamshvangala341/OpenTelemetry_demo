---
id: login-sign-in-disabled-until-complete
title: Sign In stays disabled until both email and password have a value
preconditions:
  - "Mock app is reachable at the staging base URL"
  - "The visitor is not signed in"
steps:
  - action: Open the login page
    expected: Login form is visible and Sign In is disabled
  - action: Enter three spaces in the Email field
    expected: Sign In stays disabled
    data: "   "
  - action: Enter the email
    expected: Sign In stays disabled
    data: "env:QZTESTING_AGENTQA_USERNAME"
  - action: Enter three spaces in the Password field
    expected: Sign In stays disabled
    data: "   "
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
