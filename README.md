# Judge.me (judge-me)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
