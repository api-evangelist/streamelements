# StreamElements

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

StreamElements is a cloud-based platform for live streamers and content creators on Twitch, YouTube, Kick and Facebook, offering 100% free customizable overlays and alerts, a chatbot, tipping and donations, loyalty points, giveaways and contests, song requests, a media/merch store, brand sponsorships, and analytics — all managed from the StreamElements dashboard. Developers integrate through a public REST API at api.streamelements.com (kappa v2/v3) authenticated with JWT, overlay API keys, or OAuth2, plus the Astro real-time WebSocket gateway (wss://astro.streamelements.com) for live event topics.

**Areas:** Company · Consumer · Live Streaming · Creator Economy · Overlays · Chatbots · Monetization · Donations · Loyalty Points · Giveaways · Video · Twitch

## StreamElements on APIs.io

Everything profiled for StreamElements is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/streamelements/](https://apis.io/providers/streamelements/)** — or go straight to one of the APIs or properties below.

### APIs (24)

- [StreamElements Activities API](https://apis.io/apis/streamelements/streamelements-activities-api/) — Endpoints to interract with activities collected by StreamElements
- [StreamElements Bot API](https://apis.io/apis/streamelements/streamelements-bot-api/) — Endpoints to manage StreamElements chat bot
- [StreamElements Channels API](https://apis.io/apis/streamelements/streamelements-channels-api/) — Endpoints to get channel data
- [StreamElements Chatstats API](https://apis.io/apis/streamelements/streamelements-chatstats-api/) — Endpoint to get chat statistics
- [StreamElements Commands API](https://apis.io/apis/streamelements/streamelements-commands-api/) — Bot commands management
- [StreamElements Contests API](https://apis.io/apis/streamelements/streamelements-contests-api/) — Endpoints to interract with contests
- [StreamElements Filters API](https://apis.io/apis/streamelements/streamelements-filters-api/) — Bot spam filters management
- [StreamElements Giveaways API](https://apis.io/apis/streamelements/streamelements-giveaways-api/) — This endpoint is available only in the API version 3. Make sure to use the v3 base URL: https://api.streamelements.com/kappa/v3.
- [StreamElements Loyalties API](https://apis.io/apis/streamelements/streamelements-loyalties-api/) — Endpoints to manage loyalty settings
- [StreamElements Modules API](https://apis.io/apis/streamelements/streamelements-modules-api/) — Endpoints to manage bot modules
- [StreamElements Overlays API](https://apis.io/apis/streamelements/streamelements-overlays-api/) — Endpoints to manage overlays assigned to channel
- [StreamElements Points API](https://apis.io/apis/streamelements/streamelements-points-api/) — Endpoints to manage loyalty points
- [StreamElements Redemptions API](https://apis.io/apis/streamelements/streamelements-redemptions-api/) — The redemptions API from StreamElements — 4 operation(s) for redemptions.
- [StreamElements Sessions API](https://apis.io/apis/streamelements/streamelements-sessions-api/) — Endpoints to manage session data
- [StreamElements single contest API](https://apis.io/apis/streamelements/streamelements-single-contest-api/) — The single contest API from StreamElements — 6 operation(s) for single contest.
- [StreamElements single giveaway API](https://apis.io/apis/streamelements/streamelements-single-giveaway-api/) — This endpoint is available only in the API version 3. Make sure to use the v3 base URL: https://api.streamelements.com/kappa/v3.
- [StreamElements single user API](https://apis.io/apis/streamelements/streamelements-single-user-api/) — Endpoints to manage single user points data
- [StreamElements Songrequests API](https://apis.io/apis/streamelements/streamelements-songrequests-api/) — Endpoints to interact with StreamElements Mediashare
- [StreamElements Stats API](https://apis.io/apis/streamelements/streamelements-stats-api/) — Folder for loyalty
- [StreamElements Store API](https://apis.io/apis/streamelements/streamelements-store-api/) — Store items management
- [StreamElements Themes API](https://apis.io/apis/streamelements/streamelements-themes-api/) — Endpoints to browse StreamElements themes
- [StreamElements Timers API](https://apis.io/apis/streamelements/streamelements-timers-api/) — Bot timers (chat "cron" messages) management
- [StreamElements Tips API](https://apis.io/apis/streamelements/streamelements-tips-api/) — Endpoints to interract with tips
- [StreamElements Users API](https://apis.io/apis/streamelements/streamelements-users-api/) — Folder for loyalty

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [StreamElements Astro Real-Time Gateway](https://apis.io/asyncapis/streamelements/streamelements-astro-asyncapi/)

#### Event channels (18)

Individual events and webhooks the provider emits.

- [channel.activities](https://apis.io/channels/streamelements/channel-activities/)
- [channel.chat.message](https://apis.io/channels/streamelements/channel-chat-message/)
- [channel.chatbot.counters](https://apis.io/channels/streamelements/channel-chatbot-counters/)
- [channel.chatbot.modules.emotecombo](https://apis.io/channels/streamelements/channel-chatbot-modules-emotecombo/)
- [channel.chatbot.modules.pyramid](https://apis.io/channels/streamelements/channel-chatbot-modules-pyramid/)
- [channel.chatbot.status](https://apis.io/channels/streamelements/channel-chatbot-status/)
- [channel.chatbot.timeout](https://apis.io/channels/streamelements/channel-chatbot-timeout/)
- [channel.contests](https://apis.io/channels/streamelements/channel-contests/)
- [channel.giveaways](https://apis.io/channels/streamelements/channel-giveaways/)
- [channel.overlay.action](https://apis.io/channels/streamelements/channel-overlay-action/)
- [channel.overlay.broadcast](https://apis.io/channels/streamelements/channel-overlay-broadcast/)
- [channel.overlay.update](https://apis.io/channels/streamelements/channel-overlay-update/)
- [channel.session.reset](https://apis.io/channels/streamelements/channel-session-reset/)
- [channel.session.update](https://apis.io/channels/streamelements/channel-session-update/)
- [channel.songrequest](https://apis.io/channels/streamelements/channel-songrequest/)
- [channel.stream.status](https://apis.io/channels/streamelements/channel-stream-status/)
- [channel.tips](https://apis.io/channels/streamelements/channel-tips/)
- [channel.tips.moderation](https://apis.io/channels/streamelements/channel-tips-moderation/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [streamelements](https://apis.io/servers/streamelements/streamelements/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Streamelements Agentic Access](https://apis.io/agentic-access/streamelements/streamelements-agentic-access/)

#### Collections (24)

Postman and Open Collection request collections.

- [SE API Docs activities API](https://apis.io/collections/streamelements/open-streamelements-activities-api/)
- [SE API Docs activities bot API](https://apis.io/collections/streamelements/open-streamelements-bot-api/)
- [SE API Docs activities channels API](https://apis.io/collections/streamelements/open-streamelements-channels-api/)
- [SE API Docs activities chatstats API](https://apis.io/collections/streamelements/open-streamelements-chatstats-api/)
- [SE API Docs activities commands API](https://apis.io/collections/streamelements/open-streamelements-commands-api/)
- [SE API Docs activities contests API](https://apis.io/collections/streamelements/open-streamelements-contests-api/)
- [SE API Docs activities filters API](https://apis.io/collections/streamelements/open-streamelements-filters-api/)
- [SE API Docs activities giveaways API](https://apis.io/collections/streamelements/open-streamelements-giveaways-api/)
- [SE API Docs activities loyalties API](https://apis.io/collections/streamelements/open-streamelements-loyalties-api/)
- [SE API Docs activities modules API](https://apis.io/collections/streamelements/open-streamelements-modules-api/)
- [SE API Docs activities overlays API](https://apis.io/collections/streamelements/open-streamelements-overlays-api/)
- [SE API Docs activities points API](https://apis.io/collections/streamelements/open-streamelements-points-api/)
- [SE API Docs activities redemptions API](https://apis.io/collections/streamelements/open-streamelements-redemptions-api/)
- [SE API Docs activities sessions API](https://apis.io/collections/streamelements/open-streamelements-sessions-api/)
- [SE API Docs activities single contest API](https://apis.io/collections/streamelements/open-streamelements-single-contest-api/)
- [SE API Docs activities single giveaway API](https://apis.io/collections/streamelements/open-streamelements-single-giveaway-api/)
- [SE API Docs activities single user API](https://apis.io/collections/streamelements/open-streamelements-single-user-api/)
- [SE API Docs activities songrequests API](https://apis.io/collections/streamelements/open-streamelements-songrequests-api/)
- [SE API Docs activities stats API](https://apis.io/collections/streamelements/open-streamelements-stats-api/)
- [SE API Docs activities store API](https://apis.io/collections/streamelements/open-streamelements-store-api/)
- [SE API Docs activities themes API](https://apis.io/collections/streamelements/open-streamelements-themes-api/)
- [SE API Docs activities timers API](https://apis.io/collections/streamelements/open-streamelements-timers-api/)
- [SE API Docs activities tips API](https://apis.io/collections/streamelements/open-streamelements-tips-api/)
- [SE API Docs activities users API](https://apis.io/collections/streamelements/open-streamelements-users-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Streamelements Api Overlay](https://apis.io/overlays/streamelements/streamelements-api-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Streamelements Authentication](https://apis.io/security/streamelements/streamelements-authentication/)
- [Streamelements Domain Security](https://apis.io/security/streamelements/streamelements-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Streamelements Scopes](https://apis.io/scopes/streamelements/streamelements-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.streamelements.com/)
- [Documentation](https://dev.streamelements.com/docs/api-docs)
- [Getting started](https://dev.streamelements.com/docs/api-docs/authentication)
- [API reference](https://dev.streamelements.com/docs/api-docs)
- [Sign up](https://streamelements.com/login)
- [Support](https://support.streamelements.com/)
- [Blog](https://blog.streamelements.com/)
- [Terms of service](https://streamelements.com/terms)
- [Privacy policy](https://streamelements.com/privacy)
- [GitHub](https://github.com/StreamElements)
- [Status](https://status.streamelements.com/)

## API Evangelist rating

**Kin Score 43.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 56.2 |
| Contract governance | 4.5 |
| Operational transparency | 42.1 |
| Developer ergonomics | 37.5 |
| Access clarity | 34.2 |

**Agent readiness 35.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | — |

**Regulatory alignment 34.3** — AI & Biometrics

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/streamelements/](https://apis.io/providers/streamelements/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for StreamElements: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/streamelements/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
