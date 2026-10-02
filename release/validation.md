# Validation — 2026-10-02

35 native tests passed: 31 model/persistence tests and four UI flows. Tests cover full training, hard paywall, swaps/history/repeated sessions, and full personalised onboarding with plan edits. DEBUG test access does not prove real StoreKit purchases.

All four local HTML pages respond with HTTP 200 and have no horizontal overflow at 390 px. Draft banners are visible. `python3 build.py --release` correctly refuses the absent provider fields. The iOS manifest passes plist validation and is copied into the application bundle. Final signed archive and production privacy report remain required.

Repository is private staging. No public policy link is claimed live. No customer data or application source has been uploaded.
