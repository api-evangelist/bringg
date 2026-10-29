# Bringg

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Bringg is a last-mile delivery and fulfillment orchestration platform headquartered in Tel Aviv (founded 2013, CEO Guy Bloch). The Bringg platform combines modular software (Shopping Experience, Plan, Dispatch, Drive, Delivery Experience, Automation Center, Intelligence, Connect) with the Bringg Carrier Network — 250+ pre-integrated third-party, crowdsourced, and autonomous carriers across 70+ countries — to give enterprise retailers and logistics providers a single integration point for orchestrating own-fleet and partner-fleet deliveries. Bringg's developer surface exposes a REST Delivery Hub API for orders/runs/customers/teams/service areas/service plans/delivery slots/blackouts/inventory/packages, a Drivers & Shifts API for users/shifts/delivery-blocks/vehicles, a Fleet Partners API for self-integrated carriers, 50+ outbound webhook event types, and JavaScript/iOS/Android SDKs powering the Dispatcher and Driver apps. All HTTP APIs use OAuth 2.0 Client Credentials Grant against region-specific GCP base URLs (US2/US3/US4, EU2/EU3) — visible on status.bringg.com. Bringg counts 800+ customers including Best Buy, AutoZone, ASDA, Wegmans, FedEx Office, Metro, uBreakiFix, and B&Q, and processes 200 million annual deliveries.

**Areas:** Last Mile Delivery · Delivery Orchestration · Fulfillment · Logistics · Retail · Dispatch · Routing · Driver App · Carrier Network · Fleet Management · Supply Chain · E-Commerce

## Bringg on APIs.io

Everything profiled for Bringg is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/bringg/](https://apis.io/providers/bringg/)** — or go straight to one of the APIs or properties below.

### APIs (30)

- [Bringg Administration API](https://apis.io/apis/bringg/bringg-administration-api/) — The Administration API from Bringg — 1 operation(s) for administration.
- [Bringg Analytics API](https://apis.io/apis/bringg/bringg-analytics-api/) — The Analytics API from Bringg — 2 operation(s) for analytics.
- [Bringg Authentication API](https://apis.io/apis/bringg/bringg-authentication-api/) — The Authentication API from Bringg — 2 operation(s) for authentication.
- [Bringg Blackouts API](https://apis.io/apis/bringg/bringg-blackouts-api/) — The Blackouts API from Bringg — 4 operation(s) for blackouts.
- [Bringg Bulk API](https://apis.io/apis/bringg/bringg-bulk-api/) — The Bulk API from Bringg — 3 operation(s) for bulk.
- [Bringg Customers API](https://apis.io/apis/bringg/bringg-customers-api/) — The Customers API from Bringg — 5 operation(s) for customers.
- [Bringg Delivery Blocks API](https://apis.io/apis/bringg/bringg-delivery-blocks-api/) — The Delivery Blocks API from Bringg — 8 operation(s) for delivery blocks.
- [Bringg Delivery Slots API](https://apis.io/apis/bringg/bringg-delivery-slots-api/) — The Delivery Slots API from Bringg — 2 operation(s) for delivery slots.
- [Bringg Drivers API](https://apis.io/apis/bringg/bringg-drivers-api/) — The Drivers API from Bringg — 15 operation(s) for drivers.
- [Bringg Floating Inventory API](https://apis.io/apis/bringg/bringg-floating-inventory-api/) — The Floating Inventory API from Bringg — 4 operation(s) for floating inventory.
- [Bringg Inventory API](https://apis.io/apis/bringg/bringg-inventory-api/) — The Inventory API from Bringg — 2 operation(s) for inventory.
- [Bringg Notes API](https://apis.io/apis/bringg/bringg-notes-api/) — The Notes API from Bringg — 3 operation(s) for notes.
- [Bringg Operations API](https://apis.io/apis/bringg/bringg-operations-api/) — The Operations API from Bringg — 1 operation(s) for operations.
- [Bringg Order Configurations API](https://apis.io/apis/bringg/bringg-order-configurations-api/) — The Order Configurations API from Bringg — 2 operation(s) for order configurations.
- [Bringg Orders API](https://apis.io/apis/bringg/bringg-orders-api/) — The Orders API from Bringg — 22 operation(s) for orders.
- [Bringg Packages API](https://apis.io/apis/bringg/bringg-packages-api/) — The Packages API from Bringg — 6 operation(s) for packages.
- [Bringg Parking Spots API](https://apis.io/apis/bringg/bringg-parking-spots-api/) — The Parking Spots API from Bringg — 5 operation(s) for parking spots.
- [Bringg Planned Routes API](https://apis.io/apis/bringg/bringg-planned-routes-api/) — The Planned Routes API from Bringg — 2 operation(s) for planned routes.
- [Bringg Quotes API](https://apis.io/apis/bringg/bringg-quotes-api/) — The Quotes API from Bringg — 1 operation(s) for quotes.
- [Bringg Recurring Orders API](https://apis.io/apis/bringg/bringg-recurring-orders-api/) — The Recurring Orders API from Bringg — 3 operation(s) for recurring orders.
- [Bringg Routes API](https://apis.io/apis/bringg/bringg-routes-api/) — The Routes API from Bringg — 4 operation(s) for routes.
- [Bringg Service Areas API](https://apis.io/apis/bringg/bringg-service-areas-api/) — The Service Areas API from Bringg — 8 operation(s) for service areas.
- [Bringg Service Plans API](https://apis.io/apis/bringg/bringg-service-plans-api/) — The Service Plans API from Bringg — 4 operation(s) for service plans.
- [Bringg Shifts API](https://apis.io/apis/bringg/bringg-shifts-api/) — The Shifts API from Bringg — 2 operation(s) for shifts.
- [Bringg Teams API](https://apis.io/apis/bringg/bringg-teams-api/) — The Teams API from Bringg — 8 operation(s) for teams.
- [Bringg Users API](https://apis.io/apis/bringg/bringg-users-api/) — The Users API from Bringg — 6 operation(s) for users.
- [Bringg Vehicle Profiles API](https://apis.io/apis/bringg/bringg-vehicle-profiles-api/) — The Vehicle Profiles API from Bringg — 5 operation(s) for vehicle profiles.
- [Bringg Vehicles API](https://apis.io/apis/bringg/bringg-vehicles-api/) — The Vehicles API from Bringg — 8 operation(s) for vehicles.
- [Bringg Waypoints API](https://apis.io/apis/bringg/bringg-waypoints-api/) — The Waypoints API from Bringg — 6 operation(s) for waypoints.
- [Bringg Webhooks API](https://apis.io/apis/bringg/bringg-webhooks-api/) — The Webhooks API from Bringg — 7 operation(s) for webhooks.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Bringg Webhooks](https://apis.io/asyncapis/bringg/bringg-webhooks-asyncapi/)

#### Event channels (45)

Individual events and webhooks the provider emits.

- [alert.new](https://apis.io/channels/bringg/alert-new/)
- [customer.created](https://apis.io/channels/bringg/customer-created/)
- [customer.opted_in_to_sms](https://apis.io/channels/bringg/customer-opted-in-to-sms/)
- [customer.opted_out_of_sms](https://apis.io/channels/bringg/customer-opted-out-of-sms/)
- [customer.tipped_driver](https://apis.io/channels/bringg/customer-tipped-driver/)
- [delivery.created](https://apis.io/channels/bringg/delivery-created/)
- [driver.arrived_on_location](https://apis.io/channels/bringg/driver-arrived-on-location/)
- [driver.changed_type](https://apis.io/channels/bringg/driver-changed-type/)
- [driver.got_home](https://apis.io/channels/bringg/driver-got-home/)
- [driver.left_home](https://apis.io/channels/bringg/driver-left-home/)
- [driver.location_updated](https://apis.io/channels/bringg/driver-location-updated/)
- [driver.on_way](https://apis.io/channels/bringg/driver-on-way/)
- [driver.unavailable_status_changed](https://apis.io/channels/bringg/driver-unavailable-status-changed/)
- [inventory.scanned](https://apis.io/channels/bringg/inventory-scanned/)
- [masked_call](https://apis.io/channels/bringg/masked-call/)
- [optimization.applied](https://apis.io/channels/bringg/optimization-applied/)
- [order.accepted_by_driver](https://apis.io/channels/bringg/order-accepted-by-driver/)
- [order.accepted_by_fleet](https://apis.io/channels/bringg/order-accepted-by-fleet/)
- [order.assigned_to_dp](https://apis.io/channels/bringg/order-assigned-to-dp/)
- [order.assigned_to_driver](https://apis.io/channels/bringg/order-assigned-to-driver/)
- [order.cancelled](https://apis.io/channels/bringg/order-cancelled/)
- [order.created](https://apis.io/channels/bringg/order-created/)
- [order.eta_changed](https://apis.io/channels/bringg/order-eta-changed/)
- [order.is_done](https://apis.io/channels/bringg/order-is-done/)
- [order.marked_late](https://apis.io/channels/bringg/order-marked-late/)
- …and 20 more published on APIs.io

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/bringg/](https://apis.io/graphqls/bringg/bringg-graphql/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Bringg Agentic Access](https://apis.io/agentic-access/bringg/bringg-agentic-access/)

#### JSON Schema (5)

The data models the API reads and writes.

- [Bringg Customer](https://apis.io/schemas/bringg/bringg-customer/)
- [Bringg Driver (User)](https://apis.io/schemas/bringg/bringg-driver/)
- [Bringg Order (Task)](https://apis.io/schemas/bringg/bringg-order/)
- [Bringg Run (Route)](https://apis.io/schemas/bringg/bringg-run/)
- [Bringg Waypoint](https://apis.io/schemas/bringg/bringg-waypoint/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Bringg Order Structure](https://apis.io/json-structure/bringg/bringg-order-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Bringg Context](https://apis.io/jsonld/bringg/bringg-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Bringg Vocabulary](https://apis.io/vocabularies/bringg/bringg-vocabulary/)

#### Examples (1)

Example requests and responses.

- [Bringg Create Task Example](https://apis.io/examples/bringg/bringg-create-task-example/)

#### Collections (63)

Postman and Open Collection request collections.

- [Bringg Delivery Hub Administration API](https://apis.io/collections/bringg/open-bringg-administration-api/)
- [Bringg Delivery Hub Administration Analytics API](https://apis.io/collections/bringg/open-bringg-analytics-api/)
- [Bringg Delivery Hub Administration Authentication API](https://apis.io/collections/bringg/open-bringg-authentication-api/)
- [Bringg Delivery Hub Administration Blackouts API](https://apis.io/collections/bringg/open-bringg-blackouts-api/)
- [Bringg Delivery Hub Administration Bulk API](https://apis.io/collections/bringg/open-bringg-bulk-api/)
- [Bringg Delivery Hub Administration Customers API](https://apis.io/collections/bringg/open-bringg-customers-api/)
- [Bringg Delivery Hub Administration Delivery Blocks API](https://apis.io/collections/bringg/open-bringg-delivery-blocks-api/)
- [Bringg Delivery Hub API](https://apis.io/collections/bringg/open-bringg-delivery-hub-api/)
- [Bringg Delivery Hub Administration Delivery Slots API](https://apis.io/collections/bringg/open-bringg-delivery-slots-api/)
- [Bringg Delivery Hub Administration Drivers API](https://apis.io/collections/bringg/open-bringg-drivers-api/)
- [Bringg Drivers and Shifts API](https://apis.io/collections/bringg/open-bringg-drivers-shifts-api/)
- [Bringg Fleet Partners (Self-Integrated Fleets) API](https://apis.io/collections/bringg/open-bringg-fleet-partners-api/)
- [Bringg Delivery Hub Administration Floating Inventory API](https://apis.io/collections/bringg/open-bringg-floating-inventory-api/)
- [Bringg Delivery Hub Administration Inventory API](https://apis.io/collections/bringg/open-bringg-inventory-api/)
- [Bringg Delivery Hub Administration Notes API](https://apis.io/collections/bringg/open-bringg-notes-api/)
- [Bringg Delivery Hub Administration Operations API](https://apis.io/collections/bringg/open-bringg-operations-api/)
- [Bringg Delivery Hub Administration Order Configurations API](https://apis.io/collections/bringg/open-bringg-order-configurations-api/)
- [Bringg Delivery Hub Administration Orders API](https://apis.io/collections/bringg/open-bringg-orders-api/)
- [Bringg Delivery Hub Administration Packages API](https://apis.io/collections/bringg/open-bringg-packages-api/)
- [Bringg Delivery Hub Administration Parking Spots API](https://apis.io/collections/bringg/open-bringg-parking-spots-api/)
- [Bringg Delivery Hub Administration Planned Routes API](https://apis.io/collections/bringg/open-bringg-planned-routes-api/)
- [Bringg Delivery Hub Administration Quotes API](https://apis.io/collections/bringg/open-bringg-quotes-api/)
- [Bringg Delivery Hub Administration Recurring Orders API](https://apis.io/collections/bringg/open-bringg-recurring-orders-api/)
- [Bringg Delivery Hub Administration Routes API](https://apis.io/collections/bringg/open-bringg-routes-api/)
- [Bringg Delivery Hub Administration Service Areas API](https://apis.io/collections/bringg/open-bringg-service-areas-api/)
- …and 38 more published on APIs.io

#### Governance rules (3)

Spectral rulesets for the provider's contracts.

- [Bringg — asyncapi rules](https://apis.io/rules/bringg/bringg-asyncapi-spectral-rules/)
- [Bringg — jsonschema rules](https://apis.io/rules/bringg/bringg-jsonschema-spectral-rules/)
- [Bringg API Rules](https://apis.io/rules/bringg/bringg-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Bringg Authentication](https://apis.io/security/bringg/bringg-authentication/)
- [Bringg Domain Security](https://apis.io/security/bringg/bringg-domain-security/)
- [Bringg Trust Center](https://apis.io/security/bringg/bringg-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Bringg Scopes](https://apis.io/scopes/bringg/bringg-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Bringg Plans Pricing](https://apis.io/plans/bringg/bringg-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Bringg Rate Limits](https://apis.io/rate-limits/bringg/bringg-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Bringg Finops](https://apis.io/finops/bringg/bringg-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.bringg.com/)
- [Documentation](https://developers.bringg.com)
- [Getting started](https://developers.bringg.com/docs/overview)
- [Changelog](https://developers.bringg.com/reference/changelog)
- [Blog](https://www.bringg.com/resources/blog)
- [Terms of service](https://developers.bringg.com/reference/terms-of-service)
- [GitHub](https://github.com/bringg)
- [Status](https://status.bringg.com)

## API Evangelist rating

**Kin Score 48.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 69.8 |
| Contract governance | 13.6 |
| Operational transparency | 38.2 |
| Developer ergonomics | 36.9 |
| Access clarity | 31.6 |

**Agent readiness 28.2** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | mostly |

**Regulatory alignment 34.2** — Telecommunications

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/bringg/](https://apis.io/providers/bringg/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Bringg: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/bringg/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
