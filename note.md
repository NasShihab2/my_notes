1️⃣ Create a new React Native project
# Navigate to your projects folder
cd D:\ReactProject

# Create a new project (latest recommended CLI)
npx @react-native-community/cli init Project1
# or if older version
npx react-native init Project1

2️⃣ Install dependencies
# Safe area context
npm install react-native-safe-area-context
# or
yarn add react-native-safe-area-context

# Optional: template screen
npm install @react-native/new-app-screen
# or
yarn add @react-native/new-app-screen

3️⃣ Open project in VS Code
code Project1

4️⃣ Start Metro Bundler (JS server)
# Always run this in your project root
npx react-native start

5️⃣ Run app on Android device/emulator
# With device connected
npx react-native run-android


If using a physical device wirelessly, set Dev Settings → Debug server host → PC_IP:8081

6️⃣ Run app on iOS (Mac only)
npx react-native run-ios

7️⃣ Build APK / Release
cd android

# Debug APK (with JS bundled)
gradlew assembleDebug

# Release APK (production)
gradlew assembleRelease


APK path: android\app\build\outputs\apk\release\app-release.apk

8️⃣ Useful device / debugging commands
# List connected Android devices
adb devices

# Stop Metro server
Ctrl + C

# Restart app manually
npx react-native run-android

9️⃣ Hot Reload / Fast Refresh

Shake device or press Ctrl + M on emulator → enable Fast Refresh

Save JS/TS files in VS Code → updates live on device without rebuilding

10️⃣ Setting Android SDK for React Native

In android/local.properties:

sdk.dir=C:\\Users\\Admin\\AppData\\Local\\Android\\Sdk


Optional system-wide:

ANDROID_HOME = C:\Users\Admin\AppData\Local\Android\Sdk
Add to PATH: %ANDROID_HOME%\platform-tools
