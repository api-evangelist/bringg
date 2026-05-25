# Bringg

Last-mile delivery and fulfillment orchestration platform. This repository profiles Bringg's developer surface as part of the [API Evangelist](https://apievangelist.com) catalog using the [APIs.json](https://apisjson.org) specification.

## Profile

- **Provider:** Bringg
- **Headquarters:** Tel Aviv, Israel (founded 2013)
- **CEO:** Guy Bloch
- **Scale:** 800+ customers, 200M annual deliveries, 70+ countries
- **Customers:** Best Buy, AutoZone, ASDA, Wegmans, FedEx Office, Metro, uBreakiFix, B&Q
- **Authentication:** OAuth 2.0 Client Credentials Grant
- **Regions:** US2, US3, US4, EU2, EU3 (all on GCP)
- **Status:** [status.bringg.com](https://status.bringg.com)
- **Developer Portal:** [developers.bringg.com](https://developers.bringg.com)
- **Knowledge Base:** [help.bringg.com](https://help.bringg.com)

## Platform Modules

| Module | Purpose |
| --- | --- |
| Shopping Experience | Checkout-time delivery options and dynamic slot selection |
| Plan | Fleet resource management and continuous route optimization |
| Dispatch | Single-pane order monitoring with exception handling |
| Drive | iOS and Android driver applications with configurable workflows |
| Delivery Experience | Customer-facing notifications, tracking, branded communication |
| Automation Center | No-code workflow automation |
| Intelligence | Dashboards, reporting, cost/profit/driver-performance insights |
| Connect | REST APIs, webhooks, and 250+ carrier integrations |

## APIs Profiled

| API | Purpose | OpenAPI |
| --- | --- | --- |
| Bringg Delivery Hub API | Orders, runs, customers, teams, service areas, service plans, delivery slots, blackouts, packages, inventory, analytics | [`openapi/bringg-delivery-hub-api-openapi.yml`](openapi/bringg-delivery-hub-api-openapi.yml) |
| Bringg Drivers And Shifts API | Users, shifts, real-time availability, delivery blocks, vehicles, vehicle profiles | [`openapi/bringg-drivers-shifts-api-openapi.yml`](openapi/bringg-drivers-shifts-api-openapi.yml) |
| Bringg Fleet Partners API | Integration surface for delivery providers / self-integrated fleets joining the Bringg Carrier Network | [`openapi/bringg-fleet-partners-api-openapi.yml`](openapi/bringg-fleet-partners-api-openapi.yml) |

## Webhook Events

Bringg emits 50+ outbound webhook event types covering the order, driver, run, customer, waypoint, and inventory lifecycle. See [`asyncapi/bringg-webhooks-asyncapi.yml`](asyncapi/bringg-webhooks-asyncapi.yml) for the channel-level inventory, and the [Bringg Webhooks Index](https://developers.bringg.com/reference/webhooks-index) for full payload reference.

## Artifacts

| Artifact | Path |
| --- | --- |
| APIs.json catalog | [`apis.yml`](apis.yml) |
| OpenAPI specs | [`openapi/`](openapi/) |
| AsyncAPI spec | [`asyncapi/`](asyncapi/) |
| JSON Schemas | [`json-schema/`](json-schema/) |
| JSON-LD context | [`json-ld/bringg-context.jsonld`](json-ld/bringg-context.jsonld) |
| JSON Structure | [`json-structure/`](json-structure/) |
| Examples | [`examples/`](examples/) |
| Spectral rules | [`rules/bringg-rules.yml`](rules/bringg-rules.yml) |
| Naftiko capabilities | [`capabilities/`](capabilities/) |
| Vocabulary | [`vocabulary/bringg-vocabulary.yml`](vocabulary/bringg-vocabulary.yml) |
| Plans | [`plans/bringg-plans-pricing.yml`](plans/bringg-plans-pricing.yml) |
| Rate limits | [`rate-limits/bringg-rate-limits.yml`](rate-limits/bringg-rate-limits.yml) |
| FinOps | [`finops/bringg-finops.yml`](finops/bringg-finops.yml) |

## Authentication

Bringg uses OAuth 2.0 Client Credentials Grant. Exchange your `client_id` / `client_secret` for an access token at:

```
POST https://admin-api.bringg.com/oauth/token   # or regional: us2-/us3-/us4-/eu2-/eu3-
```

Send the returned bearer token as `Authorization: Bearer <access_token>` on every API call. Default token TTLs are 30 minutes for write scopes and 4 hours for read scopes; the `ttl` parameter on the token request overrides this.

## License

Profile content is provided as-is by API Evangelist. Bringg trademarks, logos, and API access remain property of Bringg Inc. and are governed by the [Bringg API Terms of Service](https://developers.bringg.com/reference/terms-of-service).
