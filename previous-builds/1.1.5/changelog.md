# Changelog v1.1.5

## [1.1.5] - 2026-02-19

### Fixed
- Reverted broken `redirectUri` change that caused `Error 400: invalid_request` on both iOS and Android.
- Restored iOS Google Auth to working state.

### Notes
- Android auth still had redirect issue (browser didn't return to app). Fixed in v1.1.6.
