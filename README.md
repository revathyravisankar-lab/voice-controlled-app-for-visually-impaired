# voice-controlled-app-for-visually-impaired

An Android app that provides voice-based assistance and feedback for visually impaired users. It uses Android Speech Recognition and TextToSpeech to accept voice commands and respond audibly.

## Features
- Simple voice command recognition (uses RecognizerIntent).
- Text-to-speech feedback using the device TTS engine.
- Runtime microphone permission handling.
- Accessible UI with a large listen button and content descriptions for TalkBack.

## Requirements
- Android Studio
- Android device or emulator with microphone and speech recognition support
- Min SDK: 21+ (adjust in your Gradle configuration as needed)

## Setup
1. Open the project in Android Studio (import the Gradle project).
2. Ensure your device/emulator has Google Play Services / speech recognition available.
3. Build and run on a physical device to test microphone input and TTS.

## Permissions
The app requires the following permissions (declared in AndroidManifest.xml):
- RECORD_AUDIO — required to capture voice input.
- INTERNET — used by some speech recognition providers (optional depending on device).

The app requests RECORD_AUDIO at runtime on Android 6.0+.

## Usage
- Tap the Listen button and speak a command when prompted.
- The app will speak back what it heard and respond to simple keywords ("hello", "help").

## Accessibility & UX notes
- Use short, clear TTS messages.
- Provide haptic or visual feedback when listening starts/stops for better awareness.

## Contributing
Contributions are welcome. Please open issues or pull requests with improvements, especially around accessibility and command handling.
