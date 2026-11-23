---
id: sso-stays-on-sign-in
title: Sign in with SSO leaves the login heading visible
preconditions:
  - "Mock app is reachable at the staging base URL"
  - "The visitor is not signed in"
steps:
  - action: Open the login page
    expected: The heading "Sign in" is visible
  - action: Click Sign in with SSO
    expected: The heading "Sign in" is visible
tags:
  - regression
  - auth
  - web
target: web
priority: p1
---
