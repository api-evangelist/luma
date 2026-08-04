# Luma

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

Modern event hosting platform with REST APIs for creating events, managing ticketing, tracking attendance, and building community around live and virtual events.

**Website:** [luma.com](https://luma.com)
**API Docs:** [docs.luma.com/reference](https://docs.luma.com/reference)
**Help Center:** [help.luma.com](https://help.luma.com)

## Overview

Luma (formerly lu.ma) is an event management platform that enables organizers to create calendars, host live and virtual events, manage guest registrations, sell tickets, and build ongoing communities. The platform launched in 2020 and raised $20M Series A funding from Andreessen Horowitz in 2023.

## API

The Luma REST API allows programmatic access to all core platform resources. The base URL is `https://public-api.luma.com` and all requests require an `x-luma-api-key` header.

**API access requires an active Luma Plus subscription ($59/month, billed annually).**

### Core Resources

- **Calendar** — Create and manage event calendars, admins, and settings
- **Events** — Create, update, cancel, approve, and look up events
- **Guests** — List, invite, update status, and manage event attendees
- **Tickets** — Create and manage ticket types with pricing and capacity
- **Hosts** — Add and manage event hosts and check-in staff
- **Coupons** — Create and manage discount codes at calendar and event levels
- **Tags** — Organize events and contacts with custom tags
- **Contacts** — Import and manage calendar contacts
- **Memberships** — Manage membership tiers and member enrollment
- **Webhooks** — Subscribe to platform events for real-time integrations
- **Organizations** — Manage multiple calendars under an organization account

### Authentication

```
x-luma-api-key: YOUR_API_KEY
```

API keys are created in Luma settings under Settings → Developer → API Keys.

### Rate Limits

| Key Type | Requests per Minute |
|---|---|
| Calendar API key / OAuth token | 200 |
| Organization API key | 500 |

Exceeding the limit returns `429 Too Many Requests` with a 60-second lockout.

## Pricing

| Plan | Price | API Access |
|---|---|---|
| Free | $0/month | No |
| Luma Plus | $59/month (annual) | Yes |
| Enterprise | Custom | Yes |

The Free plan includes a 5% platform fee on ticket sales. Luma Plus removes this fee entirely.

## Resources

- [API Reference](https://docs.luma.com/reference)
- [Pricing](https://luma.com/pricing)
- [Help Center](https://help.luma.com/)
- [API Overview](https://help.luma.com/p/luma-api)
- [Embed Examples (GitHub)](https://github.com/luma-team/examples)
- [X / Twitter](https://x.com/LumaHQ)
