---
id: notifications-panel-empty-state
title: Notifications panel opens to an empty state
persona: default
preconditions:
  - User is signed in (reuse existing auth fixture / storage state from the suite)
  - "Mock app is reachable at env: BASE_URL"
steps:
  - action: Open the dashboard
    expected: The Notifications button is visible and the notifications panel is closed
  - action: Click the Notifications button
    expected: The panel opens and shows the heading "Notifications" and the text "No new notifications"
tags:
  - smoke
  - dashboard
  - web
target: web
priority: p1
---
