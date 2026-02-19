# Changelog v2.0.5

## [2.0.5] - 2026-02-20

### Added
- **Unified Form Timeline**: Service Reports are now merged into the main Form Responses sheet in Google Drive and Excel, providing a single source of truth for all machine interventions.
- **Machine Group Sync**: Full two-way synchronization for Machine Groups, including location and machine assignments.
- **Activity Log Excel Export**: Dedicated "Activity Log" tab added to Excel exports.
- **Improved Service History**: Service Reports now support full two-way updates and archiving across all devices.

### Technical Specs
- **Database Schema v2.0.5**: Added archival tracking and modification metadata for more robust data merging.
- **Sync Reliability**: Multi-device collision handling for Service Reports using unique identifiers.

## [2.0.2] - 2026-02-20

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


