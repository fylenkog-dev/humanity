# HUMANITY

**HUMANITY** is a concept for a global space where people can share personal stories, discover common values, and build human connection across backgrounds and borders.

The repository contains an early website prototype with a browser-rendered 3D Earth experience. It is a product exploration, not a live community platform.

## Project status

- **Current stage:** early MVP concept / static prototype
- **Primary language:** Ukrainian
- **Entry point:** [HUMANITY MVP page](HUMANITY_MVP_0.1/HUMANITY_mvp/index.html)
- **Main experience:** [Interactive world story map](HUMANITY_MVP_0.1/HUMANITY_mvp/map.html)
- **Product direction:** see [Product brief and roadmap](docs/PRODUCT_BRIEF.md)
- **Story journey:** see [Story submission experience](docs/STORY_SUBMISSION_FLOW.md)
- **Interactive demos:** [world story map](HUMANITY_MVP_0.1/HUMANITY_mvp/map.html) · [local-only story form](HUMANITY_MVP_0.1/HUMANITY_mvp/story.html)
- **Trust and safety:** see [Community guidelines and moderation framework](docs/COMMUNITY_GUIDELINES.md)
- **Product inspiration:** see [Research and integration roadmap](docs/INSPIRATION_AND_INTEGRATIONS.md)

## Run locally

No build step or API key is required. Open `HUMANITY_MVP_0.1/HUMANITY_mvp/index.html` in a modern browser. The 3D map loads Three.js and Earth textures from external CDNs, so an internet connection is needed for the full globe experience. A simpler animated fallback is shown when WebGL or the 3D library is unavailable; its satellite texture also needs internet access.

## Current prototype includes

- Responsive landing page
- Introductory explanation of the project
- Interactive 3D Earth with satellite-style surface texture, atmosphere, cloud layer, star field, and sample story markers
- Mouse/touch orbit and zoom controls, plus small decorative planets in the background
- Story preview panel, topic filters, text search, and zoom controls
- A guided five-story “Humanity Journey” across countries, with subtle symbolic connection arcs on the 3D globe
- A non-WebGL fallback globe with selectable sample stories and working topic/search filters
- A keyboard-accessible story list that opens the same story panel without requiring pointer interaction
- Local-only sample reactions (not transmitted or saved)
- Core values section
- Accessibility basics: semantic landmarks, skip link, visible keyboard focus, and reduced-motion support

## Not implemented

There is no backend, database, user account system, persistent story submission, publishing, moderation, live story search, geolocation, analytics, or production deployment. The 3D Earth uses externally hosted demo textures and Three.js; story points, search, filters, and reactions operate only on built-in demonstration content. The prototype does not collect or store visitor data.

## Product principles

1. **Human dignity first.** People should be treated respectfully regardless of origin, identity, belief, or circumstance.
2. **Consent and control.** A person should understand what they are sharing and be able to control whether it is public.
3. **Safety before reach.** Reporting, moderation, privacy, and abuse prevention must be designed before opening public publishing.
4. **Authenticity.** Sample content must never be presented as a real user's testimony.
5. **Accessibility.** The experience should work across devices and support different ways of navigating and reading.

## Development approach

Build in small, reviewable steps. Keep the static prototype safe and transparent while validating the product experience. Do not introduce authentication, personal-data collection, payments, or production infrastructure without an explicit product and security review.
