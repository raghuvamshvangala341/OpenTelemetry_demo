---
id: logout-returns-to-login
title: Signed-in user can sign out and cannot reopen the dashboard
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
steps:
  - action: Open the dashboard
    expected: The heading "Welcome back, Test User!" is visible
  - action: Click the user profile control labeled TU
    expected: A Sign Out action is visible
  - action: Click Sign Out
    expected: The login form is visible
  - action: Open the dashboard directly again
    expected: The app redirects to the login page and the login form is visible
tags:
  - smoke
  - auth
  - web
target: web
priority: p0
---
