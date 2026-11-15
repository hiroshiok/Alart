# Alart — Android Alarm App

Alart is an Android alarm application built with Kotlin, Jetpack Compose and Material 3. The complete source project is provided in [Alart-source.tar.gz](Alart-source.tar.gz).

## Download the APK

Every push to `main` starts the **Build Android APK** workflow. To download the installable debug APK:

1. Open the repository's **Actions** tab.
2. Select the latest successful **Build Android APK** run.
3. In **Artifacts**, download **Alart-debug-apk**.
4. Extract the downloaded artifact ZIP; it contains `Alart-debug.apk`.

You can also start a build manually from **Actions → Build Android APK → Run workflow**.

## Build pipeline

GitHub Actions installs JDK 17, Android SDK 36 and Gradle 8.13, extracts the source project, runs unit tests, builds `assembleDebug`, verifies the APK exists, and uploads it as a 30-day artifact. A second artifact named `Alart-source-code` contains the full project source. The APK is a debug-signed installable build, not a Play Store release.

## Local development

Extract `Alart-source.tar.gz` and open the `Alart` folder in Android Studio. The project uses Android Gradle Plugin 8.11.1, Kotlin 2.2.20 and Gradle 8.13.
