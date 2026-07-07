# Jotzi Feature Expansion Roadmap V2

## Purpose
This expands Jotzi from a beautiful reminders app into a premium Apple Watch-first follow-through companion. These features should be considered product candidates, not all mandatory for v1.

## New feature pillars

### 1. Jotzi Compass
A daily navigation screen that answers: “What matters next?”

Inputs:
- Due reminders
- Pinned notes
- Memory Mode notes
- Later Stack
- User energy level
- Optional calendar availability later

Outputs:
- One main next action
- Two small backup actions
- One memory spark
- One thing to defer

Watch version:
- A simple compass ring with North = Next best action
- Digital Crown cycles through directions
- Tap center to start

### 2. Energy-Aware Reminders
Users can set an energy level instead of only a time.

Energy labels:
- Low energy
- Normal
- Focused
- Social
- Errand mode
- Wind-down

Examples:
- “Show this when I have low energy.”
- “Only show this when I’m in Focus mode.”
- “Move chores to a higher-energy window.”

Privacy rule:
Energy state is user-selected first. Do not infer sensitive emotional or health status without explicit opt-in.

### 3. Reminder Difficulty
Every reminder can have a tiny difficulty level.

Levels:
- Tiny
- Easy
- Medium
- Heavy

Use cases:
- Heavy reminders get Help Me Start by default.
- Tiny reminders can be batched.
- Jotzi can warn when a day is overloaded.

### 4. Jotzi Load Meter
A non-stressful meter showing whether the day has too many reminders.

States:
- Light
- Balanced
- Full
- Overloaded

Actions:
- Auto-suggest moving lower-priority reminders
- Convert heavy tasks into tiny steps
- Move items to Later Stack
- Create a recovery day

### 5. Recovery Day
A gentle reset mode for people who fall behind.

Instead of showing an overwhelming backlog, Jotzi offers:
- Keep only essentials today
- Move the rest to tomorrow
- Archive reminders that no longer matter
- Pick one tiny win

Tone:
Supportive, never shame-based.

### 6. Reminder Bundles
Group related reminders together.

Examples:
- Morning routine
- Medication stack
- Study session
- Errand trip
- Pet care
- Work shutdown

Watch behavior:
The bundle shows one card with multiple dots. User completes one step at a time.

### 7. Smart Clustering
Jotzi groups reminders that are close together.

Example:
Instead of five separate alerts:
- Take vitamins
- Drink water
- Pack lunch
- Grab keys
- Start car

Jotzi can show:
“Morning launchpad — 5 quick things.”

### 8. Launchpad Mode
A special bundle style for starting or leaving.

Launchpads:
- Morning Launchpad
- Leaving Home
- Arriving Work
- Evening Shutdown
- Bedtime Winddown

Each launchpad has a clean checklist and one Watch haptic cue.

### 9. Watch Gesture Shortcuts
Use fast Watch interactions for low-friction control.

Possible gestures, depending on platform support:
- Tap orb: open note
- Double tap: mark done where supported
- Long press: snooze reasons
- Crown turn: cycle notes
- Swipe left: skip
- Swipe right: tiny step

Implementation must respect watchOS APIs and device support.

### 10. Haptic Language
A branded haptic design system using supported Watch haptics.

Examples:
- Gentle pulse: normal reminder
- Bright tap: completed
- Soft double tap: memory spark
- Firm tap: due now
- Quiet cue: wind-down reminder

Constraint:
Do not promise arbitrary background haptic patterns. Use supported system notification haptics and active-app WatchKit haptics.

### 11. Jotzi Journal
A lightweight reflection layer tied to reminders.

Features:
- “What did you finish?”
- “What kept coming back?”
- “What should Jotzi stop reminding you about?”
- Weekly summary
- Convert journal insight into a note or Memory Spark

### 12. Forget Me Not Mode
A mode for important things that should never disappear but also should not annoy.

Examples:
- Door code
- Parking spot
- Hotel room
- Person’s name
- Gift idea
- Important boundary

Behavior:
- Lives on Pinboard
- Can appear as Watch complication
- Can expire automatically
- Can be locked/private

### 13. Expiring Notes
Notes can self-expire.

Use cases:
- Parking spot expires tonight
- Door code expires after trip
- Grocery reminder expires tomorrow
- Event prep expires after event

Actions:
- Expire
- Archive
- Ask before deleting

### 14. Note Privacy Lock
Certain notes can be private.

Possible protections:
- Face ID on iPhone
- Hide on Watch complications
- Show only title placeholder
- Disable notification preview

Examples:
- Health notes
- Personal reminders
- Sensitive memory notes

### 15. “Nudge Me Until” Rules
A reminder can persist until a specific outcome.

Examples:
- Until I mark done
- Until tonight
- Until I leave home
- Until three checkbacks are ignored
- Until I archive it

This is more nuanced than repeating forever.

### 16. Reminder Health Check
Jotzi can review stale reminders.

Questions:
- Still important?
- Make smaller?
- Move to later?
- Delete?
- Turn into Memory Spark?

This keeps the app clean over time.

### 17. Capture from Share Sheet
User can send text, links, screenshots, or selected content into Jotzi.

Actions:
- Save as note
- Remind me later
- Add to Pinboard
- Turn into Memory Spark
- Add to a bundle

### 18. Screenshot Reminder
User can create a reminder from a screenshot.

Examples:
- Screenshot an address
- Screenshot an item to buy
- Screenshot a text conversation
- Screenshot a recipe

Jotzi attaches the image to the reminder and can optionally ask for a short title.

### 19. Contact-Aware Reminders
Optional contact-based reminders without creepy tracking.

Examples:
- “Ask Mom about the appointment”
- “Text Alex the photo”
- “Bring this up with Sam”

Features:
- Link reminder to a contact
- Quick call/text action
- No hidden contact scanning

### 20. Kindness Mode
A tone setting that changes reminder wording.

Modes:
- Direct
- Gentle
- Playful
- Minimal

Examples:
Direct: “Take vitamins.”
Gentle: “Time for your vitamins when you’re ready.”
Playful: “Tiny health win waiting.”
Minimal: “Vitamins.”

### 21. Reward Moments
Small delight moments after completions.

Examples:
- Sparkle burst
- Note spirit dance
- Garden growth
- Soft success phrase
- Watch ring glow

Rule:
Keep rewards fast and tasteful.

### 22. Jotzi Inbox Zero
A weekly cleanup ritual.

Sections:
- Unscheduled notes
- Repeatedly snoozed notes
- Expired notes
- Heavy reminders
- Pinboard candidates

Goal:
Keep Jotzi useful, not cluttered.

### 23. Smart Defaults
Jotzi learns the user’s preferred defaults locally.

Examples:
- Default snooze duration
- Favorite categories
- Usual active hours
- Preferred checkback delay
- Most-used recipe

### 24. Apple Focus Integration Plan
Future optional integration with Focus modes.

Use cases:
- Quiet reminders during Sleep Focus
- Work reminders during Work Focus
- Personal reminders after Work Focus ends

Must respect Apple platform constraints and user permission.

### 25. Travel Mode
Temporary reminder behavior for trips.

Features:
- Time-zone aware reminders
- Hotel room / parking / gate notes
- Packing list bundle
- Expiring travel notes
- Quiet mode during flights or sleep hours

### 26. Care Mode
A gentle mode for caring for another person or pet.

Examples:
- Pet medication
- Check on parent
- Water plants
- Pick up prescription

Includes:
- Shared nudges later
- Checkback confirmation
- Sensitive-note privacy

### 27. Watch Face Mood States
The watch home can visually represent reminder status.

States:
- Calm: no urgent notes
- Glow: upcoming note
- Pulse: due now
- Bloom: completed streak
- Moon: quiet hours
- Cloud: overloaded day
- Spark: Memory Mode note

### 28. “One Thing” Mode
Jotzi can hide everything except one chosen task.

Useful for:
- ADHD-friendly focus
- Overwhelm reduction
- Heavy reminders
- Morning start

Watch UI:
One orb, one tiny step, one action.

### 29. Reminder Replay
At the end of the day, replay what happened.

Shows:
- Completed
- Snoozed
- Moved
- Ignored
- Actually completed after checkback
- Best time window

This feeds adaptive timing.

### 30. Jotzi Labs
A hidden/optional area for experimental features.

Examples:
- New watch faces
- New spirits
- Experimental recipes
- Alternative scoring models
- Beta notification behaviors

Purpose:
Allow innovation without destabilizing the core app.

## Updated Pro feature candidates
Strong Pro candidates:
- Jotzi Loop advanced learning
- Jotzi Garden
- Note Spirits
- Pro Watch faces
- Reminder Bundles
- Smart Clustering
- Launchpad Mode
- Privacy Lock
- Expiring Notes
- Travel Mode
- Care Mode
- Advanced Reminder Replay

## Updated v1 focus recommendation
The best v1 should include:
1. Beautiful Today and Inbox
2. Create/edit reminder
3. Apple Watch home
4. Done / Snooze / Skip / Later
5. Jotzi Loop basic
6. Memory Mode basic
7. Pinboard basic
8. Reminder Recipes starter pack
9. Privacy/legal foundation
10. Polished design and haptics

Do not overload v1 with every advanced feature. Use this roadmap to build a premium product over versions.
