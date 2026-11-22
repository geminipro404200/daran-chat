# Դարան (Daran) — Android Application

Complete Android Studio (Kotlin) project for the **Դարան** educational management platform (`am.daran.edu`).

## Included Features
- **Custom Launcher Icons**: Your uploaded «Դարան» logo pre-generated in all 5 Android densities (`mdpi` through `xxxhdpi`, square + round).
- **Full Embedded Daran Platform**: Chief Operator, School Operator, Teacher (with AI topic generator isolated from grades & daily attendance), Student portal, school-to-chief messaging, strict multi-school isolation, and Username + SHA-256 login.
- **Android Security Hardening**:
  - `FLAG_SECURE` enabled (blocks screenshots and screen recording).
  - `usesCleartextTraffic="false"` and `allowBackup="false"`.
  - Served locally over secure `WebViewAssetLoader` HTTPS origin with persistent `localStorage`.
- **Optional Central Server Mode**: Set `REMOTE_SERVER_URL` in `MainActivity.kt` to your hosted HTTPS URL (from `daran-server.zip`) to sync all Android devices and computers to one shared database.

## How to Build the APK
1. Unzip `daran-android.zip` and open the folder in **Android Studio** (Ladybug or newer).
2. Wait for Gradle Sync to finish.
3. Click **Build → Build Bundle(s) / APK(s) → Build APK(s)** to generate `app-debug.apk` (or **Generate Signed App Bundle / APK** for Google Play release).
