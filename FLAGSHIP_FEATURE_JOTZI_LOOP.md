# Jotzi Loop — Flagship Differentiator

## Product idea
Jotzi Loop is a wrist-first reminder system that does more than fire an alert. It helps the user actually follow through, learns the moments that work best for that person, and confirms whether a task was truly completed.

## Why it is different
Most competing Apple Watch note and reminder apps focus on capture, lists, recurrence, snooze, widgets, complications, or repeated alerts. Jotzi Loop combines four behaviors into one private, on-device workflow:

1. Adaptive resurfacing
2. One-tap snooze reasons
3. Completion checkback
4. A two-minute starter action

## User flow

### 1. Reminder arrives
The watch presents:
- Done
- Snooze
- Not now
- Help me start

### 2. If the user snoozes
Jotzi asks for one optional reason:
- Busy
- Not here
- Need more time
- Waiting on someone
- Wrong time

The answer takes one tap and is stored locally.

### 3. Jotzi adapts
After repeated behavior, Jotzi can suggest:
- “You usually complete this after 7 PM. Move it?”
- “You snooze this at work. Remind you when you leave?”
- “This reminder works better on weekends.”
- “You complete this faster after a 10-minute warning.”

No cloud AI is required. Suggestions should be generated from local reminder history.

### 4. Help me start
For reminders that feel too large, Jotzi converts the note into a tiny first action, such as:
- “Open the document.”
- “Put the shoes by the door.”
- “Write the first sentence.”
- “Take the bottle out.”

The first action should take about two minutes or less. The user can accept, edit, or dismiss it.

### 5. Completion checkback
For selected reminders, tapping Done does not end the workflow immediately. Jotzi asks later:
- “Did this actually get done?”

Responses:
- Yes
- Not yet
- Partly
- Skip checkback

This prevents accidental dismissal and separates “tapped Done” from “actually completed.”

## Memory Mode
Jotzi Loop also supports non-task notes that should gently return throughout the day:
- Affirmations
- Personal boundaries
- Important thoughts
- Instructions
- Names or facts to remember
- Motivation

Memory Mode can show a note a selected number of times during active hours without requiring an exact time.

## Watch experience
- Large one-tap actions
- No typing required for common responses
- Optional dictation for custom reasons
- Haptic-first presentation using system-supported watchOS notifications
- Local watch scheduling where appropriate
- Works offline and syncs later

## Privacy
- Learning is local-first
- No behavioral advertising
- No sale of reminder history
- No remote AI required
- User can reset learned timing suggestions at any time
- Suggestions remain optional

## Settings
- Enable or disable Jotzi Loop globally
- Enable per reminder
- Choose checkback delay
- Choose persistence level: Gentle, Standard, Persistent
- Disable learning for selected categories
- Reset learned patterns
- Set quiet hours

## Technical constraints
- Background reminder delivery must use supported local or remote notifications.
- Custom haptic sequences must not be promised where watchOS only allows system-defined haptic behavior.
- In-app haptics may use supported WatchKit haptic types while the app is active.
- The system must avoid notification spam, battery drain, and repeated alerts during Focus or quiet hours.

## Success metrics
- Percentage of reminders actually completed
- Reduction in repeated snoozes over time
- Percentage of accepted timing suggestions
- Percentage of checkbacks confirming real completion
- User-controlled notification burden

## App Store positioning
**Jotzi Loop — reminders that learn when you actually follow through.**

This should be presented as Jotzi’s flagship feature and a primary Pro benefit after the core reminder experience is stable.
