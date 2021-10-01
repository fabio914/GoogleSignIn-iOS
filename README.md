# Google Sign-In for Carthage / XCFramework

[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)

This is a dynamic version of the [Google Sign-In](https://developers.google.com/identity/sign-in/ios/sdk/) framework for iOS that is compatible with [Carthage](https://github.com/Carthage/Carthage). It's a simple framework that includes the original [GoogleSignIn-iOS](https://github.com/google/GoogleSignIn-iOS) Swift Package dependency.

## Installation

- Add this line to your `Cartfile`:
```
github "https://github.com/fabio914/GoogleSignIn-iOS" == 6.0.2
```
 - Update your dependencies:
```
$ carthage update GoogleSignIn-iOS --use-xcframeworks
```
 - Add `GoogleSignIn.xcframework` (at `Carthage/Build/`) to your project.
 
 - Add `GoogleSignIn_GoogleSignIn.bundle` to your Xcode project's **Copy Bundle Resources** build phase. Alerts and `GIDSignInButton` won't work without it.
 
 - In the **Project > Target > Info > URL Types** panel, create a new item and paste your `REVERSED_CLIENT_ID` into the **URL Schemes** field. You can find your `REVERSED_CLIENT_ID` in the `GoogleService-Info.plist` file. More [details](https://developers.google.com/identity/sign-in/ios/start-integrating#add_a_url_scheme_for_google_sign-in_to_your_project).
 
 - Follow these [instructions](https://developers.google.com/identity/sign-in/ios/sign-in?ver=swift).
 
 ## Building XCFramework with Carthage
 
 ```
 carthage build --use-xcframeworks --no-skip-current
```

## Version

 - XCode 12.4
 - iOS 9.0
