# Changelog v1.5.0

## [1.5.0] - 2026-02-19

### Changes
### Added

# Changelog v1.4.0

## [1.4.0] - 2026-02-19

### Added
- **Smart History Browsing**: Increased history pagination to 50 records and added quick-select date range chips (7D, 30D).
- **Animated Loading**: Added new animated skeleton screens to provide better visual feedback while loading history data.
- **Image Preview**: Tapped images in history now open in a full-screen preview.

### Fixed
- **Drive Image Integration**: resolved issues where Google Drive sharing links would not always render correctly in the history tab.
- **Inventory Consistency**: Fixed a bug where machine quantity displays could show stale data instead of live stock levels.
- **Refined Alerts**: Improved the "Machine Attention" logic to reduce noise by requiring a minimum number of plays before flagging low payout.
- **Service Report Reliability**: Added better error handling and empty-state feedback when starting new service reports.

# Changelog v1.3.0

## [1.3.0] - 2026-02-19

### Changes
### Added
- **Smart Session Management:** Enhanced Google login to automatically refresh your session, reducing the need to sign in repeatedly.
- **Connection Status:** Added a visual status indicator in Settings to show your current connection health.
- **Inventory Audit:** Inventory updates now track and log exact quantity changes (previous vs. new) for better history tracking.
- **Image Organization:** Photos are now automatically sorted into specific folders (Inventory, Machine Photos, Reports) in Google Drive.

### Fixed
- **Data Validation:** Added checks to prevent accidental entry of invalid inventory quantities.
- **Sync Reliability:** Improved image synchronization to ensure files are routed to their correct destinations.

# Changelog v1.2.0

## [1.2.0] - 2026-02-19

### Changes
- Maintenance and stability improvements

# Changelog v1.1.9

## [1.1.9] - 2026-02-19

### Changes
- update

# Changelog v1.1.8

## [1.1.8] - 2026-02-19

### Fixed
- **Google Drive Sync:** Fixed image upload collision issues by ensuring unique filenames for new captures.
- **Data Import:** Fixed bug where machine images were not being updated during fetch from Drive.
- **Drive Image Formulas:** Improved detection of `=IMAGE()` formulas in spreadsheets for better cross-device sync.
- **Sync Reliability:** Added protection for historical records during full sync on new devices.

# Changelog v1.1.7

## [1.1.7] - 2026-02-19

### Added
- **Manual Update Check:** Added a "Check for Updates" button in the Settings page under App Info.

### Fixed
- **Update Notifications:** Improved the update checking logic by adding a cache-busting timestamp to the version check URL.
- **Testing:** Temporarily enabled update notifications for development builds to allow verification during testing.
