# ZeroCloud OS system architecture

## Purpose
A local-first, connection-first Metro-inspired Android platform. Minimize steps between an intention to reach someone and an authorized action, without converting availability into an obligation.

## Layers
1. **Experience:** ZeroStart launcher, Metro design system, Back/Start/Search navigation, People sidebar, ZeroSearch, task switcher.
2. **Applications:** ZeroPhone, ZeroMessages, ZeroPeople, ZeroCamera, ZeroGallery, ZeroClock, ZeroCalc, ZeroFiles, ZeroPower, ZeroSettings, ZeroHub.
3. **Portable core:** contact identity mapping, privacy policy engine, consent registry, local search providers, encrypted storage, connection suggestions, media indexing, event provenance.
4. **Optional networking:** authenticated identity, E2EE shared spaces, ciphertext relay, delivery acknowledgments, optional encrypted backup and recovery.
5. **AOSP privileged layer:** SystemUI, navigation dispatch, recents, settings, notification integration, platform services. Do not claim these APIs are available to an ordinary launcher.

## Editions
Pure (Google-free), Compatible (only legally licensed/certified proprietary integrations), Developer (experimental but security-aware).

## Cross-cutting contracts
- Per-source permission and per-recipient disclosure boundaries.
- No location collection as a prerequisite for using People or Memories.
- Every contextual suggestion includes provenance and dismissal controls.
- Data minimization, encrypted local storage, offline-first operation.
- Capability gating for Camera2/HAL, radio, RCS, power APIs and device vendor services.
- No engagement optimization, coercive social scoring or hidden presence tracking.

## Architecture status
Specification only. Interfaces, device support, cryptographic protocol and build pipeline require implementation and testing.
