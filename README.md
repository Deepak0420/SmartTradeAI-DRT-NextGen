# SmartTradeAI DRT NextGen

Android-first trading analysis app scaffold.

## Current milestone
- Kotlin + Jetpack Compose Android app
- Transparent educational DRT-style range calculation
- Manual close-price input for testing
- GitHub Actions workflow to build a debug APK and run unit tests

## Important
This is **not** Binomo's proprietary DRT implementation. The current engine is an explicitly documented educational approximation using a rolling mean and population standard deviation. It does not connect to a broker, place trades, or guarantee predictions.

## Build
Open this project in Android Studio (recent version with Android SDK 35), allow Gradle sync, then run the `app` configuration.

The GitHub Actions workflow builds `app-debug.apk` and uploads it as an artifact on pushes and pull requests to `main`.

## Next milestones
1. Validate the Android build.
2. Add chart rendering and selectable candle intervals.
3. Add a reliable market-data provider (with API key handling).
4. Add a floating assistant and configurable alerts.
5. Consider a Chrome extension and cross-device sync.

Do not add broker credentials or API secrets to source control.
