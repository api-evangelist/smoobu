# Smoobu (smoobu)

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
