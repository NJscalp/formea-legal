# Formea subscription data map — 2026-10-05

Onboarding answers, fitness goals, workouts, progress and local reminder settings remain on the device.

RevenueCat receives anonymous customer identifiers and purchase/transaction records to deliver subscription functionality. Apple handles payment credentials. No email, name, IDFA, advertising attributes or fitness records are submitted to RevenueCat by Formea.

App Store privacy disclosures must include **Purchases → Purchase History**, for **App Functionality** and **Analytics**, **not linked to an identifiable person** and **no tracking**. RevenueCat generates anonymous IDs; no custom user ID or identifiable customer attributes are supplied. Data Not Collected is no longer appropriate for this integration. Review the final binary and RevenueCat configuration before publication.

The app uses UserDefaults to retain migration status: required reason **CA92.1**. RevenueCat ships its own privacy manifest. Anonymous purchase history is declared as unlinked data in Formea’s manifest.

Build 3 was submitted before the RevenueCat SDK integration. Build 4 adds the SDK. Server notifications can report new purchases from build 3 after the Formea Apple connection was configured; this is not a historical backfill of all prior customers.

Source: https://www.revenuecat.com/docs/platform-resources/apple-platform-resources/apple-app-privacy
