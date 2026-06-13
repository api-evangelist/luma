# Luma

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
