# Changelog v1.3.0

## [1.3.0] - 2026-02-19

### Changes
- **Auth Expiry & Auto-Refresh:**
  - Added token expiry tracking and optional refresh token storage in SecureStore.
  - Implemented auto-refresh logic in `getToken()` for tokens expiring < 5 mins.
  - Added visual Auth Status indicator in Settings (valid/expired/refreshing).
  - Backend now handles Google OAuth refresh tokens properly.

- **Inventory DB Update Pipeline:**
  - Enhanced `updateInventoryItem` and `incrementInventoryQuantity` to log **before/after quantities** for full audit trails.
  - Added input validation for quantity updates (prevents NaN, warns on negative).
  - Confirmed atomic transactions for all inventory modifications.

- **Image Management & Drive Folders:**
  - Implemented structured Google Drive folders:
    - `Inventory/`
    - `Machine_Photos/`
    - `Service_Reports/`
    - `Meter_Readings/`
  - Added `generateImageFilename` for metadata-based naming (`type_machineId_timestamp.jpg`).
  - Updated sync logic to route images to correct subfolders based on context.
  - Added `Image Folder` column to inventory sync data for better tracking.

- **Planning:**
  - Completed Phase 2: Foundation.
  - Updated project state to Phase 3.

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
