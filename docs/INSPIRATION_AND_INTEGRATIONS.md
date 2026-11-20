# HUMANITY — inspiration research and integration roadmap

_Last reviewed: 2026-11-20. This is product research, not an endorsement or claim of partnership._

HUMANITY should borrow proven interaction patterns, not copy another service's identity or interface. The goal is a warm, accessible global story space where people can discover shared experiences while authors retain control over what they reveal.

## Reference projects and what we learn

| Reference | Useful pattern | HUMANITY adaptation |
|---|---|---|
| [Terrastories](https://terrastories.app/) | Community-led place-based storytelling; private/restricted stories; offline-first and data-sovereignty principles | Broad location only by default; private/restricted visibility designed before public publishing; community ownership and consent |
| [Historypin](https://www.historypin.org/) | Collaborative map pins, collections, favorites, comments, themed tours | Curated story collections and gentle reactions; comments only after moderation and reporting are operational |
| [StoryMapJS](https://storymap.knightlab.com/) | A sequence of stories connected by geography and narrative | Short editorial journeys that guide readers across places and shared values |
| [Globe.gl](https://globe.gl/) | Interactive Three.js globe with data layers and arcs | Keep the existing Three.js globe; use subtle connection arcs as a visual metaphor between sample stories |
| [CesiumJS](https://cesium.com/platform/cesiumjs/) | Open-source globe engine, precise geospatial rendering and large-scale data support | Keep as a future evaluation if we outgrow the lightweight custom globe; no need to migrate the early prototype now |

## Changes introduced in the prototype

- Added a **Humanity Journey** panel with a five-story guided sequence across countries.
- Added subtle curved links between sample story locations on the 3D globe. These are symbolic connections, not routes or claims of real relationships.
- Kept the guided journey available in both the Three.js view and the non-WebGL fallback.
- No external accounts, API keys, user tracking, backend, or data collection were introduced.

## Product principles to preserve

1. **People before engagement metrics.** No infinite-scroll pressure, streaks, popularity contests, or public like counts as a measure of human worth.
2. **Consent and privacy by design.** Ask for country/region only; never require precise coordinates. Offer private/restricted stories only when the backend can enforce access.
3. **Authenticity.** Demo stories remain clearly labeled as fictional examples. Never invent a community member or imply a sample reaction is real.
4. **Safe participation.** Reporting, moderation, appeals, and safeguarding need real owners and tested workflows before public publishing or comments.
5. **Accessible discovery.** Search, filters, keyboard controls, reduced motion, readable typography, and a non-WebGL fallback.
6. **Community benefit.** Future collections can support themes such as welcome, kindness, rebuilding, belonging, and mutual aid, but must not become unverified fundraising or emergency-response channels.

## Candidate integrations (not enabled)

- **MapLibre GL JS** for an optional 2D map mode and open map-data ecosystem.
- **CesiumJS** if terrain, large-scale geospatial data, or a more capable globe becomes necessary.
- **StoryMapJS-inspired editor** for author-created multi-place journeys, after real story storage and moderation exist.
- **Audio storytelling** (short voice notes with explicit consent and transcript option) only after privacy, storage, deletion, and moderation are designed.
- **Translation workflow** with original-language display and clearly labeled machine-assisted translations; never silently overwrite the author's words.

## What we deliberately will not add yet

- Public comments, direct messages, precise live location, public author profiles, follower counts, algorithmic ranking, fundraising, or open uploads.
- Authentication, databases, payments, analytics, and production deployment without explicit product/security review and user approval.

## Current limitations

This repository is still a static prototype. The guided journey, globe markers, and reactions use hard-coded demo content and browser-only state. They do not represent actual users, submit stories, persist reactions, or provide moderation. Any future public launch requires an approved privacy notice, consent model, moderation staffing, reporting/appeals, retention/deletion policy, and secure backend.
