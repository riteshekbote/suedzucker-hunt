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
