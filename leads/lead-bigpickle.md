## 2026-09-03 15:45:20 UTC [target] (model bigpickle)
[NEW] www.suedzuckergroup.com — corporate site redirect target of suedzucker.de (Drupal 11, live)
[NEW] shop.suedzucker.com — customer shop SPA with /login (e-commerce auth)
[NEW] plantportal.info — Plant Portal (farmer portal, partner-number linking flow)
[NEW] app.agriconetwork.com — Giełda Wysłodkowa byproduct trading platform (financial)
[NEW] bisz.suedzucker.de — BISZ Rübenanbau portal (Plant Portal link, gov/agri data)
[NEW] suedzucker.mitarbeiterangebote.de — employee corporate-benefits portal
[CHANGED] inventory root zone: suedzucker.de → suedzuckergroup.com (official rename per on-site announcement)
[PRIO] plantportal.info,score=8.1,axis=business_value high (farmer PII/contracts) + gate_ease partial (public registration) + tech_exposure (custom auth, OTP-by-SMS-link flow)
[PRIO] app.agriconetwork.com,score=8.3,axis=business_value high (money/auth trading) + custom app
[PRIO] shop.suedzucker.com,score=7.8,axis=tech_exposure + auth/e-commerce (IDOR/price tamper)
[PRIO] www.suedzuckergroup.com,score=6.5,axis=tech known (Drupal11), low gate (mostly 404/403)
[PRIO] suedzucker.mitarbeiterangebote.de,score=6.0,axis=auth (SSO/benefits, employee data)
[PRIO] plantportal.info,7.9,farmers+PII+contracts, custom auth/OTP flow, registration gated
[PRIO] app.agriconetwork.com,7.6,financial trading totals, custom app auth, high biz value
[PRIO] shop.suedzucker.com,7.2,e-commerce auth/IDOR/price, SPA, gate=login
[PRIO] suedzucker.mitarbeiterangebote.de,6.4,employee benefits, third-party SSO
[PRIO] bisz.suedzucker.de,5.8,agri info+PlantPortal entry, Drupal-ish, mostly public
[PRIO] www.suedzuckergroup.com,5.5,Drupal11 hardened, low attack surface
[HYP] Plant Portal partner-number linking IDOR/BOLA
class: IDOR
asset: plantportal.info
confidence: 55
reasoning: Flow doc (bodengesundheitsdienst.de PDF) shows linking to a 7-digit Partnernummer then SMS/post activation. Predictable numeric partner IDs + a "link existing partner account" function is a classic BOLA vector for cross-farmer data (contracts, deliveries, settlement). No live reach confirmed yet.
evidence_needed: Reach plantportal.info, observe /register + /partnerlink endpoints, test whether a linked partner's data is scoped by the session or by the supplied number.
verify_steps: PASSIVE-first: GET https://plantportal.info/ ; GET https://plantportal.info/robots.txt ; OPTIONS/GET likely JS SPA — confirm reach before any auth test. Active (auth-gated) would require own test account, not live customer data.
impact: cross-tenant access to farmer contract/delivery/settlement data (PII + financial) — HIGH.
testability: AUTH_HELPED
[HYP] agriconetwork byproduct-trading authorization bug
class: BUSLOGIC
asset: app.agriconetwork.com
confidence: 45
reasoning: Publicly documented as a trading platform where farmers set prices and counterparties buy pulp (Giełda Wysłodkowa). Money-flow + contract + SMS-confirm transactions implies high-value authorization/price logic. Currently transport-error (unreachable), so unverified.
evidence_needed: reach + enumerate API endpoints (/api, /graphql, swagger), map buy/sell endpoints and authorization model.
verify_steps: GET https://app.agriconetwork.com/ ; GET /robots.txt ; GET /api ; GET /.well-known/openid-configuration — read-only reach first.
impact: price manipulation / unauthorized transaction on real byproduct marketplace — HIGH (money).
testability: AUTH_HELPED
[HYP] shop.suedzucker.com e-commerce IDOR / price-tamper / weak basket logic
class: BUSLOGIC
asset: shop.suedzucker.com
confidence: 50
reasoning: Customer shop SPA with /login. e-commerce flows (basket, price, order, user profile) are prime IDOR/BUSLOGIC targets. Currently returns empty (heavily JS/anti-bot), so not yet reachable via simple fetch.
evidence_needed: reach shop SPA, identify API base (XHR), audit price/basket/profile endpoints for vertical/horizontal authz and server-side price validation.
verify_steps: GET https://shop.suedzucker.com/ ; GET /login ; identify JS bundle paths -> locate API host; read-only reach.
impact: order/price manipulation, cross-account order data — HIGH (money/auth).
testability: AUTH_HELPED
[PARKED] www.suedzuckergroup.com Drupal11 known-CVE: REJECTED class (outdated library w/o program-specific exploit) + site hardened (404/403 on release.txt, node/user, jsonapi, graphql).
[PARKED] bisz.suedzucker.de: public info portal, no auth-relevant surface confirmed; low value; drop confidence<40.
[PARKED] etracker secure-code kxgsS9 exposure: descriptive/headers-only class, REJECTED.
[FINAL] plantportal.info 55 (IDOR/BOLA, high data value)
[FINAL] shop.suedzucker.com 50 (BUSLOGIC e-commerce)
[FINAL] app.agriconetwork.com 45 (BUSLOGIC money)
[NEXT] PROBE: GET https://plantportal.info/ then /robots.txt and /.well-known/openid-configuration to map the farmer-portal tech + auth model (read-only reach scan).
[LEARN] REJECTED MISCONFIG @ www.suedzuckergroup.com: JSON:API+GraphQL disabled, registration closed, version files 404 — hardened Drupal; not a vuln.
[LEARN] REJECTED MISCONFIG @ www.suedzuckergroup.com: etracker secure-code in page source is a descriptive/tracking config, not in-scope impact.
[LEARN] ACCEPTED RECON @ suedzucker.de: root renamed to suedzuckergroup.com — passive surface analysis of old zone was targeting dead root; must re-enumerate new TLD.
[RISK] suedzucker: 68 — broad program (all company infra) newly hit a renamed corpus with several live subsidiary/partner portals (farmer PII, financial trading, e-commerce) that are reachable and not yet scoped in inventory; moderate carrying risk stays acceptable since all steps are read-only/GATE-gated and no live customer data is being touched.
## 2026-09-03 19:02:48 UTC [target] (model bigpickle)
## 2026-09-03 21:51:41 UTC [target] (model bigpickle)
[PRIO] plantportal.suedzuckergroup.com,8.3,axis=tech_exposure+gate — Nuxt SPA, MSAL Entra B2C, documented api-gateway backends (internal-auth + domain services), /association/impersonation route, partnerNo in watermark, switchToPartnerNumber query param
[PRIO] smartfarming.suedzuckergroup.com,8.0,axis=business_value+tech_exposure — public Swagger for full REST API (fields/actions/orders/media/org user-data), JWT token-gen-with-RSA documented, single-resource numeric-ID BOLA surface
[PRIO] shop.suedzucker.com,7.6,axis=tech_exposure — SFDC Commerce Cloud (managed infra limits exploitability but high value e-commerce auth)
[PRIO] bisz.suedzucker.de,5.5,axis=auth — now unreachable-ish (code=000), lower priority
[PRIO] app.agriconetwork.com,5.0,axis=business_value — still unreachable (code=000)
[HYP] MyDataPlant REST API BOLA via numeric single-resource IDs
class: IDOR
asset: smartfarming.suedzuckergroup.com/mdp-api/v3/api
confidence: 60
reasoning: Public Swagger documents GET/PATCH/DELETE by resource id for fields, actions, persons, vehicles, products, media, orderpositions, organizations, user-data/users. JSON:API single-resource reads by enumerate-able numeric/ULID ids on an org-scoped smart-farming backend are a canonical BOLA vector. Backend returns 400 (not 401) to bare requests, implying auth handled per-request rather than at edge. Auth is JWT ("token (JWT)" + "token generation with RSA signature" documented).
evidence_needed: Confirm a valid mdp_bgd_api JWT is required per-endpoint and whether GET by id is scoped to the token's organization vs cross-tenant (requires own test account; not live customer data).
verify_steps: Passive: GET https://smartfarming.suedzuckergroup.com/mdp-api/v3/api (already confirms Swagger public). Do NOT issue authed cross-tenant reads without an own test account.
impact: cross-tenant read/modify/delete of farm field data, orders, persons, media (agri PII + operations) — HIGH.
testability: AUTH_HELPED
[HYP] Plant Portal partner-number linking / impersonation BOLA
class: IDOR
asset: plantportal.suedzuckergroup.com
confidence: 58
reasoning: Nuxt route /partner-linking/:processPartnerNumber (integer) + ?switchToPartnerNumber=<int> query param (read into state and embedded in anti-screenshot watermark as partnerNo) + /association/impersonation guarded by only-for-partner middleware. The linking/impersonation flow binds an identity to a numeric partner number — predictable numeric IDs and an impersonation route are a systemic BOLA surface. Access token scopes: api://1b7819b0.../external_api_access.
evidence_needed: Whether supplied Parternummer/switchToPartnerNumber scopes data to session or lets one partner act on another's data (needs own test account).
verify_steps: Passive: confirmed routes in bundle + runtime config. Active only with own test account.
impact: cross-tenant access to farmer contract/delivery/settlement data + association impersonation — HIGH.
testability: AUTH_HELPED
[HYP] MyDataPlant export-to-configured-URL SSRF / server-side request
class: SSRF
asset: smartfarming.suedzuckergroup.com/mdp-api/v3/api
confidence: 40
reasoning: Swagger has endpoint "send export to configured URL" (GET) and "Send export to configured URL" where users can configure a target URL (also "user-settings .. url" POST). A server-side fetch to a user-controlled URL is a classic SSRF-to-internal/cloud-metadata vector. Confidence limited: no live confirmation of request behavior; auth-gated.
evidence_needed: Whether the configured URL is fetched server-side and allows internal/169.254.169.254 targets.
verify_steps: Passive-only now. Requires own test account + careful, non-destructive testing.
impact: SSRF to internal services / cloud metadata (169.254.169.254) -> possible credential exposure — HIGH.
testability: AUTH_HELPED
[NEXT] PROBE: GET https://smartfarming.suedzuckergroup.com/mdp-api/v3/api (already done — the public Swagger confirms full REST surface reachable without auth; next read-only step is to fetch the token-generation endpoint documentation to understand how mdp_bgd_api JWT is issued) — but strictly passive. Confirm auth before any active id-based read.
[LEARN] ACCEPTED RECON @ plantportal.suedzuckergroup.com: Nuxt "epp" app confirmed; MSAL Entra B2C (authority szgrmb2cprod.ciamlogin.com, clientId ba3120d6-3d54-478b-a048-5f1242196100), Bearer scopes api://1b7819b0.../external_api_access and api://aad3fee6.../mdp_bgd_api; runtime __NUXT__ config exposes api-gateway backend URIs (401 auth-gated) — all read-only exposure of public client config, not a vuln.
[LEARN] ACCEPTED RECON @ smartfarming.suedzuckergroup.com/mdp-api/v3/api: full MyDataPlant REST Swagger is publicly browsable (no auth required to read docs); reveals endpoint map + JWT token/RSA token-gen endpoints — recon value, public docs not itself a vuln.
[LEARN] ACCEPTED RECON @ shop.suedzucker.com: identified as Salesforce Commerce Cloud "sfdc communities"/DXP (SLDS, /sfsites/). Managed third-party infra; tenant-level findings hard to prove passively.
[LEARN] REJECTED NOT-VULN @ plantportal api-gateway endpoints: ceres-internal-auth-service / ceres-domain-backend-services / ceres-image-service all return 401 unauth (properly gated) — not a vuln.
[RISK] suedzucker: 64 — recon now focused on a live, renamed subsidiary/partner cluster (Plant Portal + MyDataPlant REST + SFCC shop). All steps were read-only (GET/HEAD of public docs and 401/302 reach probes, passive JS/Swagger analysis); no live customer data touched, no auth-bypass or mutating tests. Public Swagger and client config exposure raise the attack surface visibly but remain in-scope recon; carrying risk stays moderate and acceptable. Careful to keep all further Plant Portal/MyDataPlant steps on own test accounts only.
