# Bringg GraphQL Schema

Conceptual GraphQL schema for the [Bringg Delivery Hub API](https://developers.bringg.com/reference/welcome-to-bringgs-api-reference), derived from Bringg's REST API surface: the Delivery Hub API, Drivers & Shifts API, and Fleet Partners API.

## Overview

Bringg is a last-mile delivery orchestration platform serving enterprise retailers and logistics providers. It exposes REST APIs for orders, runs (routes), drivers, vehicles, service areas, fleets, inventory, and webhooks — all authenticated via OAuth 2.0 Client Credentials Grant against region-specific GCP base URLs (US2, US3, US4, EU2, EU3).

This GraphQL schema models the same concepts as a unified, typed query surface.

## Schema File

- [bringg-schema.graphql](bringg-schema.graphql)

## Coverage

The schema covers 65+ named types across the following domains:

### Order Domain
- `Order` — top-level order entity linking customer, deliveries, and tasks
- `OrderDetails` — merchant/team/service plan assignment, delivery window, package metadata
- `OrderStatus`, `OrderType`, `OrderPriority` — status, classification, and urgency enums
- `OrderItems` — collection of line items on the order
- `OrderLineItem` — individual SKU/barcode entry with quantity and pricing
- `ItemDetails` — product metadata including hazardous, refrigeration, and dimension flags

### Delivery Domain
- `Delivery` — delivery leg with driver, vehicle, waypoints, tracking, rating, and tip
- `DeliveryDetails` — addresses, proof of delivery, duration, and distance
- `DeliveryStatus`, `DeliveryType` — lifecycle state and fulfillment mode enums
- `DeliveryWindow` — planned start/end time for scheduled delivery slots

### Pickup Domain
- `Pickup` — pickup leg of a delivery
- `PickupDetails` — contact, access code, parking instructions, and ready time

### Driver Domain
- `Driver` — driver entity with location, capacity, and current route
- `DriverDetails` — PII, license, device, and app version metadata
- `DriverStatus` — shift, break, and current task state
- `DriverLocation` — real-time GPS coordinates with heading, speed, and accuracy
- `DriverCapacity` — weight/volume/item utilization vs maximums

### Task Domain
- `Task` — atomic unit of work (delivery, pickup, return, service) assigned to a driver
- `TaskDetails` — merchant context, proof requirements, and custom fields
- `TaskType`, `TaskStatus` — classification and lifecycle enums
- `TaskTimestamp` — full audit trail: created, accepted, started, arrived, completed

### Route Domain
- `Route` — ordered set of stops assigned to a driver and vehicle
- `RouteDetails` — name, planned vs actual start/end, tags
- `RouteOptimization` — optimization strategy enum (time, distance, cost, balanced)
- `RouteStop` — individual waypoint+task pairing with planned and actual arrival times
- `RouteETAs` — per-stop ETA calculations with confidence intervals

### WayPoint Domain
- `WayPoint` — geographic stop on a route (pickup, dropoff, or intermediate)
- `WayPointDetails` — contact, access code, proof of delivery, and signature URLs
- `WayPointType` — classification enum

### Fleet Domain
- `Fleet` — carrier or own-fleet entity with vehicles, drivers, and coverage zones
- `FleetDetails` — region, capabilities, webhook URL, and API version

### Vehicle Domain
- `Vehicle` — vehicle entity with type, capacity, and driver assignment
- `VehicleDetails` — make, model, license plate, fuel type, refrigeration flag
- `VehicleType` — car, van, truck, motorcycle, bicycle, cargo bike, autonomous
- `VehicleCapacity` — max and current weight/volume utilization

### Dispatcher Domain
- `Dispatcher` — human dispatcher with team assignments and role permissions
- `DispatcherDetails` — contact info, role, permissions, and timezone

### Customer Domain
- `Customer` — customer entity with contact details and order history
- `CustomerDetails` — phone, email, opt-in flags, merchant assignment, custom fields
- `CustomerAddress` — collection of saved addresses with a default

### Address & Geo Domain
- `Address` — structured postal address with optional geolocation
- `GeoLocation` — lat/lng with accuracy, altitude, and geofence radius

### Zone Domain
- `Zone` — service area, exclusion zone, depot, or hub with polygon boundary
- `ZoneDetails` — name, color, tags, and merchant assignment
- `ZoneType` — classification enum
- `ZoneAvailability` — operating days/hours, blackout dates, and capacity limits

### Rating & Tip Domain
- `Rating` — post-delivery customer satisfaction score
- `RatingDetails` — numeric score, comment, categories, and merchant response
- `Tip` — monetary gratuity attached to a delivery and driver
- `TipDetails` — amount, currency, payment method, and processing status

### Webhook Domain
- `Webhook` — registered endpoint subscription for Bringg event notifications
- `WebhookEvent` — enum of 22 event types covering the full order/driver/fleet lifecycle
- Webhook delivery record with status code, retry count, and payload

### Tracking Domain
- `Tracking` — customer-facing order progress with event history
- `TrackingDetails` — tracking number, notification channels, and current status
- `TrackingURL` — public URL, short URL, and QR code for customer sharing
- `TrackingEvent` — timestamped status change with location

### Auth Domain
- `APIKey` — scoped API key with expiry and environment
- `Token` — OAuth 2.0 Bearer token response with TTL and regional scope

## Operations

### Queries
Read access to all top-level entities: orders, deliveries, drivers, tasks, routes, waypoints, fleets, vehicles, dispatchers, customers, zones, webhooks, and tracking.

### Mutations
Write operations for creating and updating orders, deliveries, tasks, routes, vehicles, customers, zones, and webhooks; completing tasks with proof of delivery; driver location and status updates; route optimization; rating submission; tip addition; and token generation/revocation.

### Subscriptions
Real-time event streams for order updates, delivery updates, driver location changes, driver status changes, task status changes, route updates, and webhook events.

## Source APIs

| API | Description |
|-----|-------------|
| [Bringg Delivery Hub API](https://developers.bringg.com/reference/welcome-to-bringgs-api-reference) | Orders, runs, customers, service areas, inventory, packages |
| [Bringg Drivers & Shifts API](https://developers.bringg.com/reference/driver-shifts) | Drivers, shifts, delivery blocks, vehicles |
| [Bringg Fleet Partners API](https://developers.bringg.com/reference/overview-1) | Carrier integration, quotes, webhooks |

## Authentication

Bringg uses OAuth 2.0 Client Credentials Grant. Tokens have configurable TTLs (default 30 min for write scopes, 4 hours for read scopes) and are region-specific (US2/US3/US4, EU2/EU3).

## Related Artifacts

- [OpenAPI: Delivery Hub](../openapi/bringg-delivery-hub-api-openapi.yml)
- [OpenAPI: Drivers & Shifts](../openapi/bringg-drivers-shifts-api-openapi.yml)
- [OpenAPI: Fleet Partners](../openapi/bringg-fleet-partners-api-openapi.yml)
- [AsyncAPI: Webhooks](../asyncapi/bringg-webhooks-asyncapi.yml)
- [JSON Schema: Order](../json-schema/bringg-order-schema.json)
- [JSON Schema: Driver](../json-schema/bringg-driver-schema.json)
- [JSON Schema: Customer](../json-schema/bringg-customer-schema.json)
- [JSON Schema: WayPoint](../json-schema/bringg-waypoint-schema.json)
