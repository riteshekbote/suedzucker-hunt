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
