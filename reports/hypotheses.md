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
