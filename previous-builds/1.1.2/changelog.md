# Changelog v1.1.2

## [1.1.2] - 2026-02-06

### Added
- **ID-Based Linking:** Introduced unique IDs (`settingId`) for machine records to ensure robust synchronization.
- **Image Sync:** Enabled downloading images directly from Google Drive.
- **Maintenance:** Added functionality to clear all local database data from the settings menu.

### Technical
- Updated GitHub release check logic to accurately detect new versions.
- Refactored `database.ts` to support UUID-based relationships.
