---

id: dashboard-loads

title: Authenticated dashboard shows primary navigation

preconditions:

  - User is signed in (reuse existing auth fixture / storage state from the suite)

  - "Mock app is reachable at env: BASE_URL"

steps:

  - action: Open the dashboard

    expected: The heading Dashboard is visible

  - action: Click the Reports link

    expected: The Reports link is visible
 

tags:

  - smoke

  - dashboard

  - web

target: web

priority: p1

---
 