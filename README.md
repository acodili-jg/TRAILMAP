![USTP Trailmap Icon](assets/image/icon.png)

# USTP Trailmap

A map of the University of Science and Technology of Southern Philippines in Cagayan de Oro city.

Promotional Video on Facebook: https://fb.watch/p3b_fgwO6L/

## Building

### 1. With Expo Account

This will run the app and is usable through Expo Go.

Writer Note: I recommend using Expo Go on a real phone as I can't get it to work on an emulator.

```
# Check the scripts section in package.json
yarn start

# Equivalent alternative
npx expo start
```

<sub>See: https://docs.expo.dev/get-started/start-developing/#start-a-development-server
</sub>

### 2. Without Expo Account

This will build and install the app.

Note: depending on the environment, build times might take a very long time, especially for realease builds.

```
# Generates the Android and IOS files
npx expo prebuild

# Remember to connect your device or run your Emulator for testing
npx react-native run-android --mode="release"

# Signs the APK and publishes it to Google Play Store.
npx react-native build-android --mode=release
```

Remember to follow up the [React Native Documentation](https://reactnative.dev/docs/signed-apk-android) to sign the APK and publish to Google Play Store.

<sub>See: https://github.com/expo/eas-cli/issues/1606#issuecomment-1681583138</sub>

### Other Resources

* Expo Sign-up. https://expo.dev/signup
* Android Studio Emulator. https://docs.expo.dev/workflow/android-studio-emulator/
