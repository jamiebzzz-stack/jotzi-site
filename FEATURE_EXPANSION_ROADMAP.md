# Jotzi 10/10 Feature Expansion Roadmap

## Product goal
Make Jotzi feel like a premium, delightful, Apple Watch-first notes and reminders companion that does more than remind. Jotzi should help users capture, remember, start, follow through, reflect, and build gentle daily rhythm.

## Design rule
Every feature must pass three tests:
1. It makes reminders easier to act on.
2. It feels useful on Apple Watch, not just iPhone.
3. It does not create notification stress or visual clutter.

## Flagship feature stack

### 1. Jotzi Loop
Already locked as the flagship system.
- Snooze reasons
- Adaptive timing suggestions
- Help Me Start
- Completion checkbacks
- Memory Mode
- Local-first learning

### 2. Living Watch Face
A playful Watch home inspired by mood/status watch apps, but about notes.
- Large colorful note orb
- Progress ring
- Sparkles and small motion
- Remaining-note counter
- Tap to cycle notes
- Done button
- Category-based colors
- Complication-friendly status

### 3. Note Pets / Note Spirits
A collectible visual layer for Watch and iPhone.

Each category can have a tiny animated “note spirit”:
- Work: little briefcase sprite
- Health: little heart or leaf sprite
- Personal: little star sprite
- Errands: little running note sprite
- Memory Mode: moon or sparkle sprite

Behavior:
- Spirits wake up when a note is due.
- They calm down when completed.
- They gently sparkle when a streak is maintained.
- They never shame the user for missing a reminder.

Purpose:
Make reminders emotionally sticky without turning the app into a game that feels childish.

### 4. Jotzi Garden
A gentle completion visualization.

Instead of streak pressure, completed notes grow a small garden/starfield.
- Each completed reminder plants a star, flower, leaf, or light.
- Weekly view shows a constellation or garden path.
- Missed days do not punish the user.
- Memory Mode notes can become stars.
- Health routines can grow leaves.

This creates a beautiful reason to return to the app.

### 5. Smart Resurface
A note can come back only when it makes sense.

Signals:
- User’s chosen active hours
- Prior completion patterns
- Snooze reasons
- Calendar-free blocks if permission is added later
- Location only if optional location reminders are enabled
- Focus and quiet hours

Examples:
- “This was snoozed as Busy three times. Try after work?”
- “You usually complete this on Sunday morning.”
- “This note has not been seen in 2 weeks. Bring it back?”

### 6. Tiny Steps Mode
A structured version of Help Me Start.

User can break a note into tiny steps:
- Step 1: Open the document
- Step 2: Write first sentence
- Step 3: Send draft

Watch view:
- One tiny step at a time
- Done / Next / Pause
- Progress ring advances per step

### 7. Voice-to-Loop Capture
User dictates a thought and Jotzi turns it into a structured reminder.

Examples:
- “Remind me to call Mom after work tomorrow”
- “Keep reminding me to drink water today”
- “Show me this affirmation three times a day”
- “Remind me to check in on how I feel every night”

Implementation rule:
Start with deterministic natural-language parsing. Do not require cloud AI for core reminders.

### 8. Pinboard
A beautiful home for notes that are not tasks.

Use cases:
- Affirmations
- Boundaries
- Names
- Addresses
- Door codes
- Ideas
- Things to remember

Features:
- Pin to Watch
- Pin to widget
- Show in Memory Mode
- Convert to reminder
- Archive when no longer needed

### 9. Jotzi Pulse
A quick daily check-in layer.

Prompt examples:
- “What should Jotzi help you remember today?”
- “What feels important?”
- “What are you avoiding?”
- “What is one tiny win?”

Outputs:
- Creates notes/reminders
- Feeds Memory Mode if user chooses
- Shows weekly reflection summary

### 10. Reminder Recipes
Pre-built packs that help users start fast.

Packs:
- Medication and supplements
- Hydration
- ADHD-friendly morning routine
- Evening reset
- Workday focus
- Errand day
- Self-care
- Pet care
- Family reminders
- Study routine

Each recipe can create a bundle of reminders with editable times.

### 11. Gentle Accountability
A non-shaming follow-through system.

Instead of “failed” language:
- “Still worth doing?”
- “Try a smaller step?”
- “Move it to tomorrow?”
- “Archive for now?”

This should be a core tone principle across the app.

### 12. Shared Nudges
Optional shared reminder loops for trusted people.

Use cases:
- Family errands
- Partner reminders
- Caregiving support
- Team personal reminders

Rules:
- Not a surveillance tool
- No hidden tracking
- Clear invite and consent
- User controls every shared note

### 13. Focus Bubbles
A session mode for notes that need attention.

User chooses one note and enters a timed focus bubble.
- 5, 10, 15, 25 minutes
- Watch shows only that note
- Haptic end cue
- Option to mark partial progress

### 14. Later Stack
A better “not now” system.

Instead of burying snoozed reminders, Jotzi creates a Later Stack.
- Later today
- Tomorrow
- Weekend
- When I have energy
- When I am home
- Someday

The app periodically asks the user to clean the stack gently.

### 15. Memory Sparks
Short notes that appear like thought bubbles.

Good for:
- Motivational phrases
- Spiritual reminders
- Therapy notes
- Names
- Study facts
- Personal promises

Modes:
- Morning spark
- Midday spark
- Evening spark
- Random within active hours

### 16. Watch Complication Personality
Complications should feel alive without being distracting.

States:
- Calm: no urgent notes
- Glow: upcoming reminder
- Pulse: due now
- Sparkle: completed streak
- Moon: quiet hours
- Leaf: health note
- Star: Memory Mode note

### 17. Privacy Dashboard
A clear in-app dashboard that shows:
- Notifications enabled/disabled
- Watch sync status
- iCloud sync status
- HealthKit status
- Location reminder status
- Siri/App Intents status
- Data deletion controls

This supports trust and helps App Review.

### 18. Pro Themes
Premium visual themes.

Possible themes:
- Classic Jotzi: cream, navy, peach-gold
- Midnight Notes: deep navy and silver
- Garden Glow: green and gold
- Rose Quartz: blush and cream
- Focus Ember: orange and charcoal
- Moonlit: blue, silver, and lavender

### 19. Apple Watch Crown Navigation
Use the Digital Crown to cycle through notes, tiny steps, or pinned memories.

Actions:
- Crown scrolls note orbit
- Tap center to open
- Swipe for actions
- Long press for snooze reasons

### 20. Jotzi Score — but not stressful
A gentle “follow-through” status, not a grade.

Possible labels:
- Flowing
- Light day
- Building momentum
- Needs trimming
- Overloaded

Purpose:
Help users notice when they have too many reminders and reduce overload.

## Free vs Pro recommendation

### Free
- Core notes and reminders
- Basic Watch app
- Basic widgets
- Limited active notes
- Basic repeating reminders

### Pro
- Jotzi Loop
- Memory Mode
- Tiny Steps Mode
- Jotzi Garden
- Reminder Recipes
- Advanced complications
- Pro themes
- Shared nudges
- HealthKit integrations
- Location reminders
- Advanced history and reflections

## Build priority

### Phase 1 — Foundation
- Jotzi Loop core engine
- Reminder models
- SwiftUI iPhone preview screens
- SwiftUI Watch home prototype
- Local persistence

### Phase 2 — Daily usability
- Create/edit reminders
- Today timeline
- Inbox
- Watch Done/Snooze/Skip
- Notification actions
- Basic widgets

### Phase 3 — Differentiators
- Living Watch Face
- Memory Mode
- Help Me Start
- Completion checkbacks
- Tiny Steps
- Reminder Recipes

### Phase 4 — Delight and retention
- Jotzi Garden
- Note Spirits
- Pro themes
- Watch complication personality
- Jotzi Pulse

### Phase 5 — Advanced optional systems
- HealthKit
- Location reminders
- Shared nudges
- Siri/App Intents
- Privacy Dashboard

## Release gate
Do not add all features to v1 if it makes the app bloated. The best v1 should feel polished, clear, fast, and magical. Jotzi Loop, Watch home, reminders, and basic Memory Mode matter more than shipping every advanced feature at once.
