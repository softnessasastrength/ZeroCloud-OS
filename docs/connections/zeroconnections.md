# ZeroConnections: human connection without social coercion

**Accepted under ADR-012:** A private digital black book and consent-based shared connection platform, local-first by default.

## Identity and trust
People records may combine local contacts and user-confirmed external identities. Linking two records requires explicit user action or review. Mutual connection establishment does not authorize sharing every data field. Support key verification, revocation, device enrollment and recovery with transparent trust state.

## Private black book
Personal notes, important dates, preferences, follow-up ideas, context and manually authored reflections belong only to the device owner by default. No automatic synchronization to the other person. Encrypt at rest and in any optional backup. Provide export, deletion and granular exclusions.

## Shared spaces
Opt-in, per-connection E2EE plans, reminders, notes and selected media. Membership and object-level sharing must be explicit; do not silently copy private notes into shared spaces. A server relay may carry ciphertext but should not receive content keys. Specify threat model, metadata leakage, key rotation, lost-device recovery and revocation limits before shipping.

## Location lifecycle
Directional consent: sender explicitly chooses to share; recipient explicitly chooses to receive. Allow approximate/precise, audience, duration, expiration and immediate stop. Label timestamps, stale fixes, offline status and accuracy. No stealth tracking, no implicit continuous history, no inferred invitation to visit. Revocation stops future updates but cannot erase information already seen or copied by recipients.

## Contextual assistance
Optional, explainable, dismissible suggestions based on authorized local sources: calendar, shared plans, contact notes and explicitly permitted location/photo metadata. No emotional diagnosis, relationship score, or claims that co-location proves a shared experience. Suggestions never send messages or invitations automatically.

## Reliability
Offline queue for user-approved outbound actions, idempotency, delivery acknowledgments, clock-skew handling, explicit sync errors, retry policies and encrypted backup/recovery design. Do not claim E2EE or reliable delivery until audited and tested.

## Stages
Private contact notes → identity linking → E2EE shared spaces → granular location sharing → contextual assistance → multi-device sync and security audit.

## Related proposals
[ZeroPresence](zeropresence.md), [ZeroReflections](zeroreflections.md), [ZeroMemories](zeromemories.md). These are proposed extensions, not separately accepted decisions.
