# oauth

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Firebase Setup

To integrate Firebase into your Flutter app, follow these steps:

1. Create a Firebase project:
   - Go to the [Firebase Console](https://console.firebase.google.com/)
   - Click on "Add project" and follow the setup wizard

2. Generate SHA-1 certificate fingerprint:
   - For debug mode: Run 
`keytool -list -v -keystore ~/.android/debug.keystore -alias androiddebugkey -storepass android -keypass android` in your terminal
   - For release mode: Use your app signing key

3. Add the SHA-1 to your Firebase project:
   - In the Firebase Console, go to Project settings > Your apps > Android app
   - Click "Add fingerprint" and enter the SHA-1

4. Download the configuration file:
   - In the Firebase Console, go to Project settings > Your apps > Android app
   - Click "Download google-services.json"
   - Place the file in your project's `android/app/` directory

5. Configure your app:
   - Follow the instructions in the Firebase Console to add the necessary dependencies and plugins to your `build.gradle` files

Remember to update your app's Firebase configuration if you make any changes to your app's package name or signing certificate.
