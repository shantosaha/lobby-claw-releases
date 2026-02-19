# Changelog v1.1.4

## [1.1.4] - 2026-02-19

### Fixed
- **Android Google Auth:** Resolved the "Something went wrong" error (stuck at `auth.expo.io`) by implementing a native redirect scheme (`lobbyclawapp://`).
- Bypassed the Expo Auth Proxy for more reliable native authentication.

### Technical
- Updated `googleSyncService.ts` to use `expo-linking` for explicit `redirectUri` generation.
- Incremented `versionCode` for Android release.
