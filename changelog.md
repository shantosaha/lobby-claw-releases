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
