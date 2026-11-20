---

id: login-happy-path

title: Valid user can sign in to the mock app

preconditions:

  - "Mock app is reachable at the staging base URL (env: BASE_URL)"

  - "A valid demo user exists (credentials via env: AQ_USER / AQ_PASS — never literals)"

steps:

  - action: Open the login page

    expected: Login form is visible

  - action: Enter username from env AQ_USER and password from env AQ_PASS

    expected: Fields accept input

  - action: Submit the login form

    expected: User lands on the authenticated dashboard

tags:

  - smoke

  - auth

  - web

target: web

priority: p0

---
 