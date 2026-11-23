---
id: profile-menu-shows-sign-out
title: Profile control opens the Sign Out action
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
steps:
  - action: Open the dashboard
    expected: '"TU" is visible'
  - action: Click TU
    expected: '"Sign Out" is visible'
tags:
  - smoke
  - auth
  - web
target: web
priority: p1
---
