# Jotzi Product Specification

## Product vision
Jotzi is a premium iPhone and Apple Watch app for personal notes, gentle reminders, haptic nudges, affirmations, check-ins, and recurring prompts throughout the day.

Tagline: **Reminders That Stick**

## Core platforms
- iPhone app
- Apple Watch companion app
- Apple Watch complications and Smart Stack widgets
- iPhone Home Screen and Lock Screen widgets

## iPhone app features

### Onboarding
- Brand-led onboarding
- Explain notes, haptics, watch syncing, and reminders
- Notification permission setup
- Optional iCloud sync setup
- Watch pairing guidance

### Today
- Timeline of all reminders and notes scheduled for today
- Next reminder card
- Progress for completed notes
- Quick complete, snooze, skip, and reschedule actions
- Filter by category, priority, and status

### Inbox
- Unscheduled notes
- Fast capture from text or voice
- Convert an inbox note into a timed, recurring, pinned, or throughout-the-day reminder

### Create and edit note
Each note can include:
- Title
- Additional details
- Category
- Custom color
- Priority
- Date and time
- Repeat rule
- Active hours
- Number of reminders per day
- Pinned status
- Watch notification toggle
- Sound and haptic preference
- Snooze options
- Optional location trigger
- Optional voice note

### Reminder types
- One-time reminder
- Daily reminder
- Weekday reminder
- Weekend reminder
- Weekly reminder
- Selected weekdays
- Custom interval
- Every few hours
- Multiple times throughout the day
- Randomly spaced encouragements within active hours
- Pinned note
- Check-in prompt

### Note management
- Create
- Edit
- Duplicate
- Archive
- Delete
- Search
- Filter
- Sort
- Mark complete
- Restore completed notes
- Completion history
- Snooze history

### Check-ins
- Custom questions such as “How are you feeling?”
- Quick responses
- Optional notes
- Daily and weekly history
- Simple trend view

### Categories
- Personal
- Work
- Health
- Medication
- Errands
- Motivation
- Custom categories

### Settings
- Notification preferences
- Haptic intensity preference where supported
- Default snooze duration
- Active hours
- Appearance
- iCloud sync status
- Watch connection status
- Privacy controls
- Subscription management

## Apple Watch app features

### Watch home
- Next note
- Time until next reminder
- Notes remaining today
- Quick add button

### Today list
- Scrollable list of today’s reminders
- Priority and category indicators
- Completed state

### Reminder actions
- Done
- Snooze 10 minutes
- Snooze 30 minutes
- Snooze 1 hour
- Later today
- Skip
- Reschedule

### Quick capture
- Dictate a new note
- Add from preset timing buttons
- In 15 minutes
- In 1 hour
- Tonight
- Tomorrow
- When I get home

### Watch-only behavior
- Offline access to synced reminders
- Queue updates until the phone reconnects
- Local watch notifications where appropriate
- Haptic-first reminder experience

### Complications and Smart Stack
- Next reminder
- Number of notes remaining
- Quick add
- Pinned note

## Notifications
- iPhone and Watch notification support
- Interactive actions
- Duplicate-notification prevention
- Reliable rescheduling after edits
- Time-zone aware behavior
- Quiet hours support

## Sync and data
- Local-first storage
- iCloud sync
- iPhone–Watch synchronization
- Conflict handling
- Sync status indicators
- No account required for core use

## Voice and system integrations
- Siri and App Intents support
- Dictated note creation
- “Remind me…” natural-language shortcuts
- Spotlight indexing where appropriate

## Widgets
### iPhone
- Next reminder
- Today progress
- Quick add
- Pinned note

### Apple Watch
- Circular complication
- Rectangular complication
- Corner complication where supported
- Smart Stack widget

## Monetization

### Free
- Up to 5 active notes
- Basic timed reminders
- Basic repeating reminders
- iPhone and Watch syncing
- Basic widgets

### Pro
- Unlimited active notes
- Throughout-the-day reminders
- Random spacing within active hours
- Advanced recurrence
- Location reminders
- Voice notes
- Check-in history
- Advanced widgets and complications
- Custom categories and colors
- Shared reminders if added later

## Privacy
- Notes private by default
- No advertising
- No sale of personal data
- Minimal analytics
- Clear notification and iCloud explanations

## Design direction
- Premium, dreamy, elegant, and tactile
- Cream, navy, silver, and subtle peach-gold palette
- Old English J mark
- Fine stardust and restrained sparkle
- Watch-first clarity with large tap targets
- Avoid visual clutter in reminder screens

## Technical direction
- Native Apple architecture for watchOS support
- SwiftUI for iPhone and Apple Watch interfaces
- SwiftData for local persistence
- CloudKit for iCloud sync
- WatchConnectivity for immediate device communication
- UserNotifications for scheduling and actions
- WidgetKit for complications and widgets
- StoreKit 2 for subscriptions
- App Intents for Siri and shortcuts

## Release rule
Do not begin production builds, TestFlight submission, or App Store submission until the complete feature audit, device QA, notification QA, sync QA, and subscription QA are finished.
