# Jotzi — Apple Privacy Nutrition Label Draft

Publisher: Ocoee Studios LLC  
App: Jotzi  
Current state: Expo prototype / pre-native HealthKit integration

## Current draft answer

For the current prototype, if the app has:
- no production backend,
- no user accounts,
- no ads,
- no analytics SDK,
- no third-party tracking,
- no real HealthKit connection,
- no real Face ID storage,
- no cloud sync,

then the App Store Connect privacy answer is likely:

**Data Collection: No, this app does not collect data from users.**

## Important future changes

This answer must be reviewed before App Store submission if any of the following are added:

- HealthKit access
- Apple Watch companion data
- push notifications
- RevenueCat or subscriptions
- analytics
- crash reporting tied to users
- cloud sync
- accounts/login
- email collection
- support forms
- advertising or tracking SDKs

## HealthKit positioning

If HealthKit is implemented later:
- request user permission before reading HealthKit data,
- use health data only for reminder timing/context,
- do not sell health data,
- do not use health data for advertising or tracking,
- clearly explain HealthKit use in the privacy policy and App Store privacy responses.

## Face ID / Vault positioning

If biometric Vault unlock is implemented later:
- Face ID should be handled by Apple device APIs,
- biometric identity data should not be collected by Ocoee Studios LLC,
- Vault content storage must be reviewed separately depending on whether it is local-only or synced.

## App Store Connect wording

Suggested short description:

Jotzi is a gentle reminder companion. The current version stores reminder and preference information locally on device. Jotzi does not sell user data. Future HealthKit or Apple Watch features will require user permission before accessing health-related information.
