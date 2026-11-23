# Fruit Match Mania — GitHub Android Build

This build workflow wraps the existing `index.html` game with Capacitor and builds:
- Debug APK (installable for testing)
- Release AAB (unsigned; Play Store upload requires signing)

## Add these files to the root of your existing GitHub repository
- `package.json`
- `capacitor.config.json`
- `.github/workflows/android.yml`

Keep your existing `index.html` in the repository root.

## Run
Open the repository → Actions → Build Fruit Match Mania Android → Run workflow.
The workflow also runs automatically after pushes to `main`.

When the run finishes, open the successful run and download the
`Fruit-Match-Mania-Android` artifact.

IMPORTANT:
The APK is a debug build for testing. The AAB produced here is unsigned.
Before uploading to Google Play, create and securely configure an Android
release keystore and signing secrets in GitHub Actions. Never commit a keystore
or passwords to the repository.
