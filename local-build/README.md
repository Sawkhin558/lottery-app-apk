# Local APK Build Instructions

## Method 1: Android Studio (Easiest)
1. Install Android Studio
2. Open this folder in Android Studio
3. Click Build → Build APK
4. APK will be in `app/build/outputs/apk/debug/`

## Method 2: Command Line
```bash
# Make sure you have Android SDK installed
./gradlew assembleDebug
```

## Method 3: Online Builder
Use services like:
- WebViewGold
- GoNative
- Website 2 APK Builder

## Project Structure
- `app/src/main/assets/index.html` - Your lottery app
- `app/src/main/java/com/lottery/app/MainActivity.java` - WebView activity
- `app/src/main/AndroidManifest.xml` - Permissions and config

## Permissions Included
- INTERNET
- READ_EXTERNAL_STORAGE  
- WRITE_EXTERNAL_STORAGE