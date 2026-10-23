# Mimi Reader — Android WebView template

This is a starter Android app that wraps a permitted website in a simple WebView interface.

## Build APK using GitHub Actions from a phone

1. Create a new repository on GitHub.
2. Upload the contents of this folder to the repository (not the ZIP file itself).
3. Open the repository's **Actions** tab.
4. Select **Build Android APK** and tap **Run workflow**, or push a commit to `main`.
5. Open the completed workflow run and download the `MimiReader-debug-apk` artifact.
6. Extract the artifact ZIP to get `app-debug.apk`, then install it on your Android phone.

## Configure the homepage

Edit `app/src/main/java/com/example/mimireader/MainActivity.java` and change:

`private static final String HOME_URL = "https://example.com";`

to a website you are permitted to access and display. Keep HTTPS enabled.

## Notes

- This is a generic starter template, not a finished store-ready release.
- Some websites block embedded WebViews or require browser features that WebView does not support.
- A debug APK is suitable for testing; publishing requires a properly signed release build.
