# Lyric Weaver Mobile

Lyric Weaver Mobile is a Flutter mobile app version of the Lyric Weaver multilingual lyric generator.

It packages a lyric generator into a mobile app using Flutter and WebView, designed for Android and iOS builds.

## Features

- Multilingual lyric generation
  - Traditional Chinese
  - English
  - Japanese
  - Taiwanese Hokkien
- Offline bundled HTML lyric generator
- Flutter mobile app shell
- WebView display
- Copy lyrics
- Download lyrics as TXT
- Share lyrics where supported
- Android APK / AAB build support
- iOS project structure included

## Project Structure

```text
Lyric-Weaver-Mobile/
├── assets/
│   ├── web/
│   │   └── index.html
│   └── icons/
├── lib/
│   └── main.dart
├── android/
├── ios/
├── docs/
│   ├── BUILD_NOTES.md
│   ├── PRIVACY_POLICY.md
│   └── TERMS_OF_SERVICE.md
├── store/
│   ├── google_play/
│   └── apple_app_store/
├── pubspec.yaml
├── README.md
├── CHANGELOG.md
├── LICENSE
└── .gitignore
```

## Requirements

- Flutter SDK
- Android Studio
- Android SDK
- Windows / macOS / Linux for Android builds
- macOS + Xcode for iOS builds

Check your environment:

```bash
flutter doctor
```

## Run the App

```bash
flutter pub get
flutter run
```

## Build Android APK

```bash
flutter build apk --release
```

Output:

```text
build/app/outputs/flutter-apk/app-release.apk
```

## Build Android AAB for Google Play

```bash
flutter build appbundle --release
```

Output:

```text
build/app/outputs/bundle/release/app-release.aab
```

## Build iOS

```bash
flutter build ios --release
open ios/Runner.xcworkspace
```

Archive the app in Xcode and upload it through App Store Connect.

## GitHub Upload Notes

Upload the project source files, but do not upload generated build folders.

Do not upload:

```text
build/
.dart_tool/
.gradle/
android/.gradle/
```

APK and AAB files are better stored in GitHub Releases instead of the source repository.

## Privacy

The default app runs locally and does not collect personal data. If analytics, ads, cloud sync, or AI API integration are added later, update the privacy policy.

## License

MIT License
