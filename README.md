# Ambient OS — Android Foldable Launcher (Early Build)

Native Kotlin + Jetpack Compose Android HOME launcher with responsive cover/unfolded UI, low-key midnight theme, bottom command bar, app drawer, notification stream, Focus and System pages.

## Build in GitHub
1. Create an empty GitHub repository.
2. Upload the **contents** of this folder to the repository root, including `.github/workflows/build-apk.yml`.
3. Open **Actions → Build Ambient OS APK → Run workflow**.
4. When successful, open the run → **Artifacts** → `AmbientOS-debug-apk`.
5. Download, unzip, install `app-debug.apk` on your phone. Enable installation from the chosen source when Android asks.
6. Open Ambient OS → System → Set as default launcher. Enable notification access separately to show notifications.

## Current limitations
- This is an early MVP, **not** a finished replica of the concept image.
- Notification stream is read-only and only includes data provided by Android's notification APIs.
- No Instagram/Messenger inline replies, SMS/MMS role, email sync, media gallery, or animations yet.
- Command bar supports page commands and installed app name matching.
- No APK was built in the authoring environment; GitHub Actions must verify compilation.
- Android's QUERY_ALL_PACKAGES permission is broad; restrict package visibility before Play Store distribution.
