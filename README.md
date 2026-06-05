# Bringg (bringg)

Bringg is a last-mile delivery and fulfillment orchestration platform headquartered in Tel Aviv (founded 2013, CEO Guy Bloch). The Bringg platform combines modular software (Shopping Experience, Plan, Dispatch, Drive, Delivery Experience, Automation Center, Intelligence, Connect) with the Bringg Carrier Network — 250+ pre-integrated third-party, crowdsourced, and autonomous carriers across 70+ countries — to give enterprise retailers and logistics providers a single integration point for orchestrating own-fleet and partner-fleet deliveries. Bringg's developer surface exposes a REST Delivery Hub API for orders/runs/customers/teams/service areas/service plans/delivery slots/blackouts/inventory/packages, a Drivers & Shifts API for users/shifts/delivery-blocks/vehicles, a Fleet Partners API for self-integrated carriers, 50+ outbound webhook event types, and JavaScript/iOS/Android SDKs powering the Dispatcher and Driver apps. All HTTP APIs use OAuth 2.0 Client Credentials Grant against region-specific GCP base URLs (US2/US3/US4, EU2/EU3) — visible on status.bringg.com. Bringg counts 800+ customers including Best Buy, AutoZone, ASDA, Wegmans, FedEx Office, Metro, uBreakiFix, and B&Q, and processes 200 million annual deliveries.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Last-Mile Delivery
- Delivery Orchestration
- Fulfillment
- Logistics
- Retail
- Dispatch
- Routing
- Driver App
- Carrier Network
- Fleet Management
- Supply Chain
- E-commerce
- Same-Day Delivery
- Curbside Pickup
- Returns

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Bringg Delivery Hub API

Bringg's REST orchestration API for the Delivery Hub — create and manage orders (tasks), runs (routes), customers, teams, service areas, service plans, planned delivery windows (delivery slots), exclusion windows (blackouts), parking spots, packages, inventory, floating inventory, recurring orders, delivery blocks, vehicles, and analytics reports. All endpoints use OAuth 2.0 Client Credentials Grant against region-specific GCP base URLs (US2/US3/US4, EU2/EU3).

- **Human URL:** [https://developers.bringg.com/reference/welcome-to-bringgs-api-reference](https://developers.bringg.com/reference/welcome-to-bringgs-api-reference)
- **Base URL:** `https://us2-admin-api.bringg.com`

#### Tags

- Last-Mile Delivery
- Orders
- Dispatch
- Routing
- Service Areas
- Service Plans
- Quotes
- Inventory
- Analytics

#### Properties

- [Documentation](https://developers.bringg.com/reference/welcome-to-bringgs-api-reference)
- [Documentation](https://developers.bringg.com/docs/overview)
- [Documentation](https://developers.bringg.com/docs/rest)
- [Authentication](https://developers.bringg.com/docs/bringg-api-access-management)
- [Authentication](https://developers.bringg.com/docs/oauth-20-urls)
- [OpenAPI](openapi/bringg-delivery-hub-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bringg-delivery-hub-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bringg-delivery-hub-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bringg-order-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bringg-customer-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bringg-waypoint-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bringg-run-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/bringg-order-structure.json)
- [JSON-LD](json-ld/bringg-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/bringg-create-task-example.json)

### Bringg Drivers And Shifts API

Manage Bringg drivers, user roles, shifts, real-time availability, driver location updates, delivery blocks (shift slots), QR-code-based login, and vehicles with vehicle profiles. Backs the Bringg Driver App and dispatcher workflows; uses OAuth 2.0 Client Credentials Grant.

- **Human URL:** [https://developers.bringg.com/reference/driver-shifts](https://developers.bringg.com/reference/driver-shifts)
- **Base URL:** `https://us2-admin-api.bringg.com`

#### Tags

- Drivers
- Shifts
- Users
- Delivery Blocks
- Vehicles
- Fleet

#### Properties

- [Documentation](https://developers.bringg.com/reference/driver-shifts)
- [Documentation](https://developers.bringg.com/reference/users-3)
- [Documentation](https://developers.bringg.com/reference/vehicles)
- [Documentation](https://developers.bringg.com/reference/delivery-blocks)
- [OpenAPI](openapi/bringg-drivers-shifts-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bringg-drivers-shifts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bringg-drivers-shifts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bringg-driver-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Bringg Fleet Partners API

Integration surface for delivery providers and self-integrated fleets connecting to the Bringg Delivery Hub. Partners host webhook endpoints Bringg calls (Delivery Created, Get Quote, Delivery Updated, Delivery Cancelled, Merchant Registered, Return Delivery Created) and expose endpoints for order acceptance, status updates, driver location, and proof of delivery. Used by 250+ third-party carriers and crowdsourced fleets in the Bringg Carrier Network.

- **Human URL:** [https://developers.bringg.com/reference/overview-1](https://developers.bringg.com/reference/overview-1)
- **Base URL:** `https://app.bringg.com`

#### Tags

- Fleet Partners
- Self-Integrated Fleets
- Carrier Integration
- Quotes
- Webhooks

#### Properties

- [Documentation](https://developers.bringg.com/reference/overview-1)
- [Getting Started](https://developers.bringg.com/reference/how-to-get-started)
- [Documentation](https://developers.bringg.com/reference/getting-certified)
- [Documentation](https://developers.bringg.com/reference/how-to-conduct-and-end-to-end-test)
- [Documentation](https://developers.bringg.com/reference/webhooks)
- [Documentation](https://developers.bringg.com/reference/webhooks-index)
- [OpenAPI](openapi/bringg-fleet-partners-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bringg-fleet-partners-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bringg-fleet-partners-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/bringg-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

## Common Properties

- [Portal](https://www.bringg.com)
- [Documentation](https://developers.bringg.com)
- [Documentation](https://developers.bringg.com/reference/welcome-to-bringgs-api-reference)
- [Documentation](https://developers.bringg.com/v2.0/docs/overview)
- [Getting Started](https://developers.bringg.com/docs/overview)
- [Authentication](https://developers.bringg.com/docs/bringg-api-access-management)
- [Authentication](https://developers.bringg.com/docs/oauth-20-urls)
- [Errors](https://developers.bringg.com/docs/errors)
- [Webhooks](https://developers.bringg.com/docs/bringg-webhooks)
- [Webhooks](https://developers.bringg.com/reference/webhooks-index)
- [Documentation](https://developers.bringg.com/docs/webhook-authentication-methods)
- [Documentation](https://developers.bringg.com/docs/data-formatting)
- [Documentation](https://developers.bringg.com/docs/bringg-system-requirements)
- [Changelog](https://developers.bringg.com/reference/changelog)
- [Status Page](https://status.bringg.com)
- [Terms of Service](https://developers.bringg.com/reference/terms-of-service)
- [Knowledge Base](https://help.bringg.com)
- [Blog](https://www.bringg.com/resources/blog)
- [Portal](https://www.bringg.com/platform/)
- [Portal](https://www.bringg.com/carrier-network/)
- [Portal](https://www.bringg.com/about/)
- [SDK](https://developers.bringg.com/docs/dashboard-sdk-resources)
- [SDK](https://github.com/bringg/Bringg-iOS-DriverSDK)
- [GitHub Organization](https://github.com/bringg)
- [LinkedIn](https://www.linkedin.com/company/bringg)
- [Twitter](https://twitter.com/bringg)
- [Sign Up](https://www.bringg.com/contact-us/)
- [Plans](plans/bringg-plans-pricing.yml)
- [Rate Limits](rate-limits/bringg-rate-limits.yml)
- [Fin Ops](finops/bringg-finops.yml)
- [Features](undefined)
- [Modules](undefined)
- [Solutions](undefined)
- [Integrations](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
