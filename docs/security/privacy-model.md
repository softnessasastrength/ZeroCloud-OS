# Privacy, consent and security model

## Principles
Local-first, least privilege, audience-scoped disclosure, purpose limitation, transparent provenance, revocable future sharing, and no covert tracking.

## Data classes
1. Private local: black-book notes, personal reflections, local search index, private albums.
2. Selectively shared: presence, availability, plans, location, chosen media and messages.
3. Operational metadata: identity/key identifiers, delivery state, timestamps and relay routing; minimize and disclose residual exposure.

## Required enforcement
- Explicit field-level consent and audience checks at every publication.
- Per-connection directional location sharing with expiry and precision.
- E2EE for qualifying shared spaces with device key lifecycle, verification, rotation, recovery and compromise handling.
- No server-side plaintext indexing of private notes or reflections.
- Permission revocation propagates to caches and future transmissions; cannot retract copies already received.
- Encrypted storage and backups with tested restore/delete behavior.
- Locked-device redaction, notification privacy and secure recent-task previews.
- No automatic emotion inference, relationship scoring, coercive engagement ranking, or inferred invitation.
- No silent transport downgrade across SMS/MMS/RCS/Matrix.

## Verification gates
Threat model for stalking, coercion, device theft, key loss, compromised relay, abusive invitations and accidental disclosure; independent crypto review, fuzzing, offline/replay tests, privacy regression tests, and usability studies before release.
