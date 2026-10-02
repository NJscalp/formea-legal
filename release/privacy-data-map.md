# Privacy data map — current iPhone source, 2026-10-02

| Data / service | Where it goes | Purpose | Evidence |
|---|---|---|---|
| Onboarding answers, goals, activity, movement preferences | Local JSON in app sandbox | Rule-based plan ordering and variants | `OnboardingView.swift`, `Personalization.swift`, `AppStore.swift` |
| Schedule and reminders | Local state and iOS local notification scheduler | User-selected reminders | `Plan.swift` |
| Energy check-in, workout dates, actual time, exercise status, feedback, optional body ratings | Local JSON | Adapt today's session, resume, show progress/history | `Models.swift`, `AppStore.swift`, `RitualViews.swift` |
| Product identifiers and verified subscription entitlement, expiration/revocation | Apple StoreKit and on-device entitlement check | Purchases and access control | `PaywallView.swift` |
| Payment details | Apple | App Store billing | Developer receives no card data through this source |
| Voluntary support email and attachments | Provider mailbox; mail providers | Respond to a user request | Public support operation, not automatic app telemetry |
| IP and browser request information when legal links open | GitHub Pages hosting | Deliver the website | Separate website processing; disclose GitHub |

No developer backend, account, analytics SDK, ads, tracking identifier, HealthKit, cloud sync, camera, location, contacts or microphone integration was found in the current app source. Backups are Apple/device settings, not a Formea sync service.

## Proposed App Store Connect answers

The current app-only code is a candidate for **Data Not Collected** under Apple's definition: local processing is not off-device collection by the developer. This is a proposal, not a submitted answer. Confirm the final binary, all SDKs, support flows, App Store reports and any later integrations before answering. Voluntary off-app support email and GitHub hosting are still disclosed in the policy. If support moves inside the app or a service begins retaining app-linked data, re-evaluate the privacy label.

Tracking: no. ATT permission: not currently needed. Health/fitness data exist locally; do not claim the app does not handle any fitness data. A privacy manifest is distinct from the public privacy policy and the App Store Connect privacy questionnaire.

The source uses file existence and local reading/writing, not filesystem timestamps, disk-space APIs, UserDefaults, system boot time or active keyboard APIs found in Apple's required-reason API list. Re-check the archived binary and any SDK additions; do not add fictional API reasons. The manifest records no tracking, no collected data and no required-reason API usage for the audited source.

Sources: [Apple privacy definitions](https://developer.apple.com/app-store/app-privacy-details/), [privacy manifests](https://developer.apple.com/documentation/bundleresources/privacy-manifest-files), [GitHub privacy](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).
