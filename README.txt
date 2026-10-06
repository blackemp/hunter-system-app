HUNTER SYSTEM - build the Android APK (no Android Studio needed)

1. Create a free account at github.com and make a NEW repository (private is fine).
2. Upload everything in this folder to it (Add file > Upload files).
   IMPORTANT: the hidden folder .github/workflows/build.yml must end up in the repo.
   If it is missing after upload, use Add file > Create new file, type the name
   .github/workflows/build.yml and paste the contents of build.yml from this download.
3. Open the repo's Actions tab. Pick "Build Android APK", then Run workflow.
   (It also runs automatically on upload.) It takes about 5 to 8 minutes.
4. When it shows a green tick, open the run and download "hunter-system-apk" from Artifacts.
   Unzip it to get app-debug.apk.
5. Copy the APK to your phone, tap it, and allow "Install unknown apps" for your
   file manager or browser when Android asks.

To change the app later, edit www/index.html in the repo and the APK rebuilds.
The app works fully offline. Data is stored on the phone; uninstalling erases it.
