# Südzucker AG / Südzucker Group inventory (discovery seed 2026-09-02)
# NOTE: hosts below are discovery candidates from passive DNS/CT; confirm in-scope vs program scope before active testing.
mail.suedzucker.de
suedzucker.de
web.suedzucker.de
www.suedzucker.de

## PASSIVE RECON 2026-09-02 (read-only, non-intrusive)

> Recon observations only. These are NOT confirmed vulnerabilities; ownership/in-scope of each host must be confirmed against the program scope before any active testing. Hosts resolve + serve HTTP — investigation requires scoped authorization.

**Probed:** 4 hosts | **Live HTTP:** 0

| Host | Status | Server/Tech |
|---|---|---|

**CNAME review signals (1):**
- `mail.suedzucker.de` -> `szwmaz0001.suedzucker.de`

## 2026-09-02 21:40:00 UTC

## 2026-09-02 23:35:54 UTC

## 2026-09-03 01:37:08 UTC

## 2026-09-03 06:28:47 UTC

## 2026-09-03 11:41:49 UTC

## 2026-09-03 16:00:35 UTC
- NEW www.suedzuckergroup.com — corporate site redirect target of suedzucker.de (Drupal 11, live)
- NEW shop.suedzucker.com — customer shop SPA with /login (e-commerce auth)
- NEW plantportal.info — Plant Portal (farmer portal, partner-number linking flow)
- NEW app.agriconetwork.com — Giełda Wysłodkowa byproduct trading platform (financial)
- NEW bisz.suedzucker.de — BISZ Rübenanbau portal (Plant Portal link, gov/agri data)
- NEW suedzucker.mitarbeiterangebote.de — employee corporate-benefits portal
- CHANGED inventory root zone: suedzucker.de → suedzuckergroup.com (official rename per on-site announcement)

## 2026-09-03 19:14:36 UTC

## 2026-09-03 21:51:49 UTC
- NEW plantportal.suedzuckergroup.com (Nuxt 3 + PrimeVue, "epp" v1.8.0) — farmer portal, partner-number linking flow confirmed via Nuxt payload
- NEW shop.suedzucker.com (Salesforce B2B Commerce LWR) — live SPA with /login, /cart, /checkout, /order, /SelfRegister, /OrderSummary/:recordId, /product/:recordId routes
- CHANGED plantportal.info → 301 redirects to plantportal.suedzuckergroup.com (subdomain of main corp domain)

## 2026-09-03 23:56:35 UTC
- NEW plantportal.suedzuckergroup.com (Nuxt 3 + PrimeVue, "epp" v1.8.0) — farmer portal, partner-number linking flow confirmed via Nuxt payload
- NEW shop.suedzucker.com (Salesforce B2B Commerce LWR) — live SPA with /login, /cart, /checkout, /order, /SelfRegister, /OrderSummary/:recordId, /product/:recordId routes
- CHANGED plantportal.info → 301 redirects to plantportal.suedzuckergroup.com (subdomain of main corp domain)
- NEW www.suedzuckergroup.com — corporate site redirect target of suedzucker.de (Drupal 11, live)
- NEW shop.suedzucker.com — customer shop SPA with /login (e-commerce auth)
- NEW plantportal.info — Plant Portal (farmer portal, partner-number linking flow)
- NEW app.agriconetwork.com — Giełda Wysłodkowa byproduct trading platform (financial)
- NEW bisz.suedzucker.de — BISZ Rübenanbau portal (Plant Portal link, gov/agri data)
- NEW suedzucker.mitarbeiterangebote.de — employee corporate-benefits portal
- CHANGED inventory root zone: suedzucker.de → suedzuckergroup.com (official rename per on-site announcement)
- NEW plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0 SPA confirmed via `_payload.json`; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a048-5f1242196100); scopes `ap
- NEW shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 262.60); routes `/OrderSummary/:recordId`, `/product/:recordId`, `/cart`, `/checkout`, `/order`, `/SelfRegister`; CSP connect-src includes 
- NEW smartfarming.suedzuckergroup.com/mdp-api/v3/api: MyDataPlant REST API — 574 endpoints in public Swagger UI (no auth to read docs); JSON:API format; JWT token auth (`/tokens` endpoint); requires `X-Sel
- CHANGED plantportal.info → 301 redirects to plantportal.suedzuckergroup.com (subdomain of main corp domain, confirmed live)
- CHANGED Inventory root zone: suedzucker.de → suedzuckergroup.com (official rename per on-site announcement)

## 2026-09-04 02:52:37 UTC

## 2026-09-04 07:31:16 UTC

## 2026-09-04 12:23:16 UTC

## 2026-09-04 16:46:06 UTC

## 2026-09-04 19:18:44 UTC

## 2026-09-04 21:36:21 UTC

## 2026-09-04 23:22:47 UTC

## 2026-09-05 01:08:45 UTC

## 2026-09-05 05:51:00 UTC

## 2026-09-05 09:54:40 UTC
- NEW 2026-09-05 09:52:59 UTC: No new hosts or technology changes observed since last scan 2026-09-05 05:51:00 UTC. Inventory stable across 7 in-scope assets. Knowledge base entries since last run are confi

## 2026-09-05 13:15:34 UTC

## 2026-09-05 16:21:14 UTC

## 2026-09-05 18:29:35 UTC
- CHANGED probed: portal.mydataplant.com /services/*.py sibling sweep (fields.py field.py map.py geometry.py layers.py legend.py user.py export.py wms.py overview.py plan.py) all 404 — outline.py is the SOLE au
- CHANGED probed: smartfarming gateway /mdp-api/v3/api/{openapi,swagger}.json -> 400 application/vnd.api+json (JSON:API Missing-header error, gateway intercepts) — no machine-readable OpenAPI spec exposed; inli

## 2026-09-05 20:47:37 UTC
- CHANGED portal.mydataplant.com/services/*.py sibling sweep complete — 11 paths (fields.py, field.py, map.py, geometry.py, layers.py, legend.py, user.py, export.py, wms.py, overview.py, plan.py) all 404; outli
- CHANGED smartfarming.suedzuckergroup.com/mdp-api/v3/api/{openapi,swagger}.json → 400 application/vnd.api+json (JSON:API Missing-header) — no machine-readable OpenAPI exposed; inline HTML Swagger only surface
- CHANGED reposcan 2026-09-05 18:19 — no public GitHub org for suedzucker; repo-scan structural no-op

## 2026-09-05 22:39:50 UTC
- CHANGED portal.mydataplant.com/services/*.py sibling sweep complete — 11 paths (fields.py, field.py, map.py, geometry.py, layers.py, legend.py, user.py, export.py, wms.py, overview.py, plan.py) all 404; outli
- CHANGED smartfarming.suedzuckergroup.com/mdp-api/v3/api/{openapi,swagger}.json → 400 application/vnd.api+json (JSON:API Missing-header) — no machine-readable OpenAPI exposed; inline HTML Swagger only surface
- CHANGED reposcan 2026-09-05 18:19 — no public GitHub org for suedzucker; repo-scan structural no-op

## 2026-09-06 00:14:25 UTC

## 2026-09-06 04:51:16 UTC
- NEW apps{,,-beta,-dev,-test}.suedzuckergroup.com — **Simplifier Launchpad** (low-code iPaaS), akka-http/10.5.3, SAP UI5 shell, pac4j SSO (`pac4jCsrfToken` cookie), 4 envs on one AWS ALB, certs issued 2026
- NEW rawmaterial{,,-dev,-test}.suedzuckergroup.com — live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root serves generic error page (app path not mapped).
- NEW campus{,,-test}.suedzuckergroup.com — "SZ Group Campus - Login" at /ilp/ (root 302→/ilp/), shared ELB.
- NEW matomo.suedzuckergroup.com — Matomo analytics (matomo.cloud SaaS), public Sign-in page.
- NEW e.suedzuckergroup.com — CNAME to flowmailer.net (email-delivery service, low value).

## 2026-09-06 09:18:46 UTC
- NEW apps{,-beta,-dev,-test}.suedzuckergroup.com — Simplifier Launchpad (low-code iPaaS), akka-http/10.5.3, SAP UI5 shell, pac4j SSO (pac4jCsrfToken), 4 envs on shared AWS ALB, certs 2026-09-02
- NEW rawmaterial{,-dev,-test}.suedzuckergroup.com — live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error, app path not mapped
- NEW campus{,-test}.suedzuckergroup.com — "SZ Group Campus - Login" at /ilp/, root 302 → /ilp/
- NEW matomo.suedzuckergroup.com — Matomo (matomo.cloud SaaS), public Sign-in
- NEW e.suedzuckergroup.com — CNAME→web.flowmailer.net (email-delivery, low value)

## 2026-09-06 13:08:42 UTC

## 2026-09-06 16:17:41 UTC

## 2026-09-06 18:17:45 UTC
- NEW apps{,-beta,-dev,-test}.suedzuckergroup.com — Simplifier Launchpad (low-code iPaaS), akka-http/10.5.3, SAP UI5 shell, pac4j SSO (pac4jCsrfToken), 4 envs on shared AWS ALB, certs 2026-09-02
- NEW rawmaterial{,-dev,-test}.suedzuckergroup.com — live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error, app path not mapped
- NEW campus{,-test}.suedzuckergroup.com — "SZ Group Campus - Login" at /ilp/, root 302 → /ilp/
- NEW matomo.suedzuckergroup.com — Matomo (matomo.cloud SaaS), public Sign-in
- NEW e.suedzuckergroup.com — CNAME→web.flowmailer.net (email-delivery, low value)
- CHANGED portal.mydataplant.com/services/*.py sibling sweep complete — 11 paths all 404; outline.py sole auth-free gateway-bypassing service
- CHANGED smartfarming gateway /mdp-api/v3/api/{openapi,swagger}.json → 400 application/vnd.api+json — no machine-readable OpenAPI exposed
- CHANGED reposcan 2026-09-05 18:19 — no public GitHub org for suedzucker; repo-scan structural no-op
- CHANGED app.cropchart.net — AgricoNetwork's real app host (Moro React SPA + Spring Boot on GKE), uniform 401 MISSING_AUTHORIZATION_HEADER, actuator+Swagger disabled
- CHANGED app.agriconetwork.com — NXDOMAIN, no A/CNAME, no cert in CT history; dead asset confirmed

## 2026-09-06 20:31:31 UTC
- NEW apps{,-beta,-dev,-test}.suedzuckergroup.com — Simplifier Launchpad (low-code iPaaS), akka-http/10.5.3, SAP UI5 shell, pac4j SSO (pac4jCsrfToken), 4 envs on shared AWS ALB, certs 2026-09-02
- NEW rawmaterial{,-dev,-test}.suedzuckergroup.com — live via Azure Front Door (szazweupdfddmz01.z01.azurefd.net); root = generic error, app path not mapped
- NEW campus{,-test}.suedzuckergroup.com — "SZ Group Campus - Login" at /ilp/, root 302 → /ilp/
- NEW matomo.suedzuckergroup.com — Matomo (matomo.cloud SaaS), public Sign-in
- NEW e.suedzuckergroup.com — CNAME→web.flowmailer.net (email-delivery, low value)
- CHANGED portal.mydataplant.com/services/*.py sibling sweep complete — 11 paths all 404; outline.py sole auth-free gateway-bypassing service
- CHANGED smartfarming gateway /mdp-api/v3/api/{openapi,swagger}.json → 400 application/vnd.api+json — no machine-readable OpenAPI exposed
- CHANGED reposcan 2026-09-05 18:19 — no public GitHub org for suedzucker; repo-scan structural no-op
- CHANGED app.cropchart.net — AgricoNetwork's real app host (Moro React SPA + Spring Boot on GKE), uniform 401 MISSING_AUTHORIZATION_HEADER, actuator+Swagger disabled
- CHANGED app.agriconetwork.com — NXDOMAIN, no A/CNAME, no cert in CT history; dead asset confirmed
- CHANGED dev-chatwithyourdata.suedzuckergroup.com — GCP IP 34.117.138.249 but TLS/connect fails (code 000); unreachable
- CHANGED seedrecommender.suedzuckergroup.com — no live A record, certs from 2022; stale CT entry

## 2026-09-06 22:24:45 UTC
- CHANGED Simplifier Launchpad pre-auth management endpoints (`/api`, `/management`, `/actuator`, `/services`, `/rest`, `/admin`, `/config`, `/metadata`, `/registry`) return 404 across all 4 envs (apps, apps-be
- CHANGED rawmaterial{,-dev,-test}.suedzuckergroup.com root returns generic error page (identical HTML across all 3) — app path still unmapped, no new surface
- CHANGED campus{,-test}.suedzuckergroup.com confirmed as IMC Learning Suite (ILP) at `/ilp/` — standard corporate LMS, no high-value class

## 2026-09-07 00:05:49 UTC
- CHANGED No new hosts or technology changes since 2026-09-06 22:24:45 UTC — inventory stable across 11 in-scope assets (www.suedzuckergroup.com, shop.suedzucker.com, plantportal.suedzuckergroup.com, smartfarmi
- CHANGED Simplifier Launchpad pre-auth management endpoints (`/api`, `/management`, `/actuator`, `/services`, `/rest`, `/admin`, `/config`, `/metadata`, `/registry`) confirmed 404 across all 4 envs — pre-auth 
- CHANGED rawmaterial{,-dev,-test}.suedzuckergroup.com root returns identical generic error page — app path unmapped, no attack surface
- CHANGED campus{,-test}.suedzuckergroup.com confirmed IMC Learning Suite (ILP) at `/ilp/` — corporate LMS, out-of-scope class
- CHANGED portal.mydataplant.com/services/outline.py: sole auth-free gateway-bypassing service confirmed (11 sibling *.py paths 404); 200+empty SVG for all tested combos; 500 on non-numeric reveals Apache/2.4.2
- CHANGED smartfarming.suedzuckergroup.com/mdp-api/v3/api: public Swagger (inline HTML, 15k lines) only surface; `/openapi.json` and `/swagger.json` return 400 JSON:API Missing-header — no machine-readable spec
- CHANGED plantportal.suedzuckergroup.com: Nuxt 3 "epp" v1.8.0, MSAL Entra B2C (szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a048-5f1242196100), runtime `__NUXT__` config exposes api-gateway backend 
- CHANGED shop.suedzucker.com: Salesforce B2B Commerce LWR (WebRuntime 236.0), SAP Commerce Cloud backend suedzucker.eu10.hcs.cloud.sap, OAuth via suedzucker.authentication.eu10.hana.ondemand.com (SAP BTP UAA),

## 2026-09-07 04:53:24 UTC
- NEW apps.suedzuckergroup.com/HybridUserInterface/workflow-runtime: auth-free UI5 module "Simplifier Workflow" monitoring UI (`io.simplifier.workflow.rt`) — root/Component.js/manifest/views/controllers all
- CHANGED Simplifier gating model: static asset surface is auth-free (normal UI5), but every API path is gated — `/UserInterface/api` -> pac4j `401 "authentication required"`, `/workflow-runtime/api/*` -> app-l

## 2026-09-07 09:58:10 UTC
- NEW NO_DELTA — no new hosts, tech, or knowledge-base entries since 2026-09-07 04:53 UTC; inventory stable at 11 in-scope assets.
- CHANGED NO_DELTA — all active hypotheses blocked on AUTH_HELPED test accounts; no passive escalation available on existing leads.

## 2026-09-07 15:37:20 UTC
- NEW NO_DELTA — no new hosts, tech, or knowledge-base entries since 2026-09-07 09:58 UTC; inventory stable at 11 in-scope assets.
- CHANGED NO_DELTA — all active hypotheses remain AUTH_HELPED-blocked; no passive escalation path exists on any lead.

## 2026-09-07 19:30:25 UTC
- NEW NO_DELTA — no new hosts, tech, or knowledge-base entries since 2026-09-07 09:58 UTC; inventory stable at 11 in-scope assets.
- CHANGED NO_DELTA — all active hypotheses remain AUTH_HELPED-blocked; no passive escalation path exists on any lead.
- NEW No new hosts, technology changes, or knowledge-base entries since 2026-09-07 15:37 UTC — inventory stable at 11 in-scope assets (www.suedzuckergroup.com, shop.suedzucker.com, plantportal.suedzuckergro
- CHANGED No passive escalation available on any active hypothesis — all three top IDOR targets (plantportal partner-linking, MyDataPlant X-Selected-Partner-Link-Id, shop OrderSummary) remain blocked on AUTH_HE
