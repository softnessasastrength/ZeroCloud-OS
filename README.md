# ZeroCloud OS

**A connection-first, Metro-inspired Android operating system.**

ZeroCloud OS is a proposed Android-native-first, eventually AOSP-derived platform designed to reduce the everyday friction of human connection while preserving autonomy, consent, privacy, accessibility, and robust core phone functionality.

> We can communicate with almost anyone in the world. The operating system should make it easier to actually connect.

## Project status
Architecture and product design only. No functioning OS build, device compatibility, cryptographic implementation, or security audit is claimed.

- **Accepted:** Architecture Decisions 001–013.
- **Pending:** Design Decision 014, intelligent connection layer.
- **Proposed, not separately accepted:** ZeroPresence, Social Availability, ZeroReflections, ZeroMemories.

## Documentation
- [Architecture overview](docs/architecture/system-overview.md)
- [Decision register](docs/decisions/README.md)
- [Connection platform](docs/connections/zeroconnections.md)
- [Security and consent](docs/security/privacy-model.md)
- [Roadmap](ROADMAP.md)

## Platform strategy
1. Kotlin/Jetpack Compose launcher and first-party app prototypes on Android.
2. Emulator/Cuttlefish validation, then verified supported unlockable Pixel hardware.
3. AOSP integration of SystemUI, navigation, search, settings and platform services.
4. Pure, Compatible, and Developer editions, with licensing and certification constraints respected.

## Non-negotiables
Explicit audience-scoped consent; local-first data processing; no covert tracking; E2EE for eligible shared spaces with independently managed keys; no misleading transport security labels; no invented memories or emotional inferences; secure updates and Android platform security preserved.

This repository is independent of the separate ZeroCloud miniature-cloud infrastructure project.
