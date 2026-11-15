# eFootDream Squad: APK project

Your index.html is already in `www/`. Pick ONE route:

## A) Android Studio (local)
Requires Node 18+, JDK 17, Android Studio.
    npm install
    npm run setup
    npm run apk
APK: android/app/build/outputs/apk/debug/app-debug.apk
(Or `npx cap open android` and use Build > Build APK(s).)

## B) No local setup: GitHub Actions
Push this folder to a new GitHub repo, open Actions > "Build APK" > Run workflow,
then download the `efootdream-debug-apk` artifact.

## Notes
- Debug APK installs directly. For Google Play, create a signed release build (AAB) in Android Studio.
- The app loads supabase-js (jsDelivr) and Google Fonts online, so it needs internet.
- After editing www/index.html, run `npm run sync` and rebuild.
