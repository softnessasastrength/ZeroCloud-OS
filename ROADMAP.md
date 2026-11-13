# ZeroCloud OS roadmap

**Status: design only.** Stages are planned, not completed.

| Stage | Scope | Exit criteria |
|---|---|---|
| 0 | ADRs, threat model, design tokens, repo scaffolding | decisions versioned, CI plan, risk register |
| 1 | Kotlin/Compose Metro launcher, tiles, accessible navigation | stock Android prototype, UI tests |
| 2 | ZeroPeople and ZeroSearch portable APIs | permission tests, local-only search |
| 3 | ZeroMessages/Phone/Camera/Gallery foundations | capability-gated integrations, privacy tests |
| 4 | Private ZeroConnections black book | encrypted storage, import/export, delete tests |
| 5 | Identity and shared E2EE spaces | audited protocol design, key recovery, delivery tests |
| 6 | Granular presence, social availability and location | consent/abuse testing, stale/offline UX |
| 7 | ZeroReflections and ZeroMemories proposals if approved | provenance and user-curation tests |
| 8 | AOSP emulator/Cuttlefish integration | SystemUI/navigation/recents build and regression CI |
| 9 | Qualified Pixel device port | vendor compatibility, secure boot/update/recovery tests |
| 10 | Pure/Compatible/Developer edition releases | edition-specific validation, licensing review |

## Pending decision 014
Select the intelligence architecture before implementing local contextual models: A manual, B rules, C contextual, D local-first ML, E extensible external provider. No choice yet.

## Scope boundaries
No code, OS image, ROM compatibility, E2EE implementation or release is represented as completed by this documentation.
