# Changelog v1.1.4

## [1.1.4] - 2026-02-19

### Fixed
- Attempted Android Google Auth fix using native redirect scheme.

### Known Issue
- This version introduced a regression: `redirect_uri=lobbyclawapp:///` caused `Error 400: invalid_request` on both iOS and Android.
- **Do not use this version.** Replaced by v1.1.5.
