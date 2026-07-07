# Jotzi HealthKit and App Privacy Specification

## HealthKit purpose
HealthKit is optional. Jotzi may use it only for user-requested wellness reminders and completion logging, such as hydration, mindfulness, movement, sleep-related routines, and other supported HealthKit data types that are explicitly approved during implementation.

## Rules
- Never require HealthKit for the core notes and reminders experience.
- Request permission only when the user turns on a specific Health feature.
- Request each HealthKit data type separately and explain why it is needed.
- Do not use HealthKit data for advertising, profiling, data brokerage, or unrelated analytics.
- Do not sell or share HealthKit data.
- Store the minimum data necessary.
- Keep HealthKit-derived information on-device and in the user’s private iCloud scope unless Apple’s rules and the user’s explicit consent permit otherwise.
- Do not present Jotzi as diagnosing, treating, curing, or preventing disease.
- Do not make medication adherence or emergency claims.
- Provide clear deletion and disconnect controls.

## Proposed Health features
- Hydration reminder completion logging
- Mindfulness reminder completion logging
- Movement or stand reminder completion logging
- Sleep routine reminders based on user-selected schedules
- Optional read-only context for supported HealthKit metrics
- Optional write-back only when the user deliberately confirms completion

## Authorization UX
1. Explain the feature before showing Apple’s permission sheet.
2. State exactly which data type is requested.
3. Explain whether Jotzi reads, writes, or both.
4. Provide a useful non-HealthKit fallback if permission is denied.
5. Never repeatedly pressure users to enable access.

## App Privacy nutrition label draft
Final answers must be based on the shipped code and all third-party SDKs.

### Expected disclosures for a privacy-first build
- Health & Fitness: collected only if HealthKit features are enabled; linked to the user only where technically necessary; not used for tracking.
- User Content: note text, reminder details, voice-note content, and check-in responses; used for app functionality; not used for tracking.
- Identifiers: avoid collecting persistent external identifiers unless required for account or purchase functionality.
- Purchases: subscription status handled by StoreKit; disclose only what the production implementation actually collects.
- Diagnostics: disclose crash or performance data only if a diagnostics SDK is included.
- Location: disclose only if optional location reminders ship.

## Required implementation artifacts
- HealthKit entitlement
- Health share usage description
- Health update usage description, if writing data
- Privacy policy URL
- App Privacy answers in App Store Connect
- In-app Health data disclosure
- Health data deletion/disconnect controls
- QA matrix for permission-denied, partial-permission, and revoked-permission states

## Release gate
No HealthKit capability may ship until the exact data types, purpose strings, storage paths, privacy label answers, and review notes are audited against the final binary.
