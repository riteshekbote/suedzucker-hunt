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
