# RNAndroidDemo

A React Native Android demo app with CI/CD via GitHub Actions.

## Build

```bash
npm install
cd android && ./gradlew assembleDebug
```

The debug APK will be at `android/app/build/outputs/apk/debug/app-debug.apk`.

## CI/CD

The GitHub Actions workflow builds the debug APK and uploads it to AutoDevice on every push to `main`.

### Required Secrets

- `AUTODEVICE_API_KEY` — API key for AutoDevice
