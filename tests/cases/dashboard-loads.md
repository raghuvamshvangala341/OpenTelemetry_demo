---

id: dashboard-loads

title: Authenticated dashboard shows primary navigation

preconditions:

  - User is signed in (reuse existing auth fixture / storage state from the suite)

  - "Mock app is reachable at env: BASE_URL"

steps:

  - action: Open the dashboard

    expected: The heading Dashboard is visible

  - action: Look at the primary navigation

    expected: The links Home, Reports, and Workspaces are visible

tags:

  - smoke

  - dashboard

  - web

target: web

priority: p1

---
 