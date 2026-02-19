# Changelog v2.0.1

## [2.0.1] - 2026-02-20

### Added
- Dedicated redirect handler for Google Authentication
- "What's New" release highlights for v2.0.1
- Archival support for mock data in mockData.ts

### Fixed
- Android Google Auth redirect
- Data persistence issue where mock data reappeared
- "Clear All Data" button immediately refreshing UI
- "This screen doesn't exist" error during OAuth

### Updated
- Global app state management to prioritize user data over sample data
- Transitioned seeder to non-functional stub (archived to separate file)
- Refined dashboard navigation after data wipes

### Removed
- Automatic seeding of mock data on app startup
- Overwriting of local database with sample data during initialization


# Changelog v2.0.1

## [2.0.1] - 2026-02-20

### Added
- Fix Google Account Connection Issue


# Changelog

All notable changes to the Cinema Lobby App are documented here.  
Format based on [Keep a Changelog](https://keepachangelog.com/).

## [2.0.0] - 2026-02-20

### Added
- **Major Architecture Upgrade**: Full version 2.0.0 release with optimized background sync and modular database structure.
- **Enhanced Activity Log Sync**: Your full machine activity history (actions, staff names, and setting changes) now syncs across all devices via Google Drive for unified multi-device management.
- **Service Report Updates**: All status changes and notes in service reports are now tracked and synced for complete maintenance history.
- **Tactical Splash Screen**: Integrated a high-fidelity "Initialize System" dashboard for a premium, futuristic launch experience.
- **Glowing App Icon**: Refined brand identity with a high-contrast glowing blue robotic arm logo.
- **Smart Session Management**: Enhanced Google login to automatically refresh your session, reducing the need to sign in repeatedly.
- **Connection Status**: Added a visual status indicator in Settings to show your current connection health.
- **Inventory Audit**: Inventory updates now track and log exact quantity changes (previous vs. new) for better history tracking.
- **Image Organization**: Photos are now automatically sorted into specific folders (Inventory, Machine Photos, Reports) in Google Drive.

### Fixed
- **Android Splash Fix**: Resolved issues where the splash screen appeared too small on high-density Android displays.
- **Build Optimization**: Drastically reduced APK size through R8 minification and architecture-specific filtering.
- **Splash Persistence**: Resolved native caching issues to ensure the new branding appears immediately.
- **Data Validation**: Added checks to prevent accidental entry of invalid inventory quantities.
- **Sync Reliability**: Improved image synchronization to ensure files are routed to their correct destinations.

## [1.8.0] - 2026-02-19

### Added
- **Activity Log Sync**: Your full machine activity history (actions, staff names, and setting changes) now syncs across all devices via Google Drive.
- **Service Report Updates**: All status changes and notes in service reports are now tracked and synced for complete cross-device maintenance history.
- **Tactical Splash Screen**: Integrated a high-fidelity "Initialize System" dashboard to create a premium, futuristic launch experience.
- **Glowing App Icon**: Optimized the brand identity with a high-contrast glowing blue robotic arm logo.

### Fixed
- **Build Optimization**: Drastically reduced APK size by over 60% through R8 minification and architecture-specific filtering.
- **Splash Persistence**: Fixed an issue where the old splash screen would linger in native caches on iOS.

## [1.7.0] - 2026-02-19
### Added
- **Final Premium Branding**: Integrated the cinematic "Tactical Dashboard" splash screen and the refined "Glowing Blue Claw" app icon.
- **Improved Launch Experience**: Optimized splash screen for all device sizes with a solid dark theme (#0A111A).

## [1.6.0] - 2026-02-19
### Added
- **Enhanced Chart Tooltips**: Tap any chart point to see Plays, Revenue, and Wins for that day. 
- **"What's New" Modal**: After each update, see a beautiful summary of what's been added and improved.
- **Full Version History**: Comprehensive changelog now maintained with every release.

## [1.5.0] - 2026-02-19

### Added
- **Machine Selection Shortcuts** — Deep-link from machine detail to submit settings / play record with auto-selection.
- **Change Item with Warning** — "Change" button on machine prize card with confirmation alert before navigating to setup form.
- **Upcoming Inventory Suggestion** — Banner in settings form to quick-assign the upcoming item configured for the machine.
- **Activity Log Detail View** — Expandable log entries showing full metadata, timestamps, and parsed detail JSON.
- **Activity Log Search** — Debounced search bar filtering by action, staff name, and type.
- **Dashboard Date Range Chips** — 7D / 14D / 30D / All filter for revenue, plays, and per-machine breakdowns.
- **Enhanced Chart Tooltips** — Tapping a chart point shows Plays, Revenue, and Wins for that specific day.
- **"What's New" Modal** — In-app overlay highlights new features after each update.

### Verified (Already Implemented)
- Negative inventory option (#8)
- Machine archive / restore (#10)
- Service report status timeline (#23)

## [1.4.0] - 2026-02-19

### Added
- Smart history browsing with 50-record pagination and quick-select date range chips.
- Animated skeleton loading screens for history views.
- Full-screen image preview for history items.

### Fixed
- Google Drive sharing links now render correctly in history.
- Machine quantity displays show live stock levels (COALESCE fix).
- Machine attention alerts require minimum plays threshold.
- Service report error handling and empty-state feedback.

## [1.3.0] - 2026-02-19

### Added
- Smart session management with automatic refresh.
- Connection status indicator in Settings.
- Inventory audit trail (previous vs. new quantity tracking).
- Automatic image folder organization on Google Drive.

### Fixed
- Data validation for inventory quantities.
- Image sync routing reliability.

## [1.2.0] - 2026-02-19

### Changed
- Maintenance and stability improvements.

## [1.1.9] - 2026-02-19

### Changed
- General update and improvements.

## [1.1.8] - 2026-02-19

### Fixed
- Google Drive image upload collision (unique filenames).
- Machine image updates during Drive fetch.
- `=IMAGE()` formula detection in spreadsheets.
- Historical record protection during full sync on new devices.

## [1.1.7] - 2026-02-19

### Added
- Manual "Check for Updates" button in Settings.

### Fixed
- Update notification cache-busting for version checks.
