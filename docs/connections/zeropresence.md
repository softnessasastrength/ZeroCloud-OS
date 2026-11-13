# ZeroPresence and Social Availability — proposed ADR-012 extensions

**Status:** Concept proposal, not a separately accepted architecture decision.

## Ambient awareness
A user may choose to share selected availability, activity, social openness, manual mood, calendar-derived free/busy or approximate location with named connections. Each field has independent audience, expiration and precision controls. Calendar contents and private appointments are not disclosed by a free/busy indicator.

## Social Availability
Users may manually publish time-limited openness such as “coffee,” “phone call,” “going out,” or “staying in” to a selected audience. Being available is not consent to an invitation; location is not consent to a visit.

## Lightweight invitation
Where two people have mutually opted to share compatible openness, ZeroCloud may suggest an invitation. Sending requires an affirmative user action. The recipient may accept, decline, ignore or revoke availability without explanation. Do not expose decline history, response surveillance, or “available but ignored you” signals.

## Privacy and lifecycle
Manual status overrides automatic inference. Provide Appear Offline that actually stops presence publication, plus expiry, audience review, revocation and offline/stale indicators. Optional calendar inference stays on-device. Shared status should use authenticated E2EE where implemented, with an explicit metadata threat model.

## Rollout
Manual statuses → calendar free/busy (opt-in) → mutual openness suggestions → optional location-aware presence, only after abuse-case review.
