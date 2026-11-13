# Decision 013: Metro navigation and search

## Navigation controls
- **Back tap:** dismiss active overlays or navigate back under Android contracts; preserve predictive-back compatibility when relevant.
- **Start tap:** return to Metro Start.
- **Start long-press:** open recent-apps Metro task switcher.
- **Search tap:** ZeroSearch across permissioned local providers.
- **Search long-press:** contextual search on current app/screen only where integrations explicitly support it.
- **Back long-press:** reserved; no conflicting default.
- Three-button bar persists in ordinary system use; immersive/fullscreen exceptions must be defined.
- Launcher prototype cannot force global navigation bar behavior; AOSP SystemUI owns actual system-level integration.

## Recents
Horizontal Metro task cards backed by Android task lifecycle. Dismissing a recent task is not force-stop. Screen previews must respect FLAG_SECURE and privacy-sensitive content; accessibility labels and keyboard alternatives required.

## ZeroSearch
Search provider contract: query, permissions, provenance, result type, ranking hints, deep-link action and redaction policy. Contacts, apps, authorized conversations, shared plans and media may provide results. No blanket database access. Private notes and E2EE data remain locked/excluded until locally authorized. No sensitive lockscreen previews.

## People access
1. Visible People affordance/optional Start sidebar.
2. Search a person to see permitted communication routes, presence and plans.
3. Full ZeroPeople app for contacts and ZeroConnections.

## Accessibility and performance
Touch targets, high contrast, scalable type, TalkBack, switch access, keyboard focus, one-handed alternatives, reduced motion, insets and orientation support. Measure tap count and task completion through consented usability studies, not surveillance.
