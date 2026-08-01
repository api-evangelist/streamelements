---
name: Subscribe to real-time channel events (Astro)
description: Connect to the StreamElements Astro WebSocket gateway and subscribe to per-channel topics (tips, activities, session updates) to react to live events.
api: asyncapi/streamelements-astro-asyncapi.yml
operations:
  - WSS astro.streamelements.com/ subscribe channel.tips
  - WSS astro.streamelements.com/ subscribe channel.activities
  - WSS astro.streamelements.com/ subscribe channel.session.update
---

# Subscribe to real-time channel events (Astro)

Astro is StreamElements' pubsub WebSocket gateway for live stream events. Use it instead of polling the REST API when you need to react the moment something happens.

## Connect
Open `wss://astro.streamelements.com/`. On connect the server sends a `welcome` message. If reconnecting after a graceful shutdown, include `?reconnect_token=<token>`. A draining server rejects with `502`; exceeding the connection rate limit returns `429` with `Retry-After: 2`.

## Authenticate + subscribe
Send a subscribe message carrying `data.token` and `data.token_type` (`jwt`, `apikey`, or `oauth2`) plus the `topic`. Tokens are account-specific — copy the token for the platform account (Twitch/YouTube/Kick) whose events you want.

## Topics (and required scope)
- `channel.tips` — completed tips/donations (`tips:read`)
- `channel.activities` — follows/subs/cheers/hosts/raids/redemptions (`activities:read`)
- `channel.session.update` — latest tip/follower/sub, goals, totals (`session:read`)
- `channel.stream.status` — live/offline (`stream-live:read`)
- `channel.chatbot.status` — chatbot connection state (`bot:read`)

Full topic catalog and payloads: `asyncapi/streamelements-astro-asyncapi.yml`.

## Payload shape
Every message is JSON: `{ id, ts, type, topic, data }` where `data` is topic-specific (e.g. `channel.tips` carries `data.donation.{user,amount,currency,message}`).
