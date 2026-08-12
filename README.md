# DELCO Attendance Android App

Android wrapper for the production DELCO Timekeeper app at https://delco-timekeeper.lovable.app/.

The live Lovable/TanStack Start server functions and Supabase backend remain hosted and unchanged. The Android app provides a native WebView shell with foreground GPS permission handling for attendance/geofence use.

## Automatic APK build

This repository includes `.github/workflows/build-apk.yml`. Every push to `main` builds an installable debug APK and uploads it as the `DELCO-Attendance-APK` GitHub Actions artifact.

## App identity

- App name: DELCO Attendance
- Package: `com.delco.attendance`
- Version: `1.0.0`
- minSdk: 23
- targetSdk / compileSdk: 36

The debug APK is intended for testing/direct installation. Play Store publishing later requires a signed release AAB and private signing key.
