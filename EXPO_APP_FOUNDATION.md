# Jotzi Expo App Foundation

This branch starts the no-Xcode iPhone app path for Jotzi.

## Added on this branch

- `App.tsx` — first React Native screen foundation with Jotzi tabs and approved visual direction.
- `package.json` — npm script shell for Expo.
- `tsconfig.json` — TypeScript project configuration.
- `.gitignore` — ignores local Expo and Node build artifacts.
- `README_EXPO.md` — quick branch summary.
- `docs/EXPO_NO_XCODE_PATH.md` — locks the decision to pause manual Xcode setup.

## Current app tabs

1. Today
2. Loop
3. Garden
4. Memory
5. Recipes
6. Create

## Design direction

The screen foundation uses the approved Jotzi language:

- Cream paper background
- Navy typography
- Peach-gold accents
- Silver sparkle details
- Soft rounded cards
- Magical but practical reminder companion tone

## Important limitation

The current `package.json` intentionally keeps dependencies empty until Expo initializes the exact SDK dependency set locally. This avoids guessing dependency versions.

## Safety

This branch does not start a build, upload to TestFlight, submit to Apple, or merge into `main`.
