# Formea submission pack — not ready to submit

## Blocking before release

- Replace workout video placeholders with reviewed demonstrations or another finished, accurate way of teaching every available exercise and variation. The current player visibly says content is pending. Do not market finished videos before they exist.
- Obtain professional review of the exercise instructions, variations, replacement equivalence and 24-session progression. The app currently explicitly describes these as drafts.
- Verify rights to the actual bundled paywall photo and all other assets. The latest reference-pose image was generated with a third-party photo as reference; alteration or generation alone is not proof of rights or non-resemblance. Use licensed or independently created assets with documented provenance where rights are uncertain.
- Complete provider and contact details; publish and test policy/support pages publicly. Add functional privacy and support links to Settings and the paywall. A short private policy sheet alone does not replace public policy hosting.
- Create auto-renewable subscription products `com.formea.plus.weekly` and `com.formea.plus.sixmonths` in one subscription group. Intended US prices: $9.99 weekly and $45.99 every six months. The app must display Apple's localised prices. Configure availability, product localisation, review screenshots, tax/banking agreements and subscription review metadata.
- Test real StoreKit purchase, cancellation, pending purchase, restore, expiry, revocation, billing retry/grace if configured, and product-unavailable behavior using a StoreKit test configuration and Sandbox/TestFlight. Current UI access tests use DEBUG-only simulation and do not prove a successful Apple purchase.
- Demonstrate ongoing membership value; 24 static sessions with unfinished media are a weak offer for recurring billing. Apple requires ongoing value (3.1.2(a)); new content is one possible approach, not a mandatory prescribed feature.

## App Store Connect fields

Name: Formea (check availability). Subtitle candidate: `Pilates at your own pace` (23 characters). Category: Health & Fitness. iPhone only in the current target; minimum iOS 18.

Privacy URL after publication: `https://njscalp.github.io/formea-legal/privacy.html`

Support URL after publication: `https://njscalp.github.io/formea-legal/support.html`

Marketing URL, optional: `https://njscalp.github.io/formea-legal/`

Terms explanation URL: `https://njscalp.github.io/formea-legal/terms.html`. Standard licence: `https://www.apple.com/legal/internet-services/itunes/dev/stdeula/`. These Formea pages supplement Apple's Standard EULA; no custom EULA is currently proposed.

Complete the age-rating questionnaire from the actual content. Do not guess a final rating or mark the app as a children's service. Complete content-rights, app-privacy and export-compliance questions. Verify export treatment of Apple's standard encryption based on the final binary, rather than assuming a blanket exemption. Submit a signed archive with the current accepted Xcode/SDK; check Apple's requirements at upload time.

Supply developer legal identity, app-review contact email and telephone, real copyright owner/year, territory availability and any regional trader disclosures required by App Store Connect. These are operator-supplied fields and cannot be invented from the machine username.

## Store description draft

Make a little space for Pilates. Formea builds a starting plan around your goals, experience, movement preferences and time, so your next session is easy to find.

Explore 24 sessions across four chapters. Choose 5, 10 or 15 minutes, use a gentler variation, swap supported exercises and schedule optional reminders. A daily check-in can help you choose a gentler session. See your recorded workouts and active minutes, revisit saved flows and record extra sessions separately.

No Formea account is needed. Your plan and workout history stay on your iPhone. Formea Plus is required for workouts and subscriber features. Available subscriptions are weekly and six-monthly; local prices and billing details are shown before purchase. Subscriptions renew automatically unless cancelled. Manage renewal in your Apple Account subscriptions. Deleting the app does not cancel a subscription.

Formea provides general fitness guidance and does not replace medical advice. Results vary; no specific body change is promised.

Privacy: [add verified public URL]
Terms: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/
Membership: [add verified Formea terms URL]

This draft intentionally makes no finished-video claims. Publish only after the actual shipped teaching content is complete and this description accurately describes it.

## Reviewer notes draft

Formea has no account or login. Complete onboarding, then purchase or restore Formea Plus using the review environment to access the app. Both subscription products provide the same features and differ by billing period. DEBUG preview flags are absent from the release purchase flow.

After access, Today starts your next workout; My plan shows four chapters; Progress shows local session history. Daily energy may adapt today's variation. Swap exercise chooses supported alternatives; extra/repeated workouts are recorded separately. Notifications are optional local reminders. No HealthKit, advertising, remote analytics or developer-hosted server is used.

Do not submit these notes while products or teaching content are unfinished. Fill in actual contact details and explain any final non-obvious functionality. No demo login is required because no account system exists; subscriptions still need full reviewer access through working IAP.

## Validation still required

Real-device and TestFlight smoke test; offline/background/pause recovery; VoiceOver and large text; denied reminders; history retention; purchase/refund/restore behavior; live public links; metadata/screenshots consistent with the shipped app; complete archive privacy report. App Store screenshots may include disclosed demonstration data, but must reflect the real product. Approval remains Apple's decision.

Primary sources: [Review Guidelines](https://developer.apple.com/app-store/review/guidelines/) (2.1, 2.3, 3.1.2, 5.1.1), [Privacy details](https://developer.apple.com/app-store/app-privacy-details/), [Support URL requirements](https://developer.apple.com/help/app-store-connect/reference/app-information/platform-version-information/).
