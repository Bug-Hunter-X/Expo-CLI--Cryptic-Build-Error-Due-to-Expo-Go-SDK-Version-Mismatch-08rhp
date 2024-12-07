# Expo CLI: Cryptic Build Error Due to Expo Go/SDK Version Mismatch

This repository demonstrates a common but often difficult-to-diagnose bug in the Expo CLI. The issue stems from a version mismatch between the Expo Go app installed on your device and the SDK version specified in your project. This mismatch leads to vague error messages during the build or installation process.

## Reproducing the Bug

1.  Create a new Expo project with a specific SDK version:
   ```bash
expo init my-app --template blank
cd my-app
npm install
```
2.  (Manually create a version mismatch. This step will simulate the issue. In a real-world scenario, you might encounter this due to unexpected update conflicts.)
3.  Attempt to run the app on your device or emulator using the Expo Go app.
4.  Observe the cryptic error message.

## Solution

The key to resolving this is to ensure both your Expo Go app and your project's SDK version are compatible.  Update Expo Go to the latest version and/or update your project's SDK version accordingly.  If the problem persists, check to ensure your device's OS and Expo Go are up to date.