# Changelog v1.1.6

## [1.1.6] - 2026-02-19

### Fixed
- **Android Google Auth redirect:** Added `com.frankenstein.lobbyclawapp` scheme to AndroidManifest intent filter.
- The `expo-auth-session` Google provider generates native redirect URIs using `Application.applicationId` (e.g., `com.frankenstein.lobbyclawapp:/oauthredirect`), but the manifest only had the custom `lobbyclawapp://` scheme registered. Chrome couldn't redirect back to the app because the OS didn't recognize the `com.frankenstein.lobbyclawapp://` scheme.

### Technical
- Added `<data android:scheme="com.frankenstein.lobbyclawapp"/>` to the `MainActivity` intent filter in `AndroidManifest.xml`.
- This allows Android to intercept the Google OAuth redirect and return the user to the app.
