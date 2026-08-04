# Donorbox (donorbox)

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

Donorbox is an online donation and fundraising platform for nonprofits, offering branded donation forms, recurring giving, peer-to-peer campaigns, event ticketing, memberships, and text-to-give. Its REST API (an add-on available on Pro and Premium plans) exposes read-only access to Campaigns, Donations, Plans (recurring donation subscriptions), Donors, Events, Tickets, and Ticket Purchases, authenticated with HTTP Basic Auth using an organization email and API key, with custom webhooks available as an alternative to polling.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/apis.yml)

## Tags

- Nonprofit
- Fundraising
- Donations
- Payments
- Recurring Giving
- Event Ticketing

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Donorbox Campaigns API

Read-only access to an organization's fundraising campaigns - id, name, slug, currency, goal amount, total raised, and donation count. Filterable by campaign id or name.

- **Human URL:** [https://github.com/donorbox/donorbox-api/blob/master/README.md#campaigns](https://github.com/donorbox/donorbox-api/blob/master/README.md#campaigns)
- **Base URL:** `https://donorbox.org/api/v1`

#### Tags

- Campaigns
- Fundraising

#### Properties

- [Documentation](https://github.com/donorbox/donorbox-api/wiki)
- [API Reference](https://github.com/donorbox/donorbox-api/blob/master/README.md#campaigns)
- [OpenAPI](openapi/donorbox-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/donorbox.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/donorbox.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Donorbox Donations API

Read-only access to an organization's donations, including campaign, donor, amount, currency, status, donation type (Stripe or PayPal), UTM attribution, processing fee, and custom question/answer fields collected on the donation form. Filterable by email, donor, campaign, id, date range, and amount range.

- **Human URL:** [https://github.com/donorbox/donorbox-api/blob/master/README.md#donations](https://github.com/donorbox/donorbox-api/blob/master/README.md#donations)
- **Base URL:** `https://donorbox.org/api/v1`

#### Tags

- Donations
- Payments
- Stripe
- PayPal

#### Properties

- [Documentation](https://github.com/donorbox/donorbox-api/wiki)
- [API Reference](https://github.com/donorbox/donorbox-api/blob/master/README.md#donations)
- [OpenAPI](openapi/donorbox-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/donorbox.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/donorbox.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Donorbox Plans API

Read-only access to recurring donation plans/subscriptions - donor, campaign, plan type (monthly, weekly, etc.), amount, payment method, start date, last/next donation date, and status. Filterable by donor email/id/name, campaign, and start date range.

- **Human URL:** [https://github.com/donorbox/donorbox-api/blob/master/README.md#plans](https://github.com/donorbox/donorbox-api/blob/master/README.md#plans)
- **Base URL:** `https://donorbox.org/api/v1`

#### Tags

- Recurring Donations
- Subscriptions
- Plans

#### Properties

- [Documentation](https://github.com/donorbox/donorbox-api/wiki)
- [API Reference](https://github.com/donorbox/donorbox-api/blob/master/README.md#plans)
- [OpenAPI](openapi/donorbox-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Donorbox Donors API

Read-only access to donor profiles - contact info, address, donation count, last donation date, and lifetime total by currency. Filterable by donor id, name, and email.

- **Human URL:** [https://github.com/donorbox/donorbox-api/blob/master/README.md#donors](https://github.com/donorbox/donorbox-api/blob/master/README.md#donors)
- **Base URL:** `https://donorbox.org/api/v1`

#### Tags

- Donors
- CRM

#### Properties

- [Documentation](https://github.com/donorbox/donorbox-api/wiki)
- [API Reference](https://github.com/donorbox/donorbox-api/blob/master/README.md#donors)
- [OpenAPI](openapi/donorbox-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Donorbox Events API

Read-only access to ticketed fundraising events - id, name, slug, currency, total raised, donation count, and ticket count.

- **Human URL:** [https://github.com/donorbox/donorbox-api/blob/master/README.md#events](https://github.com/donorbox/donorbox-api/blob/master/README.md#events)
- **Base URL:** `https://donorbox.org/api/v1`

#### Tags

- Events
- Ticketing

#### Properties

- [Documentation](https://github.com/donorbox/donorbox-api/wiki)
- [API Reference](https://github.com/donorbox/donorbox-api/blob/master/README.md#events)
- [OpenAPI](openapi/donorbox-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Donorbox Tickets API

Read-only access to individual event tickets - price, ticket type (name, fair market value, tax-deductible amount), the parent event, and the associated purchase transaction. Filterable by payment status (e.g. refunded).

- **Human URL:** [https://github.com/donorbox/donorbox-api/blob/master/README.md#tickets](https://github.com/donorbox/donorbox-api/blob/master/README.md#tickets)
- **Base URL:** `https://donorbox.org/api/v1`

#### Tags

- Tickets
- Events
- Ticketing

#### Properties

- [Documentation](https://github.com/donorbox/donorbox-api/wiki)
- [API Reference](https://github.com/donorbox/donorbox-api/blob/master/README.md#tickets)
- [OpenAPI](openapi/donorbox-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Donorbox Event Ticket Purchases API

Read-only access to event ticket purchase transactions - the purchasing supporter, amount, refund amount, status, and the bundle of tickets bought in that transaction. Filterable by payment status (succeeded, pending, failed, refunded).

- **Human URL:** [https://github.com/donorbox/donorbox-api/blob/master/README.md#event-ticket-purchases](https://github.com/donorbox/donorbox-api/blob/master/README.md#event-ticket-purchases)
- **Base URL:** `https://donorbox.org/api/v1`

#### Tags

- Purchases
- Events
- Ticketing

#### Properties

- [Documentation](https://github.com/donorbox/donorbox-api/wiki)
- [API Reference](https://github.com/donorbox/donorbox-api/blob/master/README.md#event-ticket-purchases)
- [OpenAPI](openapi/donorbox-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [GitHub Organization](https://github.com/donorbox)
- [LinkedIn](https://www.linkedin.com/company/donorbox)
- [Website](https://donorbox.org)
- [Documentation](https://github.com/donorbox/donorbox-api/wiki)
- [Plans](plans/donorbox-plans-pricing.yml)
- [Rate Limits](rate-limits/donorbox-rate-limits.yml)
- [Fin Ops](finops/donorbox-finops.yml)

## Notes

- Donorbox's API is entirely GET/read-only - there is no documented way to create donations, campaigns, or donors via the API. Writes into Donorbox happen through the hosted donation form/checkout flow, not the API.
- All endpoints share `https://donorbox.org/api/v1` as the base URL, are authenticated with HTTP Basic Auth (organization login email as username, API key as password), and support common `page`/`per_page` pagination (default 50, max 100) and `order=asc|desc` (default `desc`).
- Donorbox also documents a custom webhook mechanism (part of the same API & Zapier add-on) as an alternative to polling; it delivers a JSON payload via HTTP POST to a configured endpoint URL rather than exposing a WebSocket. See `review.yml`.
- The official machine-readable source for endpoint/field definitions is the `donorbox/donorbox-api` GitHub repository README and wiki, not a published OpenAPI or Postman file from Donorbox itself - `openapi/donorbox-openapi.yml` and the two collections in this repo were modeled from that README by API Evangelist.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
