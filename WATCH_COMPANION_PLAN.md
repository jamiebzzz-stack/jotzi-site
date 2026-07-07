# Jotzi Apple Watch Companion Plan

Jotzi will launch the iPhone Expo / React Native app first. The Apple Watch companion will come later as a native watchOS extension once the iPhone app foundation is stable.

## Current Status

- iPhone app: Expo / React Native foundation in progress.
- Watch app: Not built yet.
- Xcode/manual native setup: Paused for now.
- EAS/TestFlight/App Store: Not started.
- Draft PR remains unmerged.

## Product Goal

The Apple Watch companion should make Jotzi feel like a gentle wrist-based reminder spirit.

The Watch app should focus on:

- quick glance reminders
- soft haptic nudges
- simple note capture
- Jotzi Loop progress
- lightweight completion actions
- quiet, non-annoying reminder behavior

The Watch app should not try to duplicate the full iPhone app.

## Watch Experience Principles

1. **Fast**
   - A user should understand the next reminder in under 2 seconds.

2. **Gentle**
   - Haptics should feel soft, supportive, and optional.

3. **Minimal**
   - Watch screens should be small, clear, and focused.

4. **Magical**
   - The visual language should match Jotzi: dark navy, cream text, gold glow, soft spirits.

5. **Respectful**
   - Quiet Hours and notification preferences should matter.

## Proposed Watch Screens

### 1. Today Glance

Shows the next few reminders.

Possible elements:

- Jotzi mini logo
- next reminder title
- due time
- tiny spirit
- complete button
- snooze / later button

### 2. Jotzi Loop

Shows reminder growth progress.

Possible elements:

- small orbit ring
- current loop stage
- progress text
- simple completion action

Stages:

- Capture
- Time it right
- Complete
- Grow & glow

### 3. Quick Capture

Lets the user capture a small reminder or note from the Watch.

Possible inputs:

- dictation
- quick preset
- emoji/mood-style memory spark
- “remind me later” shortcut

### 4. Memory Spark

A lightweight moment capture screen.

Possible actions:

- save a small thought
- star a memory
- send to iPhone for richer editing

### 5. Settings Lite

Only the essentials on Watch:

- haptics on/off
- quiet mode
- app info
- open full settings on iPhone

## Haptic Direction

Jotzi haptics should feel soft and intentional.

Possible haptic categories:

- gentle reminder pulse
- completion sparkle
- quiet nudge
- urgent reminder, used rarely
- loop growth confirmation

The default should never feel aggressive.

## iPhone / Watch Relationship

The iPhone app remains the source of truth for:

- reminder creation
- theme and font settings
- privacy / terms / support
- recipe templates
- richer Memory Sparks
- full Jotzi Garden view

The Watch companion focuses on:

- glance
- nudge
- complete
- snooze
- capture

## Data Sync Plan

Later native implementation should support syncing:

- reminders
- completion state
- Jotzi Loop progress
- quiet hours
- haptic preference
- theme preference
- quick-captured notes

The initial implementation can start with a small local mock model before deeper sync is added.

## Native Build Notes

The watchOS companion will require native Apple tooling later.

Planned later work:

1. Add native iOS/watchOS project path.
2. Add watchOS target.
3. Build simple Watch UI.
4. Connect basic data bridge between iPhone and Watch.
5. Add haptic behaviors.
6. Test on physical Apple Watch.
7. Only then consider TestFlight/App Store workflow.

## Do Not Do Yet

Do not start any of this without explicit approval:

- no EAS builds
- no TestFlight upload
- no App Store submission
- no production build
- no PR merge
- no native Watch setup until the iPhone app foundation is ready

## Open Questions

- Should Jotzi Watch support complication widgets?
- Should the first Watch version be reminder-only, or include quick capture?
- Which haptic patterns feel best for the brand?
- Should the Watch use the same spirits, simplified spirits, or custom tiny Watch spirits?
- Should Quiet Hours sync from iPhone settings or be Watch-specific?
- Should the Watch support offline capture when away from the phone?

## Recommended Build Order

1. Finish iPhone Expo app foundation.
2. Make Settings functional enough for themes, fonts, legal, support, and haptics preferences.
3. Define reminder data model.
4. Add local reminder interactions on iPhone.
5. Add Watch companion spec and mock screens.
6. Only then begin native watchOS implementation.
