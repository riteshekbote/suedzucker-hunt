# Hypotheses (ranked)

## RANKED HYPOTHESES 2026-09-02 21:40:00 UTC

## RANKED HYPOTHESES 2026-09-02 23:35:54 UTC

## RANKED HYPOTHESES 2026-09-03 01:37:08 UTC

## RANKED HYPOTHESES 2026-09-03 06:28:47 UTC

## RANKED HYPOTHESES 2026-09-03 11:41:49 UTC

## RANKED HYPOTHESES 2026-09-03 16:00:35 UTC
- [55] plantportal.info: Plant Portal partner-number linking IDOR/BOLA (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: GET https://plantportal.info/ then /robots.txt and /.well-known/openid-configuration to map the farmer-portal tech + auth model (read-only reach scan).
- LEARN: REJECTED MISCONFIG @ www.suedzuckergroup.com: JSON:API+GraphQL disabled, registration closed, version files 404 — hardened Drupal; not a vuln.
- LEARN: REJECTED MISCONFIG @ www.suedzuckergroup.com: etracker secure-code in page source is a descriptive/tracking config, not in-scope impact.
- LEARN: ACCEPTED RECON @ suedzucker.de: root renamed to suedzuckergroup.com — passive surface analysis of old zone was targeting dead root; must re-enumerate new TLD.

## RANKED HYPOTHESES 2026-09-03 19:14:36 UTC

## RANKED HYPOTHESES 2026-09-03 21:51:49 UTC
- [60] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant REST API BOLA via numeric single-resource IDs (from art/lead_bigpickle.txt)
- [60] plantportal.suedzuckergroup.com: Plant Portal partner-number linking BOLA/IDOR (from art/lead_nemotron3.txt)
- NEXT(hypotheses-nemotron3.txt): PROBE: GET https://plantportal.suedzuckergroup.com/_nuxt/entry.<hash>.js (from Nuxt payload) to extract API base URLs and partner-linking endpoint paths — read-
- NEXT(hypotheses-bigpickle.txt): PROBE: GET https://smartfarming.suedzuckergroup.com/mdp-api/v3/api (already done — the public Swagger confirms full REST surface reachable without auth; next re
- LEARN: ACCEPTED RECON @ plantportal.info: 301 redirect to plantportal.suedzuckergroup.com (Nuxt 3, PrimeVue, epp v1.8.0) — live farmer portal, not dead asset
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 262.60) with exposed OrderSummary/:recordId and Product/:recordId routes — high-va
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass
- LEARN: ACCEPTED RECON @ suedzucker.mitarbeiterangebote.de: Employee benefits portal with session cookie (CBG3FE) — third-party SSO, employee-only gate
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed) — no further action
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" app confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a0
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full MyDataPlant REST Swagger is publicly browsable (no auth required to read docs); reveals e
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: identified as Salesforce Commerce Cloud "sfdc communities"/DXP (SLDS, /sfsites/). Managed third-party infra; tenant-level 
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (

## RANKED HYPOTHESES 2026-09-03 23:56:35 UTC
- [70] plantportal.suedzuckergroup.com: Plant Portal Partner-Linking BOLA/IDOR (from art/lead_nemotron3.txt)
- [60] plantportal.suedzuckergroup.com: Plant Portal partner-number linking BOLA/IDOR (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: GET https://plantportal.suedzuckergroup.com/_nuxt/entry.<hash>.js (from Nuxt payload) to extract API base URLs and partner-linking endpoint paths — read-
- NEXT(hypotheses-nemotron3.txt): PROBE: GET https://plantportal.suedzuckergroup.com/_nuxt/entry.<hash>.js (from Nuxt payload) to extract API base URLs and partner-linking endpoint paths — read-
- LEARN: ACCEPTED RECON @ plantportal.info: 301 redirect to plantportal.suedzuckergroup.com (Nuxt 3, PrimeVue, epp v1.8.0) — live farmer portal, not dead asset
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 262.60) with exposed OrderSummary/:recordId and Product/:recordId routes — high-va
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass
- LEARN: ACCEPTED RECON @ suedzucker.mitarbeiterangebote.de: Employee benefits portal with session cookie (CBG3FE) — third-party SSO, employee-only gate
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed) — no further action
- LEARN: REJECTED MISCONFIG @ www.suedzuckergroup.com: JSON:API+GraphQL disabled, registration closed, version files 404 — hardened Drupal; not a vuln.
- LEARN: REJECTED MISCONFIG @ www.suedzuckergroup.com: etracker secure-code in page source is a descriptive/tracking config, not in-scope impact.
- LEARN: ACCEPTED RECON @ suedzucker.de: root renamed to suedzuckergroup.com — passive surface analysis of old zone was targeting dead root; must re-enumerate new TLD.
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" app confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a0
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full MyDataPlant REST Swagger is publicly browsable (no auth required to read docs); reveals e
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: identified as Salesforce Commerce Cloud "sfdc communities"/DXP (SLDS, /sfsites/). Managed third-party infra; tenant-level 
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" app confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a0
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full MyDataPlant REST Swagger is publicly browsable (no auth required to read docs); reveals e
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: identified as Salesforce Commerce Cloud "sfdc communities"/DXP (SLDS, /sfsites/). Managed third-party infra; tenant-level 
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full public Swagger (inline sphinx-style HTML, 15k lines) previously known; NOW confirms real 
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets /exportTypes: docs show catalog-style targets (TERMINAL_USB_EXPORT, PDF) not user-arbitrary-URL fetch — SSRF-to-met
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full public Swagger (inline sphinx-style HTML, 15k lines) previously known; NOW confirms real 
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets /exportTypes: docs show catalog-style targets (TERMINAL_USB_EXPORT, PDF) not user-arbitrary-URL fetch — SSRF-to-met
- LEARN: ACCEPTED RECON @ smartfarming/mdp-api/v3/api: public Swagger confirms real backend host portal.mydataplant.com/api/v3, Bearer JWT (iss=auth-backend aud=rest-cli
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: unauthenticated requests return 400 Missing-X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets: catalog-style export targets, not arbitrary-URL server fetch — no SSRF-to-metadata evidence; deprioritize.
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" app confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a0
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full MyDataPlant REST Swagger is publicly browsable (no auth required to read docs); reveals e
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: identified as Salesforce Commerce Cloud "sfdc communities"/DXP (SLDS, /sfsites/). Managed third-party infra; tenant-level 
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed) — no further action

## RANKED HYPOTHESES 2026-09-04 02:52:37 UTC

## RANKED HYPOTHESES 2026-09-04 07:31:16 UTC
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant cross-tenant BOLA via `X-Selected-Partner-Link-Id` tenant-scoping header (from art/lead_bigpickle.txt)
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant cross-tenant BOLA via X-Selected-Partner-Link-Id tenant-scoping header (from art/lead_nemotron3.txt)
- NEXT(hypotheses-nemotron3.txt): PROBE: GET https://plantportal.suedzuckergroup.com/_nuxt/entry.<hash>.js (extract hash from _payload.json) — read-only static asset fetch to enumerate API base 
- NEXT(hypotheses-bigpickle.txt): PROBE: POST https://portal.mydataplant.com/api/v3/tokens with `{"data":{"LOGIN_NAME":"test@test.com","PASSWORD":"test"}}` — test the token endpoint's error hand
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Full public Swagger (15k lines) confirms real backend portal.mydataplant.com/api/v3, Bearer JW
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets: Catalog-style export targets (TERMINAL_USB_EXPORT, PDF) not arbitrary-URL server fetch — no SSRF-to-metadata evide
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404)
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass
- LEARN: ACCEPTED RECON @ smartfarming Swagger analysis: `X-Selected-Partner-Link-Id` is NOT in the API documentation — gateway-level enforcement only. CORS has `access-
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + `image/svg+xml` + empty body for all tested user_id+field_id combos (1/1, 2/123, 9999
- LEARN: ACCEPTED RECON @ portal.mydataplant.com CORS: `access-control-allow-credentials: true` + allows Origin in preflight but does NOT reflect arbitrary origin in sim
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts `Authorization: Bearer` (returns 401 "JWT wrong segments" for malformed token). Does NOT accept `A

## RANKED HYPOTHESES 2026-09-04 12:23:16 UTC
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant cross-tenant BOLA via X-Selected-Partner-Link-Id tenant-scoping header (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: POST https://portal.mydataplant.com/api/v3/tokens with valid-format JWT containing known userId claims — test if the /tokens endpoint can be used to refr
- NEXT(hypotheses-nemotron3.txt): PROBE: GET https://plantportal.suedzuckergroup.com/_nuxt/entry.<hash>.js (extract hash from _payload.json) — read-only static asset fetch to enumerate API base 
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: 500 error on non-numeric user_id reveals Apache/2.4.29 (Ubuntu), webmaster@kleffmann.digital — thir
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (returns 403 "forbidden(149)" without it) despite Swagger doc 
- LEARN: ACCEPTED RECON @ shop.suedzucker.com CSP audit: SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap (OAuth via suedzucker.authentication.eu10.hana.ondemand
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime, __VCAP_ID__ cookie). Sets X-Uaa-Csrf + __Host-JSES
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Full public Swagger (15k lines) confirms real backend portal.mydataplant.com/api/v3, Bearer JW
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets: Catalog-style export targets (TERMINAL_USB_EXPORT, PDF) not arbitrary-URL server fetch — no SSRF-to-metadata evide
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404)
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass
- LEARN: ACCEPTED RECON @ smartfarming Swagger analysis: `X-Selected-Partner-Link-Id` is NOT in the API documentation — gateway-level enforcement only. CORS has `access-
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + `image/svg+xml` + empty body for all tested user_id+field_id combos (1/1, 2/123, 9999
- LEARN: ACCEPTED RECON @ portal.mydataplant.com CORS: `access-control-allow-credentials: true` + allows Origin in preflight but does NOT reflect arbitrary origin in sim
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts `Authorization: Bearer` (returns 401 "JWT wrong segments" for malformed token). Does NOT accept `A

## RANKED HYPOTHESES 2026-09-04 16:46:06 UTC
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant cross-tenant BOLA via X-Selected-Partner-Link-Id tenant-scoping header (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register for a test account on shop.suedzucker.com (/SelfRegister) to obtain SFDC credentials. Then test: (1) GET /OrderSummary/<another_account's_record

## RANKED HYPOTHESES 2026-09-04 19:18:44 UTC
- [70] plantportal.suedzuckergroup.com: Plant Portal Partner-Linking BOLA via switchToPartnerNumber (from art/lead_nemotron3.txt)
- NEXT(hypotheses-nemotron3.txt): PROBE: GET https://plantportal.suedzuckergroup.com/_nuxt/entry.DpUprWo9.js — already fetched; extracted MSAL config (clientId ba3120d6-3d54-478b-a048-5f12421961
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Full public Swagger (15k lines) confirms real backend portal.mydataplant.com/api/v3, Bearer JW
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets: Catalog-style export targets (TERMINAL_USB_EXPORT, PDF) not arbitrary-URL server fetch — no SSRF-to-metadata evide
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ smartfarming Swagger analysis: `X-Selected-Partner-Link-Id` is NOT in the API documentation — gateway-level enforcement only. CORS has `access-
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + `image/svg+xml` + empty body for all tested user_id+field_id combos (1/1, 2/123, 9999
- LEARN: ACCEPTED RECON @ portal.mydataplant.com CORS: `access-control-allow-credentials: true` + allows Origin in preflight but does NOT reflect arbitrary origin in sim
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts `Authorization: Bearer` (returns 401 "JWT wrong segments" for malformed token). Does NOT accept `A
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (returns 403 "forbidden(149)" without it) despite Swagger doc 
- LEARN: ACCEPTED RECON @ shop.suedzucker.com CSP audit: SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap (OAuth via suedzucker.authentication.eu10.hana.ondemand
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime, __VCAP_ID__ cookie). Sets X-Uaa-Csrf + __Host-JSES

## RANKED HYPOTHESES 2026-09-04 21:36:21 UTC
- [70] plantportal.suedzuckergroup.com: Plant Portal Partner-Linking BOLA via switchToPartnerNumber (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: GET https://plantportal.suedzuckergroup.com/_nuxt/entry.DpUprWo9.js — already fetched; extracted MSAL config (clientId ba3120d6-3d54-478b-a048-5f12421961
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com, complete partner linking flow (SMS OTP + Partnernummer), then test horizontal par
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Full public Swagger (15k lines) confirms real backend portal.mydataplant.com/api/v3, Bearer JW
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets: Catalog-style export targets (TERMINAL_USB_EXPORT, PDF) not arbitrary-URL server fetch — no SSRF-to-metadata evide
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ smartfarming Swagger analysis: `X-Selected-Partner-Link-Id` is NOT in the API documentation — gateway-level enforcement only. CORS has `access-
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + `image/svg+xml` + empty body for all tested user_id+field_id combos (1/1, 2/123, 9999
- LEARN: ACCEPTED RECON @ portal.mydataplant.com CORS: `access-control-allow-credentials: true` + allows Origin in preflight but does NOT reflect arbitrary origin in sim
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts `Authorization: Bearer` (returns 401 "JWT wrong segments" for malformed token). Does NOT accept `A
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (returns 403 "forbidden(149)" without it) despite Swagger doc 
- LEARN: ACCEPTED RECON @ shop.suedzucker.com CSP audit: SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap (OAuth via suedzucker.authentication.eu10.hana.ondemand
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime, __VCAP_ID__ cookie). Sets X-Uaa-Csrf + __Host-JSES
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" app confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a0
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full MyDataPlant REST Swagger is publicly browsable (no auth required to read docs); reveals e
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: identified as Salesforce Commerce Cloud "sfdc communities"/DXP (SLDS, /sfsites/). Managed third-party infra; tenant-level 
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" app confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a0
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full MyDataPlant REST Swagger is publicly browsable (no auth required to read docs); reveals e
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: identified as Salesforce Commerce Cloud "sfdc communities"/DXP (SLDS, /sfsites/). Managed third-party infra; tenant-level 
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full public Swagger (inline sphinx-style HTML, 15k lines) previously known; NOW confirms real 
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets /exportTypes: docs show catalog-style targets (TERMINAL_USB_EXPORT, PDF) not user-arbitrary-URL fetch — SSRF-to-met
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full public Swagger (inline sphinx-style HTML, 15k lines) previously known; NOW confirms real 
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets /exportTypes: docs show catalog-style targets (TERMINAL_USB_EXPORT, PDF) not user-arbitrary-URL fetch — SSRF-to-met
- LEARN: ACCEPTED RECON @ smartfarming/mdp-api/v3/api: public Swagger confirms real backend host portal.mydataplant.com/api/v3, Bearer JWT (iss=auth-backend aud=rest-cli
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: unauthenticated requests return 400 Missing-X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets: catalog-style export targets, not arbitrary-URL server fetch — no SSRF-to-metadata evidence; deprioritize.
- LEARN: ACCEPTED RECON @ smartfarming Swagger analysis: `X-Selected-Partner-Link-Id` is NOT in the API documentation — gateway-level enforcement only. CORS has `access-
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + `image/svg+xml` + empty body for all tested user_id+field_id combos (1/1, 2/123, 9999
- LEARN: ACCEPTED RECON @ portal.mydataplant.com CORS: `access-control-allow-credentials: true` + allows Origin in preflight but does NOT reflect arbitrary origin in sim
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts `Authorization: Bearer` (returns 401 "JWT wrong segments" for malformed token). Does NOT accept `A
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: 500 error on non-numeric user_id reveals Apache/2.4.29 (Ubuntu), webmaster@kleffmann.digital — thir
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (returns 403 "forbidden(149)" without it) despite Swagger doc 
- LEARN: ACCEPTED RECON @ shop.suedzucker.com CSP audit: SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap (OAuth via suedzucker.authentication.eu10.hana.ondemand
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime, __VCAP_ID__ cookie). Sets X-Uaa-Csrf + __Host-JSES
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Full public Swagger (15k lines) confirms real backend portal.mydataplant.com/api/v3, Bearer JW
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets: Catalog-style export targets (TERMINAL_USB_EXPORT, PDF) not arbitrary-URL server fetch — no SSRF-to-metadata evide
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ smartfarming Swagger analysis: `X-Selected-Partner-Link-Id` is NOT in the API documentation — gateway-level enforcement only. CORS has `access-
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + `image/svg+xml` + empty body for all tested user_id+field_id combos (1/1, 2/123, 9999
- LEARN: ACCEPTED RECON @ portal.mydataplant.com CORS: `access-control-allow-credentials: true` + allows Origin in preflight but does NOT reflect arbitrary origin in sim
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts `Authorization: Bearer` (returns 401 "JWT wrong segments" for malformed token). Does NOT accept `A
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (returns 403 "forbidden(149)" without it) despite Swagger doc 
- LEARN: ACCEPTED RECON @ shop.suedzucker.com CSP audit: SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap (OAuth via suedzucker.authentication.eu10.hana.ondemand
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime, __VCAP_ID__ cookie). Sets X-Uaa-Csrf + __Host-JSES

## RANKED HYPOTHESES 2026-09-04 23:22:47 UTC
- [70] plantportal.suedzuckergroup.com: Plant Portal Horizontal Partner Data Access via switchToPartnerNumber (from art/lead_nemotron3.txt)
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant cross-tenant BOLA via X-Selected-Partner-Link-Id tenant-scoping header (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: POST https://portal.mydataplant.com/api/v3/tokens with valid-format JWT containing known userId claims — test if the /tokens endpoint can be used to refr
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com, complete partner linking flow (SMS OTP + Partnernummer), then test horizontal par
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: 500 error on non-numeric user_id reveals Apache/2.4.29 (Ubuntu), webmaster@kleffmann.digital — thir
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (returns 403 "forbidden(149)" without it) despite Swagger doc 
- LEARN: ACCEPTED RECON @ shop.suedzucker.com CSP audit: SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap (OAuth via suedzucker.authentication.eu10.hana.ondemand
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime, __VCAP_ID__ cookie). Sets X-Uaa-Csrf + __Host-JSES
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Full public Swagger (15k lines) confirms real backend portal.mydataplant.com/api/v3, Bearer JW
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets: Catalog-style export targets (TERMINAL_USB_EXPORT, PDF) not arbitrary-URL server fetch — no SSRF-to-metadata evide
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ smartfarming Swagger analysis: `X-Selected-Partner-Link-Id` is NOT in the API documentation — gateway-level enforcement only. CORS has `access-
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + `image/svg+xml` + empty body for all tested user_id+field_id combos (1/1, 2/123, 9999
- LEARN: ACCEPTED RECON @ portal.mydataplant.com CORS: `access-control-allow-credentials: true` + allows Origin in preflight but does NOT reflect arbitrary origin in sim
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts `Authorization: Bearer` (returns 401 "JWT wrong segments" for malformed token). Does NOT accept `A
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (returns 403 "forbidden(149)" without it) despite Swagger doc 
- LEARN: ACCEPTED RECON @ shop.suedzucker.com CSP audit: SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap (OAuth via suedzucker.authentication.eu10.hana.ondemand
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime, __VCAP_ID__ cookie). Sets X-Uaa-Csrf + __Host-JSES
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Full public Swagger (15k lines) confirms real backend portal.mydataplant.com/api/v3, Bearer JW
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ smartfarming/portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/
- LEARN: DOWNGRADE SSRF @ smartfarming /exportTargets: Catalog-style export targets (TERMINAL_USB_EXPORT, PDF) not arbitrary-URL server fetch — no SSRF-to-metadata evide
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ smartfarming Swagger analysis: `X-Selected-Partner-Link-Id` is NOT in the API documentation — gateway-level enforcement only. CORS has `access-
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + `image/svg+xml` + empty body for all tested user_id+field_id combos (1/1, 2/123, 9999
- LEARN: ACCEPTED RECON @ portal.mydataplant.com CORS: `access-control-allow-credentials: true` + allows Origin in preflight but does NOT reflect arbitrary origin in sim
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts `Authorization: Bearer` (returns 401 "JWT wrong segments" for malformed token). Does NOT accept `A
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (returns 403 "forbidden(149)" without it) despite Swagger doc 
- LEARN: ACCEPTED RECON @ shop.suedzucker.com CSP audit: SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap (OAuth via suedzucker.authentication.eu10.hana.ondemand
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime, __VCAP_ID__ cookie). Sets X-Uaa-Csrf + __Host-JSES
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com/_nuxt (DpUprWo9 + lazy chunks): epp v1.8.0 client model — BFF base /api-gateway/entra-ext/api/ceres-domain-back
- LEARN: ACCEPTED RECON @ plantportal/api/catalog/companies: unauthenticated 200 exposing internal multi-company catalog (SZ 1000=DE, RT 2001=BE, CHILE 2331, SLS 4100=FR
- LEARN: ACCEPTED RECON @ plantportal/rmp/: served by the same epp Nuxt SPA shell (importmap #entry→/_nuxt/DpUprWo9.js) — no separate legacy RMP app; /rmp/app/common/hom
- LEARN: ACCEPTED RECON @ plantportal/association/impersonation: route guarded only by client middleware (is-authenticated/logged-in-user/only-for-partner); endpoints GE
- LEARN: ACCEPTED RECON @ plantportal/_nuxt (C8VgmCLt/BIRtYruH/pinia store BPdoNzAO): switchToPartnerNumber captured from query in globalInit into client state only; no 
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.

## RANKED HYPOTHESES 2026-09-05 01:08:45 UTC
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com, complete partner linking flow (SMS OTP + Partnernummer), then test horizontal par
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.

## RANKED HYPOTHESES 2026-09-05 05:51:00 UTC
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com, complete partner linking flow (SMS OTP + Partnernummer), then test horizontal par
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.

## RANKED HYPOTHESES 2026-09-05 09:54:40 UTC
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- [64] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal epp partner-scope BOLA (impersonation + current-partner) (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register plantportal test account (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb135611267c, clientId ba3120d6-3d54-47
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com, complete partner linking flow (SMS OTP + Partnernummer), then test horizontal par
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.

## RANKED HYPOTHESES 2026-09-05 13:15:34 UTC
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- [0] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal epp partner-scope BOLA (impersonation + current-partner switch) (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register plantportal test account (Entra B2C signup authority szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb135611267c), link a 7-digit Pa
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com, complete partner linking flow (SMS OTP + Partnernummer), then test horizontal par
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com/_nuxt (DpUprWo9 + lazy chunks): epp v1.8.0 client model — BFF base /api-gateway/entra-ext/api/ceres-domain-back
- LEARN: ACCEPTED RECON @ plantportal/api/catalog/companies: unauthenticated 200 exposing internal multi-company catalog (SZ 1000=DE, RT 2001=BE, CHILE 2331, SLS 4100=FR
- LEARN: ACCEPTED RECON @ plantportal/rmp/: served by the same epp Nuxt SPA shell (importmap #entry→/_nuxt/DpUprWo9.js) — no separate legacy RMP app; /rmp/app/common/hom
- LEARN: ACCEPTED RECON @ plantportal/association/impersonation: route guarded only by client middleware (is-authenticated/logged-in-user/only-for-partner); endpoints GE
- LEARN: ACCEPTED RECON @ plantportal/_nuxt (C8VgmCLt/BIRtYruH/pinia store BPdoNzAO): switchToPartnerNumber captured from query in globalInit into client state only; no 
- LEARN: ACCEPTED RECON @ suedzucker inventory: delta scan 2026-09-05 09:52:59 UTC — no new hosts or technology changes on 7 in-scope assets; surface stable vs prior run
- LEARN: ACCEPTED RECON @ suedzucker inventory: delta scan 09:52:59 UTC — no new hosts/tech changes on 7 in-scope assets; surface stable, repeated scans yield no new pas
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.

## RANKED HYPOTHESES 2026-09-05 16:21:14 UTC
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.

## RANKED HYPOTHESES 2026-09-05 18:29:35 UTC
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- [64] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal epp partner-scope BOLA (impersonation + current-partner switch) (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register plantportal test account (Entra B2C signup authority szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb135611267c, clientId ba3120d6-
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-reada
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-reada
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.

## RANKED HYPOTHESES 2026-09-05 20:47:37 UTC
- [65] shop.suedzucker.com/OrderSummary/:recordId: shop.suedzucker.com SFDC Commerce OrderSummary IDOR via /OrderSummary/:recordId (from art/lead_bigpickle.txt)
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register plantportal test account (Entra B2C signup authority szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb135611267c, clientId ba3120d6-
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-reada
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-reada
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ app.cropchart.net: AgricoNetwork's real app host (linked from agriconetwork.com homepage); "Moro" React SPA + Spring Boot microservices behind 
- LEARN: REJECTED DEAD-ASSET @ app.agriconetwork.com: NXDOMAIN, no A/CNAME record, no cert in CT history (certspotter complete set = only agriconetwork.com/www). Invento
- LEARN: ACCEPTED RECON @ app.cropchart.net/api/assets/fedora/getPublicFile/{r}: auth-free gateway-bypassing file-resolver (200 application/octet-stream "Resource /publi
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-reada
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.

## RANKED HYPOTHESES 2026-09-05 22:39:50 UTC
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register plantportal test account (Entra B2C signup authority szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb135611267c, clientId ba3120d6-
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ app.cropchart.net: AgricoNetwork's real app host (linked from agriconetwork.com homepage); "Moro" React SPA + Spring Boot microservices behind 
- LEARN: REJECTED DEAD-ASSET @ app.agriconetwork.com: NXDOMAIN, no A/CNAME record, no cert in CT history (certspotter complete set = only agriconetwork.com/www). Invento
- LEARN: ACCEPTED RECON @ app.cropchart.net/api/assets/fedora/getPublicFile/{r}: auth-free gateway-bypassing file-resolver (200 application/octet-stream "Resource /publi
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-reada
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-reada
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ app.cropchart.net: AgricoNetwork's real app host (linked from agriconetwork.com homepage); "Moro" React SPA + Spring Boot microservices behind 
- LEARN: REJECTED DEAD-ASSET @ app.agriconetwork.com: NXDOMAIN, no A/CNAME record, no cert in CT history (certspotter complete set = only agriconetwork.com/www). Invento
- LEARN: ACCEPTED RECON @ app.cropchart.net/api/assets/fedora/getPublicFile/{r}: auth-free gateway-bypassing file-resolver (200 application/octet-stream "Resource /publi

## RANKED HYPOTHESES 2026-09-06 00:14:25 UTC
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- [64] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal epp partner-scope BOLA (current-partner switch + impersonation) (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Create plantportal.suedzuckergroup.com test account via Entra B2C signup (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a048-5f124219
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-reada
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ app.cropchart.net: AgricoNetwork's real app host (linked from agriconetwork.com homepage); "Moro" React SPA + Spring Boot microservices behind 
- LEARN: REJECTED DEAD-ASSET @ app.agriconetwork.com: NXDOMAIN, no A/CNAME record, no cert in CT history (certspotter complete set = only agriconetwork.com/www). Invento
- LEARN: ACCEPTED RECON @ app.cropchart.net/api/assets/fedora/getPublicFile/{r}: auth-free gateway-bypassing file-resolver (200 application/octet-stream "Resource /publi

## RANKED HYPOTHESES 2026-09-06 04:51:16 UTC
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- [45] apps{,,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth / management surface across apps*-cluster (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: GET https://apps.suedzuckergroup.com/HybridUserInterface/launchpad/assets/fp-340e776/Component.js then its AuthObject/helper modules (read-only) to extra
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ apps{,-beta,-dev,-test}.suedzuckergroup.com: Simplifier Launchpad (low-code iPaaS) — akka-http/10.5.3, SAP UI5 shell, pac4j SSO (pac4jCsrfToken
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error — app path not
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: "SZ Group Campus - Login" at /ilp/, root 302 — corporate learning portal.
- LEARN: ACCEPTED RECON @ matomo.suedzuckergroup.com: Matomo (matomo.cloud SaaS), public Sign-in — standard login panel, out-of-scope class standalone.
- LEARN: ACCEPTED RECON @ e.suedzuckergroup.com: CNAME→web.flowmailer.net — email-delivery service, low value.
- LEARN: REJECTED DEAD-ASSET @ dev-chatwithyourdata.suedzuckergroup.com: GCP IP 34.117.138.249 but TLS/connect fails (code 000) — unreachable this round.
- LEARN: REJECTED DEAD-ASSET @ seedrecommender.suedzuckergroup.com: no live A record (000), certs from 2022 — stale CT entry.
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-reada
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ app.cropchart.net: AgricoNetwork's real app host (linked from agriconetwork.com homepage); "Moro" React SPA + Spring Boot microservices behind 
- LEARN: REJECTED DEAD-ASSET @ app.agriconetwork.com: NXDOMAIN, no A/CNAME record, no cert in CT history (certspotter complete set = only agriconetwork.com/www). Invento
- LEARN: ACCEPTED RECON @ app.cropchart.net/api/assets/fedora/getPublicFile/{r}: auth-free gateway-bypassing file-resolver (200 application/octet-stream "Resource /publi

## RANKED HYPOTHESES 2026-09-06 09:18:46 UTC
- [65] portal.mydataplant.com/api/v3: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- [35] apps.suedzuckergroup.com/UserInterface/api: Simplifier UI basicAuth brute / default-credential on admin API (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: No new unauth-addressable surface remains on Simplifier (fully gated, verified 3 envs). Next high-value AUTH_HELPED step: on an owned test account, GET `
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ apps{,-beta,-dev,-test}.suedzuckergroup.com: Simplifier Launchpad (low-code iPaaS) — akka-http/10.5.3, SAP UI5 shell, pac4j SSO (pac4jCsrfToken
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error — app path not
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: "SZ Group Campus - Login" at /ilp/, root 302 — corporate learning portal.
- LEARN: ACCEPTED RECON @ matomo.suedzuckergroup.com: Matomo (matomo.cloud SaaS), public Sign-in — standard login panel, out-of-scope class standalone.
- LEARN: ACCEPTED RECON @ e.suedzuckergroup.com: CNAME→web.flowmailer.net — email-delivery service, low value.
- LEARN: REJECTED DEAD-ASSET @ dev-chatwithyourdata.suedzuckergroup.com: GCP IP 34.117.138.249 but TLS/connect fails (code 000) — unreachable this round.
- LEARN: REJECTED DEAD-ASSET @ seedrecommender.suedzuckergroup.com: no live A record (000), certs from 2022 — stale CT entry.
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json → 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-readab
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ app.cropchart.net: AgricoNetwork's real app host (linked from agriconetwork.com homepage); "Moro" React SPA + Spring Boot microservices behind 
- LEARN: REJECTED DEAD-ASSET @ app.agriconetwork.com: NXDOMAIN, no A/CNAME record, no cert in CT history (certspotter complete set = only agriconetwork.com/www). Invento
- LEARN: ACCEPTED RECON @ app.cropchart.net/api/assets/fedora/getPublicFile/{r}: auth-free gateway-bypassing file-resolver (200 application/octet-stream "Resource /publi

## RANKED HYPOTHESES 2026-09-06 13:08:42 UTC
- [65] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- [35] apps.suedzuckergroup.com/UserInterface/api: Simplifier UI basicAuth brute / default-credential on admin API (from art/lead_bigpickle.txt)
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error — app path not
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: "SZ Group Campus - Login" at /ilp/, root 302 — corporate learning portal.
- LEARN: ACCEPTED RECON @ matomo.suedzuckergroup.com: Matomo (matomo.cloud SaaS), public Sign-in — standard login panel, out-of-scope class standalone.
- LEARN: ACCEPTED RECON @ e.suedzuckergroup.com: CNAME→web.flowmailer.net — email-delivery service, low value.
- LEARN: REJECTED DEAD-ASSET @ dev-chatwithyourdata.suedzuckergroup.com: GCP IP 34.117.138.249 but TLS/connect fails (code 000) — unreachable this round.
- LEARN: REJECTED DEAD-ASSET @ seedrecommender.suedzuckergroup.com: no live A record (000), certs from 2022 — stale CT entry.
- LEARN: ACCEPTED RECON @ apps{,-beta,-dev,-test}.suedzuckergroup.com: Simplifier Launchpad (low-code iPaaS) — akka-http/10.5.3, SAP UI5 shell, pac4j SSO (pac4jCsrfToken
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error — app path not
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: "SZ Group Campus - Login" at /ilp/, root 302 — corporate learning portal.
- LEARN: ACCEPTED RECON @ matomo.suedzuckergroup.com: Matomo (matomo.cloud SaaS), public Sign-in — standard login panel, out-of-scope class standalone.
- LEARN: ACCEPTED RECON @ e.suedzuckergroup.com: CNAME→web.flowmailer.net — email-delivery service, low value.
- LEARN: REJECTED DEAD-ASSET @ dev-chatwithyourdata.suedzuckergroup.com: GCP IP 34.117.138.249 but TLS/connect fails (code 000) — unreachable this round.
- LEARN: REJECTED DEAD-ASSET @ seedrecommender.suedzuckergroup.com: no live A record (000), certs from 2022 — stale CT entry.
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" v1.8.0 confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (
- LEARN: REJECTED NOT-VULN @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backen
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: returns 200 + image/svg+xml + empty body for all tested user_id+field_id combos; auth-free, bypasse
- LEARN: ACCEPTED RECON @ portal.mydataplant.com auth: Backend accepts Authorization: Bearer (401 for malformed JWT). Does NOT accept Authentication: Bearer (403 forbidd
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3/tokens: POST /tokens requires Authorization header (403 without) despite Swagger doc stating "Authorization heade
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ suedzucker.authentication.eu10.hana.ondemand.com: SAP BTP UAA server (Cloud Foundry runtime). Sets X-Uaa-Csrf + __Host-JSESSIONID + __VCAP_ID__
- LEARN: CONFIRMED REJECTED @ www.suedzuckergroup.com: Hardened Drupal 11 (JSON:API/GraphQL disabled, registration closed, version files 404).
- LEARN: REJECTED MISCONFIG @ bisz.suedzucker.de: WordPress wp-json API exposure is descriptive/public API, not in-scope impact without auth bypass.
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json → 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-readab
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.
- LEARN: ACCEPTED RECON @ app.cropchart.net: AgricoNetwork's real app host (linked from agriconetwork.com homepage); "Moro" React SPA + Spring Boot microservices behind 
- LEARN: REJECTED DEAD-ASSET @ app.agriconetwork.com: NXDOMAIN, no A/CNAME record, no cert in CT history (certspotter complete set = only agriconetwork.com/www). Invento
- LEARN: ACCEPTED RECON @ app.cropchart.net/api/assets/fedora/getPublicFile/{r}: auth-free gateway-bypassing file-resolver (200 application/octet-stream "Resource /publi
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json → 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-readab

## RANKED HYPOTHESES 2026-09-06 16:17:41 UTC

## RANKED HYPOTHESES 2026-09-06 18:17:45 UTC
- [65] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: On owned Entra B2C test account on plantportal, GET `https://plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services/exte
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ apps{,-beta,-dev,-test}.suedzuckergroup.com: Simplifier Launchpad (low-code iPaaS) — akka-http/10.5.3, SAP UI5 shell, pac4j SSO (pac4jCsrfToken
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error — app path not
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: "SZ Group Campus - Login" at /ilp/, root 302 — corporate learning portal.
- LEARN: ACCEPTED RECON @ matomo.suedzuckergroup.com: Matomo (matomo.cloud SaaS), public Sign-in — standard login panel, out-of-scope class standalone.
- LEARN: ACCEPTED RECON @ e.suedzuckergroup.com: CNAME→web.flowmailer.net — email-delivery service, low value.
- LEARN: REJECTED DEAD-ASSET @ dev-chatwithyourdata.suedzuckergroup.com: GCP IP 34.117.138.249 but TLS/connect fails (code 000) — unreachable this round.
- LEARN: REJECTED DEAD-ASSET @ seedrecommender.suedzuckergroup.com: no live A record (000), certs from 2022 — stale CT entry.
- LEARN: ACCEPTED RECON @ apps{,-beta,-dev,-test}.suedzuckergroup.com: Simplifier Launchpad (low-code iPaaS) — akka-http/10.5.3, SAP UI5 shell, pac4j SSO (pac4jCsrfToken
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error — app path not
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: "SZ Group Campus - Login" at /ilp/, root 302 — corporate learning portal.
- LEARN: ACCEPTED RECON @ matomo.suedzuckergroup.com: Matomo (matomo.cloud SaaS), public Sign-in — standard login panel, out-of-scope class standalone.
- LEARN: ACCEPTED RECON @ e.suedzuckergroup.com: CNAME→web.flowmailer.net — email-delivery service, low value.
- LEARN: REJECTED DEAD-ASSET @ dev-chatwithyourdata.suedzuckergroup.com: GCP IP 34.117.138.249 but TLS/connect fails (code 000) — unreachable this round.
- LEARN: REJECTED DEAD-ASSET @ seedrecommender.suedzuckergroup.com: no live A record (000), certs from 2022 — stale CT entry.
- LEARN: REJECTED DEAD-ASSET @ app.agriconetwork.com: NXDOMAIN, no A/CNAME record, no cert in CT history (certspotter complete set = only agriconetwork.com/www). Invento
- LEARN: ACCEPTED RECON @ app.cropchart.net: AgricoNetwork's real app host (linked from agriconetwork.com homepage); "Moro" React SPA + Spring Boot microservices behind 
- LEARN: ACCEPTED RECON @ app.cropchart.net/api/assets/fedora/getPublicFile/{r}: auth-free gateway-bypassing file-resolver (200 application/octet-stream "Resource /publi
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json → 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-readab
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.

## RANKED HYPOTHESES 2026-09-06 20:31:31 UTC
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_bigpickle.txt)
- [55] apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad Pre-Auth Management Endpoint Exposure (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: On owned Entra B2C test account (2 partner links), read-only GET `https://plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-
- NEXT(hypotheses-nemotron3.txt): PROBE: GET https://apps.suedzuckergroup.com/HybridUserInterface/launchpad/assets/fp-340e776/Component.js (read-only static fetch) → extract internal endpoint re
- LEARN: ACCEPTED RECON @ apps{,-beta,-dev,-test}.suedzuckergroup.com: Simplifier Launchpad (low-code iPaaS) — akka-http/10.5.3, SAP UI5 shell, pac4j SSO (pac4jCsrfToken
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error — app path not
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: "SZ Group Campus - Login" at /ilp/, root 302 — corporate learning portal.
- LEARN: ACCEPTED RECON @ matomo.suedzuckergroup.com: Matomo (matomo.cloud SaaS), public Sign-in — standard login panel, out-of-scope class standalone.
- LEARN: ACCEPTED RECON @ e.suedzuckergroup.com: CNAME→web.flowmailer.net — email-delivery service, low value.
- LEARN: REJECTED DEAD-ASSET @ dev-chatwithyourdata.suedzuckergroup.com: GCP IP 34.117.138.249 but TLS/connect fails (code 000) — unreachable this round.
- LEARN: REJECTED DEAD-ASSET @ seedrecommender.suedzuckergroup.com: no live A record (000), certs from 2022 — stale CT entry.
- LEARN: REJECTED DEAD-ASSET @ app.agriconetwork.com: NXDOMAIN, no A/CNAME record, no cert in CT history (certspotter complete set = only agriconetwork.com/www). Invento
- LEARN: ACCEPTED RECON @ app.cropchart.net: AgricoNetwork's real app host (linked from agriconetwork.com homepage); "Moro" React SPA + Spring Boot microservices behind 
- LEARN: ACCEPTED RECON @ app.cropchart.net/api/assets/fedora/getPublicFile/{r}: auth-free gateway-bypassing file-resolver (200 application/octet-stream "Resource /publi
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/: 11 sibling *.py paths 404 — outline.py is the sole auth-free gateway-bypassing service; sibling enumeration c
- LEARN: ACCEPTED RECON @ smartfarming gateway: /mdp-api/v3/api/{openapi,swagger}.json → 400 application/vnd.api+json (Missing-header JSON:API error) — no machine-readab
- LEARN: ACCEPTED RECON @ reposcan 2026-09-05 18:19: no public GitHub org configured for suedzucker — repo-scan is a structural no-op, no repo surface.

## RANKED HYPOTHESES 2026-09-06 22:24:45 UTC
- [65] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: GET `https://apps.suedzuckergroup.com/HybridUserInterface/launchpad/assets/fp-340e776/Component.js` (read-only static fetch) → extract launchpad internal
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/UserInterface/api: uniform `401 "authentication required"` pac4j gate on all paths incl. Swagger-marked-no-security en
- LEARN: ACCEPTED RECON @ suedzucker inventory: delta scans 09-05→09-06 on repeated timestamps show no new hosts/tech; BOLA pair remains AUTH_HELPED-constrained — re-run
- LEARN: ACCEPTED RECON @ plantportal+smartfarming: both BOLA hypotheses reissued unchanged at same confidence (62/60) — evidence_needed is owned-token diffing only; all
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu

## RANKED HYPOTHESES 2026-09-07 00:05:49 UTC
- [65] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_nemotron3.txt)
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com, tenant 516d27c9-70e5-49b6-8ca4-fb
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu

## RANKED HYPOTHESES 2026-09-07 04:53:24 UTC
- [70] plantportal.suedzuckergroup.com: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): PROBE: AUTH_HELPED — on owned Entra B2C test accounts (2 partner links): GET `https://smartfarming.suedzuckergroup.com/mdp-api/v3/api/fields` with valid Bearer 
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at https://szgrmb2cprod.ciamlogin.com/516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: new auth-free UI5 module = "Simplifier Workflow" monitoring (io.simplifier.workf
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com: per-env gating divergence falsified — all 4 envs identical 401 (workflow-runtime api) and iden
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com: workflow-runtime API adds an IDOR-shape REST family (instance IDs in URLs) behind an app-level gate — worth AUTH_HELP
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu

## RANKED HYPOTHESES 2026-09-07 09:58:10 UTC
- [70] plantportal.suedzuckergroup.com: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register test accounts on two of the three AUTH_HELPED surfaces — plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com) and sh
- NEXT(hypotheses-nemotron3.txt): PROBE: AUTH_HELPED — register test account on plantportal.suedzuckergroup.com (Entra B2C signup at https://szgrmb2cprod.ciamlogin.com/516d27c9-70e5-49b6-8ca4-fb
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/workflow-runtime: IDOR-shape REST family (instance IDs in URLs) behind app-level 401 gate — distinct from pac4j-gated 
- LEARN: ACCEPTED RECON @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (pro
- LEARN: ACCEPTED RECON @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backend) 
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: new auth-free UI5 module "Simplifier Workflow" monitoring (io.simplifier.workflo
- LEARN: ACCEPTED RECON @ apps{,-beta,-dev,-test}.suedzuckergroup.com: Simplifier gating model confirmed — static UI5 assets auth-free, but ALL API paths gated (pac4j 40
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu

## RANKED HYPOTHESES 2026-09-07 15:37:20 UTC
- [70] plantportal.suedzuckergroup.com: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register test accounts on two of the three AUTH_HELPED surfaces — plantportal.suedzuckergroup.com (Entra B2C signup at https://szgrmb2cprod.ciamlogin.com
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register test accounts on two of the three AUTH_HELPED surfaces — plantportal.suedzuckergroup.com (Entra B2C signup at https://szgrmb2cprod.ciamlogin.com
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/workflow-runtime: IDOR-shape REST family (instance IDs in URLs) behind app-level 401 gate — distinct from pac4j-gated 
- LEARN: ACCEPTED RECON @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (pro
- LEARN: ACCEPTED RECON @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backend) 
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: new auth-free UI5 module "Simplifier Workflow" monitoring (io.simplifier.workflo
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com: per-env gating divergence falsified — all 4 envs identical 401 (workflow-runtime api) and iden
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com: workflow-runtime API adds an IDOR-shape REST family (instance IDs in URLs) behind an app-level gate — worth AUTH_HELP
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu

## RANKED HYPOTHESES 2026-09-07 19:30:25 UTC
- [70] plantportal.suedzuckergroup.com: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register test accounts on two of the three AUTH_HELPED surfaces — plantportal.suedzuckergroup.com (Entra B2C signup at szgrmb2cprod.ciamlogin.com) and sh
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register test accounts on two of the three AUTH_HELPED surfaces — plantportal.suedzuckergroup.com (Entra B2C signup at https://szgrmb2cprod.ciamlogin.com
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/workflow-runtime: IDOR-shape REST family (instance IDs in URLs) behind app-level 401 gate — distinct from pac4j-gated 
- LEARN: ACCEPTED RECON @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (pro
- LEARN: ACCEPTED RECON @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backend) 
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: new auth-free UI5 module "Simplifier Workflow" monitoring (io.simplifier.workflo
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com: per-env gating divergence falsified — all 4 envs identical 401 (workflow-runtime api) and iden
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com: workflow-runtime API adds an IDOR-shape REST family (instance IDs in URLs) behind an app-level gate — worth AUTH_HELP
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu

## RANKED HYPOTHESES 2026-09-07 22:18:09 UTC
- [70] plantportal.suedzuckergroup.com: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- [62] smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant Cross-Tenant BOLA via X-Selected-Partner-Link-Id Header (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test accounts on plantportal.suedzuckergroup.com (Entra B2C public sign-up at https://szgrmb2cprod.ciamlogin.com/516d27c9-70e5-49b6-8ca4-f
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register test accounts on two of the three AUTH_HELPED surfaces — plantportal.suedzuckergroup.com (Entra B2C signup at https://szgrmb2cprod.ciamlogin.com
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: new auth-free UI5 module "Simplifier Workflow" monitoring (io.simplifier.workflo
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com: per-env gating divergence falsified — all 4 envs identical 401 (workflow-runtime api) and iden
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com: workflow-runtime API adds an IDOR-shape REST family (instance IDs in URLs) behind an app-level gate — worth AUTH_HELP
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backend) 
- LEARN: ACCEPTED RECON @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (pro

## RANKED HYPOTHESES 2026-09-08 00:30:39 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register an owned account FIRST on shop.suedzucker.com/SelfRegister (this round CONFIRMED serving the registration shell; most-feasible unlock path) with
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test accounts on plantportal.suedzuckergroup.com (Entra B2C public sign-up at https://szgrmb2cprod.ciamlogin.com/516d27c9-70e5-49b6-8ca4-f
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: new auth-free UI5 module "Simplifier Workflow" monitoring (io.simplifier.workflo
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com: per-env gating divergence falsified — all 4 envs identical 401 (workflow-runtime api) and iden
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com: workflow-runtime API adds an IDOR-shape REST family (instance IDs in URLs) behind an app-level gate — worth AUTH_HELP
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backend) 
- LEARN: ACCEPTED RECON @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (pro

## RANKED HYPOTHESES 2026-09-08 05:20:34 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing signup), then

## RANKED HYPOTHESES 2026-09-08 09:49:56 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing signup), then
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator d
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key `AIzaSyAsMk_REDACTED` valid with Places Text Search; Elevation/Directions
- LEARN: ACCEPTED RECON @ dev.siseth.com (cropchart JS bundle reference): NXDOMAIN, unreachable — dead dev environment.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key in window.env: Seth Software Sp. z o.o. (Polish vendor), license key for 2 production envs — c
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: new auth-free UI5 module "Simplifier Workflow" monitoring (io.simplifier.workflo
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com: per-env gating divergence falsified — all 4 envs identical 401 (workflow-runtime api) and iden
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com: workflow-runtime API adds an IDOR-shape REST family (instance IDs in URLs) behind an app-level gate — worth AUTH_HELP
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backend) 
- LEARN: ACCEPTED RECON @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (pro

## RANKED HYPOTHESES 2026-09-08 14:23:25 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing signup), then
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator d
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key `AIzaSyAsMk_REDACTED` valid with Places Text Search; Elevation/Directions/Static Maps NOT ena
- LEARN: ACCEPTED RECON @ dev.siseth.com (cropchart JS bundle reference): NXDOMAIN, unreachable — dead dev environment.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key in window.env: Seth Software Sp. z o.o. (Polish vendor), license key for 2 production envs — c
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator d
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key `AIzaSyAsMk_REDACTED` valid with Places Text Search; Elevation/Directions
- LEARN: ACCEPTED RECON @ dev.siseth.com (cropchart JS bundle reference): NXDOMAIN, unreachable — dead dev environment.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key in window.env: Seth Software Sp. z o.o. (Polish vendor), license key for 2 production envs — c
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal catalog / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/200 — gating inv
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator d
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key `AIzaSyAsMk_REDACTED` valid with Places Text Search; Elevation/Directions/Static Maps NOT ena
- LEARN: ACCEPTED RECON @ dev.siseth.com (cropchart JS bundle reference): NXDOMAIN, unreachable — dead dev environment.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key in window.env: Seth Software Sp. z o.o. (Polish vendor), license key for 2 production envs — c
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: new auth-free UI5 module "Simplifier Workflow" monitoring (io.simplifier.workflo
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com: per-env gating divergence falsified — all 4 envs identical 401 (workflow-runtime api) and iden
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com: workflow-runtime API adds an IDOR-shape REST family (instance IDs in URLs) behind an app-level gate — worth AUTH_HELP
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backend) 
- LEARN: ACCEPTED RECON @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (pro

## RANKED HYPOTHESES 2026-09-08 18:06:10 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal catalog / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/200 — gating inv
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com Simplifier: 5 unregistered runtime modules (management, admin, form, report, analytics) return 503 "No Registration ye
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator d
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key `AIzaSyAsMk_REDACTED` valid with Places Text Search; Elevation/Directions/Static Maps NOT ena
- LEARN: ACCEPTED RECON @ dev.siseth.com (cropchart JS bundle reference): NXDOMAIN, unreachable — dead dev environment.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key in window.env: Seth Software Sp. z o.o. (Polish vendor), license key for 2 production envs — c
- LEARN: ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C, runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated)
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/api/v3: Full public Swagger (15k lines) confirms real backend, Bearer JWT (iss=auth-backend aud=rest-client, userId+emai
- LEARN: ACCEPTED RECON @ shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzu
- LEARN: ACCEPTED RECON @ portal.mydataplant.com/services/outline.py: Confirmed 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.29 Ubuntu + Kl
- LEARN: ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: Public Swagger (inline HTML, 15k lines) only surface; /openapi.json and /swagger.json return 4
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: new auth-free UI5 module "Simplifier Workflow" monitoring (io.simplifier.workflo
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com: per-env gating divergence falsified — all 4 envs identical 401 (workflow-runtime api) and iden
- LEARN: ACCEPTED RECON @ apps.suedzuckergroup.com: workflow-runtime API adds an IDOR-shape REST family (instance IDs in URLs) behind an app-level gate — worth AUTH_HELP
- LEARN: REJECTED MISCONFIG @ apps{,-beta,-dev,-test}.suedzuckergroup.com/HybridUserInterface/launchpad: Simplifier Launchpad pre-auth management endpoints (/api, /manag
- LEARN: ACCEPTED RECON @ campus{,-test}.suedzuckergroup.com: IMC Learning Suite (ILP) at /ilp/ — corporate LMS, standard login, out-of-scope class for high-value findin
- LEARN: ACCEPTED RECON @ rawmaterial{,-dev,-test}.suedzuckergroup.com: Azure Front Door backend, root serves identical generic error page — app path unmapped, no attack
- LEARN: ACCEPTED RECON @ portal.mydataplant.com: Unauthenticated requests return 400 Missing X-Selected-Partner-Link-Id (gateway) or 403 forbidden(149)/(177) (backend) 
- LEARN: ACCEPTED RECON @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (pro

## RANKED HYPOTHESES 2026-09-08 20:50:47 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop /SelfRegister): liveness re-confirmed 200/400/
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator d
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key `AIzaSyAsMk_REDACTED` valid with Places Text Search; Elevation/Directions/Static Maps NOT ena
- LEARN: ACCEPTED RECON @ dev.siseth.com (cropchart JS bundle reference): NXDOMAIN, unreachable — dead dev environment.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key in window.env: Seth Software Sp. z o.o. (Polish vendor), license key for 2 production envs — c
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal catalog / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/200 — gating inv

## RANKED HYPOTHESES 2026-09-08 23:09:41 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identities — shop.suedzucker.com/SelfRegister first (public 200 shell), then Entra B2C self-service signup at szgrmb2cprod.ciamlogin.
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal catalog=200 / smartfarming fields=400 / shop SelfRegister+login=200): liveness re-confirmed 21:0x U
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.

## RANKED HYPOTHESES 2026-09-09 01:19:06 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identities — shop.suedzucker.com/SelfRegister first (public 200 shell), then Entra B2C self-service signup at szgrmb2cprod.ciamlogin.
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage was empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no re
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.

## RANKED HYPOTHESES 2026-09-09 06:08:09 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- [62] shop.suedzucker.com: Salesforce B2B Commerce OrderSummary Record IDOR (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identity via shop.suedzucker.com/SelfRegister (public 200 shell) — complete self-registration flow, create at least one order, then r
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage was empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no re
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.

## RANKED HYPOTHESES 2026-09-09 11:31:53 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- [62] shop.suedzucker.com: Salesforce B2B Commerce OrderSummary Record IDOR (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identity via shop.suedzucker.com/SelfRegister (public 200 shell) — complete self-registration flow, create at least one order, then r
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no repeat
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.

## RANKED HYPOTHESES 2026-09-09 15:24:32 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identity via shop.suedzucker.com/SelfRegister (public 200 shell) — complete self-registration flow, create at least one order, then r
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage was empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no re
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.

## RANKED HYPOTHESES 2026-09-09 18:42:18 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identity via shop.suedzucker.com/SelfRegister (public 200 shell) — complete self-registration flow, create at least one order, then r
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identities via the most-feasible public paths — shop.suedzucker.com/SelfRegister first (live 200 shell, customer-facing Salesforce se
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage was empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no re
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no repeat
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage was empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no re
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.

## RANKED HYPOTHESES 2026-09-09 21:30:13 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Register owned test identity via shop.suedzucker.com/SelfRegister (live 200 shell) — complete self-registration, place at least one order, then IDOR-test
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identity via shop.suedzucker.com/SelfRegister (public 200 shell) — complete self-registration flow, create at least one order, then t
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness re-confirmed 200/400/200 — gating invariant unchanged since 09-07; fifth consecutive NO_DELTA; further
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage was empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no re
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.

## RANKED HYPOTHESES 2026-09-09 23:32:53 UTC
- [62] shop.suedzucker.com: Salesforce B2B Commerce OrderSummary Record IDOR (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Complete owned-account registration at shop.suedzucker.com/SelfRegister (public 200), receive order-confirmation ID, then IDOR-test GET /OrderSummary/{mu
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.

## RANKED HYPOTHESES 2026-09-10 01:29:35 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- [62] shop.suedzucker.com: Salesforce B2B Commerce OrderSummary Record IDOR (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Complete owned-account registration at shop.suedzucker.com/SelfRegister (public 200), receive order-confirmation ID, then IDOR-test GET /OrderSummary/{mu
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identity via shop.suedzucker.com/SelfRegister (public 200 shell) — complete self-registration flow, create at least one order, then t
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage was empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no re
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.

## RANKED HYPOTHESES 2026-09-10 06:43:28 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- [62] shop.suedzucker.com: Salesforce B2B Commerce OrderSummary Record IDOR (from art/lead_bigpickle.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Complete owned-account registration at shop.suedzucker.com/SelfRegister (public 200), receive order-confirmation ID, then IDOR-test GET /OrderSummary/{mu
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identity via shop.suedzucker.com/SelfRegister (public 200 shell) — complete self-registration flow, create at least one order, then t
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage was empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no re
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.

## RANKED HYPOTHESES 2026-09-10 11:53:52 UTC
- [70] plantportal.suedzuckergroup.com/api-gateway/entra-ext/api/ceres-domain-backend-services: Plant Portal Horizontal Partner Data Access via Partner Linking Flow (from art/lead_nemotron3.txt)
- NEXT(hypotheses-bigpickle.txt): HUMAN: Complete owned-account registration at shop.suedzucker.com/SelfRegister (public 200), receive order-confirmation ID, then IDOR-test GET /OrderSummary/{mu
- NEXT(hypotheses-nemotron3.txt): HUMAN: Register owned test identity via shop.suedzucker.com/SelfRegister (public 200 shell) — complete self-registration flow, create at least one order, then t
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces: liveness unchanged; passive phase terminal; program gated on owned-account registration.
- LEARN: REJECTED MISCONFIG @ (none new): prior rejections stand, no class reopens.
- LEARN: ACCEPTED RECON @ suedzucker inventory: 2026-09-08 23:24 triage was empty (no leads); fifth consecutive NO_DELTA on all 11 assets. Passive phase terminal — no re
- LEARN: REJECTED MISCONFIG @ (no new candidate) — none surfaced; prior rejections (Simplifier 503, Drupal hardening, config exposure) stand, no class reopens.
- LEARN: ACCEPTED RECON @ all three AUTH_HELPED surfaces (plantportal /api/catalog/companies / smartfarming /fields / shop SelfRegister): liveness re-confirmed 200/400/2
- LEARN: REJECTED MISCONFIG @ apps.suedzuckergroup.com additional Simplifier modules: 503 "No Registration yet." is a soft deployment failure, not an auth bypass or data
- LEARN: ACCEPTED RECON @ app.cropchart.net /actuator/*: SPA catch-all (Moro index.html, 2549 bytes, openresty+envoy), NOT real Spring Boot actuator — prior KB "actuator
- LEARN: ACCEPTED RECON @ app.cropchart.net window.env: Google Maps API key valid with Places Text Search; Elevation/Directions/Static Maps NOT enabled; billing-abuse su
- LEARN: ACCEPTED RECON @ dev.siseth.com: NXDOMAIN, unreachable — dead dev environment; cropchart JS bundle reference stale.
- LEARN: ACCEPTED RECON @ app.cropchart.net AG Grid Enterprise license key: client-side key for Seth Software Sp. z o.o., not a secret.
