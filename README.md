# Smoobu (smoobu)

Smoobu is an all-in-one vacation rental channel manager and property management system for short-term rental hosts and property managers. It synchronizes availability, rates, and reservations across Airbnb, Booking.com, Vrbo, and other channels, and provides a booking website, unified guest inbox, automated messaging, guest online check-in, invoicing, and dynamic pricing. The Smoobu REST API (base `https://login.smoobu.com/api`) lets Professional subscribers and integration partners read and write apartments, reservations, rates and availability, guests, and guest messages, and receive webhook notifications when bookings change. Authentication is via an API key header (with HMAC-signed requests recommended and OAuth 2 available for partners).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/apis.yml)

## Tags

- Vacation Rental
- Channel Manager
- Property Management
- Short-Term Rental
- Reservations
- Hospitality

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Smoobu Reservations API

List, retrieve, create, update, and delete reservations (bookings) across all connected channels, with rich filtering by created, arrival, departure, and modified dates. Manage per-reservation price elements (line items) and read the booking, guest, channel, and payment details behind each stay.

- **Human URL:** [https://docs.smoobu.com/](https://docs.smoobu.com/)
- **Base URL:** `https://login.smoobu.com/api`

#### Tags

- Reservations
- Bookings
- Price Elements

#### Properties

- [Documentation](https://docs.smoobu.com/)
- [API Reference](https://docs.smoobu.com/)
- [OpenAPI](openapi/smoobu-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/smoobu.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/smoobu.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Smoobu Apartments API

List all apartments (properties/listings) in a Smoobu account and retrieve a single apartment's details - name, location, currency, rooms, amenities, and connected-channel metadata used to scope reservations, rates, and availability.

- **Human URL:** [https://docs.smoobu.com/](https://docs.smoobu.com/)
- **Base URL:** `https://login.smoobu.com/api`

#### Tags

- Apartments
- Properties
- Listings

#### Properties

- [Documentation](https://docs.smoobu.com/)
- [API Reference](https://docs.smoobu.com/)
- [OpenAPI](openapi/smoobu-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/smoobu.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/smoobu.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Smoobu Rates and Availability API

Read daily rates, prices, availability, and minimum-length-of-stay per apartment over a date range, and push rate, price, availability, and restriction updates back to Smoobu (which propagates them to connected channels). Check bookable availability and quote a price for a stay via the booking availability endpoint.

- **Human URL:** [https://docs.smoobu.com/](https://docs.smoobu.com/)
- **Base URL:** `https://login.smoobu.com/api`

#### Tags

- Rates
- Availability
- Pricing

#### Properties

- [Documentation](https://docs.smoobu.com/)
- [API Reference](https://docs.smoobu.com/)
- [OpenAPI](openapi/smoobu-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/smoobu.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/smoobu.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Smoobu Guests API

List and retrieve guest records - name, contact details, address, language, and the reservations associated with each guest - for use in CRM, communication, and guest-experience workflows.

- **Human URL:** [https://docs.smoobu.com/](https://docs.smoobu.com/)
- **Base URL:** `https://login.smoobu.com/api`

#### Tags

- Guests
- Contacts
- CRM

#### Properties

- [Documentation](https://docs.smoobu.com/)
- [API Reference](https://docs.smoobu.com/)
- [OpenAPI](openapi/smoobu-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/smoobu.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/smoobu.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Smoobu Messaging API

Read the message history for a reservation, list message threads across the unified inbox, and send messages to the guest or to the host (channel) on a reservation - powering automated guest communication and support tooling.

- **Human URL:** [https://docs.smoobu.com/](https://docs.smoobu.com/)
- **Base URL:** `https://login.smoobu.com/api`

#### Tags

- Messages
- Inbox
- Guest Communication

#### Properties

- [Documentation](https://docs.smoobu.com/)
- [API Reference](https://docs.smoobu.com/)
- [OpenAPI](openapi/smoobu-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/smoobu.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/smoobu.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Smoobu Webhooks

Register an HTTPS endpoint to receive server-to-server webhook callbacks when reservations change. Smoobu POSTs a JSON payload with an action field (newReservation, updateReservation, cancelReservation, deleteReservation), the account user id, and the affected reservation data, so integrations can stay in sync without polling.

- **Human URL:** [https://docs.smoobu.com/](https://docs.smoobu.com/)
- **Base URL:** `https://login.smoobu.com/api`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.smoobu.com/)
- [OpenAPI](openapi/smoobu-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/smoobu)
- [Website](https://www.smoobu.com)
- [Documentation](https://docs.smoobu.com/)
- [Plans](plans/smoobu-plans-pricing.yml)
- [Rate Limits](rate-limits/smoobu-rate-limits.yml)
- [Fin Ops](finops/smoobu-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
