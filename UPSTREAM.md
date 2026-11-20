# Upstream provenance (AQ-110)

| Field | Value |
| --- | --- |
| Source | https://github.com/yousufwaqar/playwright-automation-framework |
| Commit | `cf3dcaa399a83cc952e37912238a800ed163e2b0` (branch `main` at pin) |
| License | MIT (see `LICENSE`) |
| Vendored | 2026-08-19 as a pinned snapshot under `fixtures/sandboxes/playwright-ts/` |

This tree is a **third-party brownfield** Playwright + TypeScript suite we did not author.
AgentQA additions in this tree are limited to:

- this `UPSTREAM.md`
- seeded AgentQA case files under `tests/cases/` (spec FR-1 shape)

Do not treat upstream `agent/` tooling or prompts as AgentQA platform code.
Credentials must remain env/vault refs — never commit real secrets; use `.env.example` patterns only.
