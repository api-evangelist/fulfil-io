# Fulfil (fulfil-io)

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

Fulfil is a cloud ERP and operations platform for e-commerce, DTC, and wholesale merchants - unifying order management, inventory, warehouse operations (WMS), manufacturing and production (MRP), purchasing, and accounting in one system, purpose-built for Shopify Plus and high-volume DTC brands. The Fulfil REST API (v2) exposes every ERP resource through a single uniform "model interface" at `https://{merchant_id}.fulfil.io/api/v2`, advertising 6,000+ endpoints with full create/read/update/delete access, action calls, reports, and wizards across all models. Authentication is via OAuth 2.0 for public apps or personal access tokens (`X-API-KEY` / HTTP Basic) for private integrations, and outbound webhooks (with a Google Pub/Sub option) deliver real-time ERP events such as order and shipment changes.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/apis.yml)

## Tags

- ERP
- E-commerce
- Order Management
- Inventory
- Warehouse Management
- Manufacturing
- Operations

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

### Fulfil Sales Orders API

Create, search, read, update, and cancel sales orders through the `sale.sale` model - the customer, order lines, amounts, shipment and invoice state of every order captured from Shopify, marketplaces, or entered directly in Fulfil.

- **Human URL:** [https://developers.fulfil.io/](https://developers.fulfil.io/)
- **Base URL:** `https://{merchant_id}.fulfil.io/api/v2`

#### Tags

- Sales Orders
- Order Management
- E-commerce

#### Properties

- [Documentation](https://developers.fulfil.io/)
- [API Reference](https://fulfiliorestapi.docs.apiary.io/)
- [OpenAPI](openapi/fulfil-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fulfil-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fulfil-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fulfil Products & Variants API

Manage the product catalog through the `product.template` (product groupings) and `product.product` (individual sellable variants / SKUs) models - codes, barcodes, pricing, attributes, and their relationships.

- **Human URL:** [https://developers.fulfil.io/](https://developers.fulfil.io/)
- **Base URL:** `https://{merchant_id}.fulfil.io/api/v2`

#### Tags

- Products
- Variants
- Catalog

#### Properties

- [Documentation](https://developers.fulfil.io/)
- [API Reference](https://fulfiliorestapi.docs.apiary.io/)
- [OpenAPI](openapi/fulfil-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fulfil-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fulfil-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fulfil Inventory & Stock API

Read and record inventory through the `stock.move` (inventory movements) and `stock.location` (warehouses, zones, bins) models - on-hand quantities, transfers, adjustments, and stock levels by location.

- **Human URL:** [https://developers.fulfil.io/](https://developers.fulfil.io/)
- **Base URL:** `https://{merchant_id}.fulfil.io/api/v2`

#### Tags

- Inventory
- Stock
- Warehouse

#### Properties

- [Documentation](https://developers.fulfil.io/)
- [API Reference](https://fulfiliorestapi.docs.apiary.io/)
- [OpenAPI](openapi/fulfil-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fulfil-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fulfil-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fulfil Customers API

Manage customers, suppliers, and contacts through the `party.party` model - names, addresses, contact mechanisms (email, phone), and the relationships that link parties to sales and purchase orders.

- **Human URL:** [https://developers.fulfil.io/](https://developers.fulfil.io/)
- **Base URL:** `https://{merchant_id}.fulfil.io/api/v2`

#### Tags

- Customers
- Parties
- Contacts

#### Properties

- [Documentation](https://developers.fulfil.io/)
- [API Reference](https://fulfiliorestapi.docs.apiary.io/)
- [OpenAPI](openapi/fulfil-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fulfil-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fulfil-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fulfil Shipments API

Track and manage outbound and inbound shipments through the `stock.shipment.out` and `stock.shipment.in` models - fulfillment state, carrier and tracking data, and the moves that pick, pack, and ship customer orders.

- **Human URL:** [https://developers.fulfil.io/](https://developers.fulfil.io/)
- **Base URL:** `https://{merchant_id}.fulfil.io/api/v2`

#### Tags

- Shipments
- Fulfillment
- Logistics

#### Properties

- [Documentation](https://developers.fulfil.io/)
- [API Reference](https://fulfiliorestapi.docs.apiary.io/)
- [OpenAPI](openapi/fulfil-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fulfil-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fulfil-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fulfil Purchases API

Create and manage purchase orders through the `purchase.purchase` model - supplier, order lines, receipt and invoice state - to replenish inventory and supply manufacturing.

- **Human URL:** [https://developers.fulfil.io/](https://developers.fulfil.io/)
- **Base URL:** `https://{merchant_id}.fulfil.io/api/v2`

#### Tags

- Purchases
- Procurement
- Suppliers

#### Properties

- [Documentation](https://developers.fulfil.io/)
- [API Reference](https://fulfiliorestapi.docs.apiary.io/)
- [OpenAPI](openapi/fulfil-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fulfil-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fulfil-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fulfil Manufacturing API

Manage manufacturing through the `production` model - production orders, their inputs and outputs, bills of material, and the state transitions that turn raw materials into finished goods.

- **Human URL:** [https://docs.fulfil.io/production/](https://docs.fulfil.io/production/)
- **Base URL:** `https://{merchant_id}.fulfil.io/api/v2`

#### Tags

- Manufacturing
- Production
- MRP

#### Properties

- [Documentation](https://docs.fulfil.io/production/)
- [API Reference](https://fulfiliorestapi.docs.apiary.io/)
- [OpenAPI](openapi/fulfil-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fulfil-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fulfil-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fulfil Webhooks API

Register and manage webhook subscriptions so external systems receive real-time notifications when ERP events occur - orders created, inventory changes, shipments dispatched. Deliveries are HTTP POSTs signed with HMAC-SHA256; a Google Pub/Sub delivery option exists for high volume.

- **Human URL:** [https://www.fulfil.io/platform/api/](https://www.fulfil.io/platform/api/)
- **Base URL:** `https://{merchant_id}.fulfil.io/api/v2`

#### Tags

- Webhooks
- Events
- Real Time

#### Properties

- [Documentation](https://www.fulfil.io/platform/api/)
- [API Reference](https://fulfiliorestapi.docs.apiary.io/)
- [OpenAPI](openapi/fulfil-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fulfil-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fulfil-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fulfil Model Interface API

The uniform model interface that underlies every Fulfil resource - generic CRUD (`GET`/`POST` `/model/{model.name}`, `GET`/`PUT`/`DELETE` `/model/{model.name}/{id}`), `search_read`, `count`, arbitrary method (action) calls, reports, and wizards - plus the `/test` credential-check endpoint. Any of Fulfil's models can be driven through it.

- **Human URL:** [https://developers.fulfil.io/](https://developers.fulfil.io/)
- **Base URL:** `https://{merchant_id}.fulfil.io/api/v2`

#### Tags

- Model Interface
- CRUD
- Reports

#### Properties

- [Documentation](https://developers.fulfil.io/)
- [API Reference](https://fulfiliorestapi.docs.apiary.io/)
- [OpenAPI](openapi/fulfil-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fulfil-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fulfil-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/fulfilio)
- [LinkedIn](https://www.linkedin.com/company/fulfil-io)
- [Website](https://www.fulfil.io)
- [Documentation](https://developers.fulfil.io/)
- [Plans](plans/fulfil-io-plans-pricing.yml)
- [Rate Limits](rate-limits/fulfil-io-rate-limits.yml)
- [Fin Ops](finops/fulfil-io-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
