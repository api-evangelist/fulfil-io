# Fulfil (fulfil-io)

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
