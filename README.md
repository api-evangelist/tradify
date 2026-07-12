# Tradify (tradify)

> **Access model up front:** As of this review (2026-07-12), **Tradify does not
> publish an open, self-serve, documented public developer API.** There is no
> public developer portal, no self-service API keys, and no documented webhooks.
> Tradify's *supported* programmatic surface is limited to pre-built accounting
> and payment **partner integrations** — Xero, MYOB Business, QuickBooks Online,
> Sage, and Stripe. A live application backend host (`api.tradifyhq.com`) exists
> and responds over HTTPS, but it is **undocumented, session-authenticated, and
> reserved for Tradify's own web and mobile apps** — not a public API. Third
> parties access Tradify data through the partner integrations, or through
> **unofficial** proxies that automate the authenticated user session. **Every
> API entry in this catalog record is MODELED** from Tradify's product
> capabilities, clearly flagged, and is *not* confirmed against official public
> API documentation.

Tradify is all-in-one job management software for trade and service businesses —
electricians, plumbers, HVAC technicians, builders, and other contractors. It
covers enquiries, quotes, jobs, scheduling and dispatch, timesheets, purchase
orders, and invoicing from web and mobile apps. Tradify is an Access company.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/apis.yml)

## Tags

- Job Management
- Trades
- Field Service
- Scheduling
- Quoting
- Invoicing
- Timesheets
- Contractors
- SaaS

## Timestamps

- **Created:** 2026-07-12
- **Modified:** 2026-07-12

## APIs (Modeled)

The following entries model the resource surface Tradify manages. They are
**inferred from product capabilities and are not backed by official public API
documentation**. No public base URL is published; the OpenAPI specification below
is intentionally server-less and every operation is marked `x-status: modeled`.

### Tradify Jobs API (Modeled)

Create, list, retrieve, update, and status jobs with linked customers, sites,
notes, and attachments.

- **Human URL:** [https://www.tradifyhq.com/how-it-works](https://www.tradifyhq.com/how-it-works)

#### Properties

- [Documentation](https://www.tradifyhq.com/how-it-works)
- [OpenAPI](openapi/tradify-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tradify.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tradify.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tradify Customers API (Modeled)

Create, list, retrieve, and update customers / contacts and their job sites.

- **Human URL:** [https://help.tradifyhq.com/hc/en-us](https://help.tradifyhq.com/hc/en-us)

### Tradify Quotes API (Modeled)

Build quotes / estimates from templates, pricelists, and material kits.

- **Human URL:** [https://www.tradifyhq.com/how-it-works](https://www.tradifyhq.com/how-it-works)

### Tradify Invoices API (Modeled)

Generate invoices from jobs, quotes, or templates. In practice, invoice sync to
accounting systems is delivered through Tradify's **Xero / MYOB / QuickBooks /
Sage** partner integrations rather than a public invoices API.

- **Human URL:** [https://help.tradifyhq.com/hc/en-us/articles/21124135640473-Create-an-Invoice-from-a-Job-Quote-or-Template](https://help.tradifyhq.com/hc/en-us/articles/21124135640473-Create-an-Invoice-from-a-Job-Quote-or-Template)

### Tradify Timesheets API (Modeled)

Capture and retrieve time entries logged against jobs from the mobile app.

- **Human URL:** [https://www.tradifyhq.com/how-it-works](https://www.tradifyhq.com/how-it-works)

## Common Properties

- [Domain Security](security/tradify-domain-security.yml)
- [Authentication](authentication/tradify-authentication.yml)
- [GitHub Organization](https://github.com/Tradify-App)
- [LinkedIn](https://www.linkedin.com/company/tradify)
- [Website](https://www.tradifyhq.com)
- [Documentation / Help Centre](https://help.tradifyhq.com/hc/en-us)
- [Plans](plans/tradify-plans-pricing.yml)
- [Rate Limits](rate-limits/tradify-rate-limits.yml)
- [Fin Ops](finops/tradify-finops.yml)

## WebSocket Review

**Does Tradify expose a documented public WebSocket API?** **No.** Tradify does
not publish any documented public API at all, so there is no documented public
WebSocket (`wss://`) surface. See [`review.yml`](review.yml). No AsyncAPI
document was authored.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
