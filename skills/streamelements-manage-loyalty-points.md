---
name: Manage channel loyalty points and store
description: Read a channel's loyalty leaderboard, adjust a viewer's points, and manage the loyalty store items and redemptions.
api: openapi/streamelements-openapi-original.yml
operations:
  - GET /points/{channel}/top
  - GET /points/{channel}/alltime
  - PUT /points/{channel}
  - GET /store/{channel}/items
  - POST /store/{channel}/items
  - GET /store/{channel}/redemptions
  - PUT /store/{channel}/redemptions/{redemptionId}
---

# Manage channel loyalty points and store

Loyalty points are the channel's engagement currency; the store lets viewers redeem points for items.

## Auth
`Authorization: Bearer <token>`. Reading loyalty needs `loyalty:read`; writing needs `loyalty:write`. Store reads need `store:read`; creating items / completing redemptions needs `store:write`. See `authentication/streamelements-authentication.yml` and `scopes/streamelements-scopes.yml`.

## Steps
1. **Read the leaderboard** — `GET /points/{channel}/top` (current) or `GET /points/{channel}/alltime`. Use `GET /points/{channel}/watchtime` for watch-time ranking.
2. **Adjust points** — `PUT /points/{channel}` to add/deduct a viewer's points (body carries the username and amount).
3. **List / create store items** — `GET /store/{channel}/items`; `POST /store/{channel}/items` to add a redeemable item.
4. **Handle redemptions** — `GET /store/{channel}/redemptions` to list; `PUT /store/{channel}/redemptions/{redemptionId}` to complete/approve a redemption; `DELETE` to reject.

## Conventions & errors
- `{channel}` is the channel guid or lowercase name; `{redemptionId}`/`{itemId}` are guids.
- Writes are **not idempotent** (no Idempotency-Key) — do not blind-retry a `PUT /points`; re-read before retrying on a `409`/timeout.
- See `errors/streamelements-problem-types.yml` and `conventions/streamelements-conventions.yml`.
