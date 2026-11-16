# HUMANITY — Product brief and roadmap

_Last updated: 2026-11-16_

## 1. Product idea

HUMANITY is a global space for personal stories, shared values, and human connection. Its purpose is to help people encounter experiences beyond their own and find common ground without erasing cultural or personal differences.

This is an early product direction, not a validated market claim.

## 2. Who it may serve

Initial audience hypotheses:
- People who want to share a meaningful personal experience.
- Readers interested in first-person perspectives beyond their immediate community.
- Community builders and educators who want thoughtful, human-centred stories.

These are hypotheses to validate with research, not confirmed user segments.

## 3. Experience principles

- **Respect:** no dehumanizing language or harassment.
- **Agency:** clear consent before a story becomes public.
- **Context:** authors choose what personal details to include; sensitive details should not be required.
- **Safety:** visible reporting and a defined moderation process before public submissions launch.
- **Transparency:** explain why content is shown, how it is moderated, and what data is collected.
- **Accessibility:** readable typography, keyboard navigation, responsive layouts, and reduced-motion support.
- **Multilingual by design:** avoid assuming that one language or cultural frame represents everyone.

## 4. Current state

The repository contains a static Ukrainian landing-page prototype. It has an introduction, illustrative story cards, values, and a participation call-to-action. It has no working submission flow or data persistence.

The story cards are explicitly illustrative and must not be mistaken for real user submissions.

## 5. Proposed roadmap

### Phase A — Foundation (current)
- [x] Establish a clear project description.
- [x] Improve the landing page and mobile navigation.
- [x] Mark sample stories as illustrative.
- [x] Document product principles and current limitations.
- [ ] Review the experience with a small group of potential users.
- [ ] Decide the first supported languages and accessibility baseline.

### Phase B — Story experience design
- [x] Draft story fields and optional author attribution.
- [x] Propose consent and visibility choices for review.
- [ ] Design story reading and author profile states without requiring accounts by default.
- [ ] Define content categories and a lightweight discovery model.
- [ ] Test prototypes with people from different language and cultural contexts.

### Phase C — Trust and safety design
- [x] Draft community guidelines and moderation principles.
- [x] Outline reporting, moderation outcomes, escalation, and appeals (workflow design only).
- [ ] Define privacy, retention, deletion, and data-access policies.
- [ ] Threat-model abuse, spam, impersonation, doxxing, and targeted harassment.
- [ ] Decide operational ownership and response expectations before accepting submissions.

### Phase D — Private pilot
- [ ] Select a minimal technical architecture after requirements are validated.
- [ ] Implement a private, invitation-only submission workflow.
- [ ] Add moderation before publication.
- [ ] Add secure storage, access controls, backups, and deletion procedures.
- [ ] Test security, accessibility, and operational readiness.
- [ ] Run a limited pilot; do not open public publishing until safety checks pass.

### Phase E — Public launch consideration
- [ ] Review pilot outcomes and unresolved risks.
- [ ] Confirm moderation capacity and incident response.
- [ ] Complete privacy and security review.
- [ ] Obtain explicit approval for production deployment.

## 6. Decisions intentionally not made

The project has not yet selected:
- A backend, database, hosting provider, or framework.
- An authentication model.
- Whether stories are public by default or require editorial approval.
- A moderation staffing model or service-level commitment.
- Analytics, advertising, payments, or monetization.
- A global launch date.

These decisions should follow user research, privacy review, and operational planning rather than being guessed during implementation.

## 7. Immediate next steps

1. Validate the landing-page message and visual direction with a few representative readers.
2. Create a story-submission journey as a non-functional prototype, including consent and visibility choices.
3. Review the draft community guidelines and moderation framework with policy, privacy, and safety stakeholders.
4. Record feedback and revise the product brief before choosing infrastructure.

## 8. Non-goals for the current prototype

The current static site must not imply that users can already create accounts, publish stories, message each other, or receive moderation support. No personal information is collected by this prototype.
