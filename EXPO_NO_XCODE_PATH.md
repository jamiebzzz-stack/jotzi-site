# Jotzi Expo Path — No Xcode For Now

This file locks the updated development path after the manual Xcode setup proved too difficult.

## Current decision

We are pausing manual Xcode work and building the iPhone app foundation with Expo / React Native first.

This does **not** abandon Jotzi.

It only changes the build path:

- Build the iPhone app experience first with Expo / React Native.
- Keep GitHub as the source of truth.
- Keep the approved Jotzi brand direction.
- Keep the Jotzi Loop / Garden / Memory Sparks / Recipes feature direction.
- Avoid manual Xcode project setup for now.
- Add the Apple Watch native companion later when the iPhone app is stable.

## Safety rules

Do not do any of the following without explicit approval:

- Do not submit to TestFlight.
- Do not submit to the App Store.
- Do not run a production EAS build.
- Do not merge draft PRs into `main` without approval.
- Do not replace the approved Jotzi brand direction.

## Recommended Expo creation path

Use the official Expo starter rather than hand-writing dependency versions:

```bash
npx create-expo-app@latest --template default@sdk-57
```

Then move the generated app files into this repository or create them directly on this branch.

## Initial iPhone app scope

The first Expo version should include:

1. Today tab
2. Jotzi Loop tab
3. Garden tab
4. Memory Sparks tab
5. Reminder Recipes tab
6. Create / Quick Add tab
7. Approved cream/navy/peach-gold/silver Jotzi styling
8. Local reminder mock data
9. No account requirement
10. No Apple Watch native target yet

## Apple Watch note

Expo is the easiest route for the iPhone app, but a real Apple Watch companion will still require native watchOS/Xcode later. That step should happen only after the iPhone app shell is solid.
