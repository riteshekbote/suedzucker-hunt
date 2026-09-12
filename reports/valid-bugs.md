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

- 1 lead(s) marked VALID at 2026-09-07 23:09:21 UTC
  - | Q4 Provable | NO | Requires own JWT + valid X-Selected-Partner-Link-Id header + cross-tenant header mutation; cannot prove without test credentials |

- 5 lead(s) marked VALID at 2026-09-11 20:00:59 UTC
  - **Verdict: VALID**
  - **Verdict: VALID**
  - | Q3 Impact | **PARTIAL** — Field boundary/location geometry is agri location PII. 200 responses with empty SVG body means either test IDs have no geometry or auth failure is soft-fail. Impact depends
  - | MyDataPlant BOLA (X-Selected-Partner-Link-Id) | **VALID** | 8.6 | IDOR/BOLA |
  - | Plant Portal BOLA (switchToPartnerNumber) | **VALID** | 8.1 | IDOR/BOLA |

- 2 lead(s) marked VALID at 2026-09-12 04:58:30 UTC
  - | Q4 Provable | **NO** — requires authenticated session + order placement to capture valid recordId, then test horizontal access |
  - **VALID leads: 0** — All three HOLD leads require AUTH_HELPED testing (own test accounts) to produce a reportable PoC. No lead has sufficient passive proof to pass all 7 gates today.
