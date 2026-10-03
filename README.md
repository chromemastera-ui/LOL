# LOL (Android app)

App name: **LOL** · icon: the cat photo · inside: your Memory Lane app (`app/src/main/assets/www/index.html`).

## Option A: get the APK without installing anything (GitHub)
1. Make a free account at github.com, then create a new repository.
2. Upload everything from this folder to it. Use "Add file → Upload files" and drag in the contents, including the hidden `.github` folder.
3. Open the **Actions** tab. The "Build LOL APK" job starts by itself (about 3-5 minutes). If it doesn't, click it and press "Run workflow".
4. When it finishes, open the run and download **LOL-apk** from "Artifacts". Unzip it to get `app-debug.apk`.
5. Send the APK to your phone and open it. Allow "install unknown apps" when Android asks.

## Option B: Android Studio
1. Open this folder in Android Studio and let it sync (it downloads the Android SDK pieces it needs).
2. Menu: **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
3. The file is at `app/build/outputs/apk/debug/app-debug.apk`.

## Notes
- Accounts, posts, coins and photos are stored on the phone itself. Each phone has its own separate data.
- To change the app, edit `app/src/main/assets/www/index.html` and build again.
- To change the icon, replace the images in `app/src/main/res/mipmap-*`.
