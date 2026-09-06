# Validated findings (running count 0)

- 2 lead(s) marked VALID at 2026-09-06 00:12:08 UTC
  - | Q3 Impact | **YES** — If valid user_id+field_id pairs yield SVG geometry, cross-tenant field boundary/location disclosure (agri location PII). |
  - | Q7 Reasonable triager | **NO** — Cannot demonstrate impact without valid IDs. Architecture is IDOR-prone but proof incomplete. |

- 1 lead(s) marked VALID at 2026-09-06 09:03:45 UTC
  - | Q4 Provable | ❌ | Gateway returns 400 (Missing header) or 403 (unauthed) — this is *correct* behavior. Whether a valid JWT for partner A can use X-Selected-Partner-Link-Id for partner B is untested.

- 3 lead(s) marked VALID at 2026-09-06 15:53:51 UTC
  - | Q3 Real impact? | **YES (if valid IDs exist)** — cross-tenant field boundary/location geometry disclosure (agri location PII) — MEDIUM/HIGH |
  - | Q4 Provable non-invasively? | **NO** — all tested combos returned empty SVG; cannot confirm data disclosure without valid field IDs from own account |
  - | outline.py geometry IDOR | **HOLD** | Confirm scope (Kleffmann vendor?) → own account → test with valid field IDs |
