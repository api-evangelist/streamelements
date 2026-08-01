---
name: Read channel activities and tips
description: Resolve the caller's StreamElements channel and read its recent activities and tips (follows, subs, cheers, donations).
api: openapi/streamelements-openapi-original.yml
operations:
  - GET /channels/me
  - GET /activities/{channel}
  - GET /tips/{channel}
  - GET /tips/{channel}/leaderboard
---

# Read channel activities and tips

Use the StreamElements REST API (`https://api.streamelements.com/kappa/v2`) to read a channel's engagement history.

## Auth
Send `Authorization: Bearer <token>` where the token is a channel **JWT**, an **overlay API key**, or an **OAuth2** access token. Reading activities requires the `activities:read` scope; reading tips requires `tips:read`. See `authentication/streamelements-authentication.yml`.

## Steps
1. **Resolve the channel** — `GET /channels/me` returns your channel object; take its `_id` (a 24-char hex guid) as `{channel}`. You may also pass the lowercase channel name as `{channel}`.
2. **List activities** — `GET /activities/{channel}?after=<ISO8601>&before=<ISO8601>`. The `after` window parameter is required. Each item is an activity (type: follow/subscriber/tip/cheer/host/raid/redemption).
3. **List tips** — `GET /tips/{channel}?limit=&offset=` for donation history; `GET /tips/{channel}/leaderboard` for the top tippers.

## Conventions & errors
- Ids are guids matching `/^[0-9a-fA-F]{24}$/`; datetimes are ms timestamps or ISO 8601 strings. See `conventions/streamelements-conventions.yml`.
- `401` → token missing/invalid; `404` → channel not found. See `errors/streamelements-problem-types.yml`.
- No idempotency contract — these are read-only calls, so retries are safe.
