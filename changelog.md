# Changelog v1.1.5

## [1.1.5] - 2026-02-19

### Fixed
- **Reverted broken Auth redirect:** Removed the custom `redirectUri` (`lobbyclawapp:///`) that caused `Error 400: invalid_request` on both iOS and Android.
- **Restored iOS Google Auth:** iOS login flow is working again (same behavior as v1.1.3).

### Technical
- The `expo-auth-session/providers/google` library handles native redirects automatically:
  - iOS: Uses the reversed `iosClientId` as the redirect scheme.
  - Android: Uses the package signature (SHA-1) with the `androidClientId`.
- Added detailed comments explaining why a custom `redirectUri` must NOT be set.

### Notes
- The original Android auth issue (stuck at `auth.expo.io`) is still present and will be investigated separately. The root cause is likely a missing or incorrect SHA-1 fingerprint for the Android Client ID in the Google Cloud Console.
