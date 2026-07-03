# Donorbox (donorbox)

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
