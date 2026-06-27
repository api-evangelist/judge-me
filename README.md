# Judge.me (judge-me)

Judge.me is a product reviews platform for Shopify and other e-commerce storefronts, collecting photo and video reviews, star ratings, site reviews, and Q&A. The Judge.me REST API at https://judge.me/api/v1 lets developers list and import reviews, fetch ready-to-render widget HTML, resolve products, send review requests, and build OAuth apps authenticated with a shop_domain plus public or private api_token.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/apis.yml)

## Tags

- Reviews
- E-commerce
- Shopify
- Ratings
- Social Proof

## Timestamps

- **Created:** 2026-06-25
- **Modified:** 2026-06-25

## APIs

### Judge.me Reviews API

List published reviews with pagination and filtering for bulk export, and programmatically create reviews with a reviewer name, email, rating, title, and body against a product or the store, using a private api_token and shop_domain.

- **Human URL:** [https://judge.me/api/docs](https://judge.me/api/docs)
- **Base URL:** `https://judge.me/api/v1`

#### Tags

- Reviews
- Ratings
- Import

#### Properties

- [Documentation](https://judge.me/help/en/articles/8409180-using-judge-me-api)
- [API Reference](https://judge.me/api/docs)
- [OpenAPI](openapi/judge-me-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/judge-me.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/judge-me.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Judge.me Reviewers API

Reviewer data - the customers who have left reviews, including name, email, and external id - is returned inline on review records and gated by the read_reviewers and write_reviewers OAuth scopes for apps syncing contacts into an external system.

- **Human URL:** [https://judge.me/api/docs](https://judge.me/api/docs)
- **Base URL:** `https://judge.me/api/v1`

#### Tags

- Reviewers
- Customers

#### Properties

- [Documentation](https://judge.me/help/en/articles/8409180-using-judge-me-api)
- [OpenAPI](openapi/judge-me-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/judge-me.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/judge-me.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Judge.me Products API

Resolve products by converting an external (platform) product handle or id into an internal Judge.me product id via the /products/-1 lookup, the same id used to scope review queries to a single product.

- **Human URL:** [https://judge.me/api/docs](https://judge.me/api/docs)
- **Base URL:** `https://judge.me/api/v1`

#### Tags

- Products
- Mapping

#### Properties

- [Documentation](https://judge.me/help/en/articles/8409180-using-judge-me-api)
- [OpenAPI](openapi/judge-me-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/judge-me.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/judge-me.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Judge.me Widgets API

Return sanitized, XSS-safe, ready-to-render review widget HTML - such as the product review widget and the preview badge showing average star rating and review count - usable from public JavaScript environments with a public api_token.

- **Human URL:** [https://judge.me/api/docs](https://judge.me/api/docs)
- **Base URL:** `https://judge.me/api/v1`

#### Tags

- Widgets
- HTML
- Display

#### Properties

- [Documentation](https://judge.me/help/en/articles/8409180-using-judge-me-api)
- [OpenAPI](openapi/judge-me-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/judge-me.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/judge-me.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Judge.me OAuth API

Standard OAuth 2.0 authorization-code flow at app.judge.me/oauth/authorize and judge.me/oauth/token letting third-party apps request scoped access (read/write shops, widgets, orders, products, reviewers, reviews, settings) on behalf of a Judge.me store.

- **Human URL:** [https://judge.me/help/en/articles/8283047-setting-up-oauth](https://judge.me/help/en/articles/8283047-setting-up-oauth)
- **Base URL:** `https://judge.me/oauth`

#### Tags

- OAuth
- Authentication
- Authorization

#### Properties

- [Documentation](https://judge.me/help/en/articles/8283047-setting-up-oauth)
- [OpenAPI](openapi/judge-me-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/judge-me.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/judge-me.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Judge.me Webhooks API

Subscribe to events so Judge.me POSTs to your URL on review lifecycle events - review/created, review/updated, review/published, review/unpublished - and widget settings updates, with an HMAC signature you can verify on receipt.

- **Human URL:** [https://judge.me/api/docs](https://judge.me/api/docs)
- **Base URL:** `https://judge.me/api/v1`

#### Tags

- Webhooks
- Events

#### Properties

- [Documentation](https://judge.me/help/en/articles/8278390-build-integrations-with-judge-me)
- [API Reference](https://judge.me/help/en/articles/8299679-verifying-webhooks-from-judge-me)
- [OpenAPI](openapi/judge-me-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/judge-me.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/judge-me.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/judge-me)
- [Website](https://judge.me/)
- [Documentation](https://judge.me/api/docs)
- [Plans](plans/judge-me-plans-pricing.yml)
- [Rate Limits](rate-limits/judge-me-rate-limits.yml)
- [Fin Ops](finops/judge-me-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
