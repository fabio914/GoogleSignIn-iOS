# Google Sign-In for Carthage

This is a dynamic version of the [GoogleSignIn](https://developers.google.com/identity/sign-in/ios/sdk/) framework for iOS that is compatible with [Carthage](https://github.com/Carthage/Carthage).

# Installation

- Add this line to your `Cartfile`:
```
github "https://github.com/fabio914/GoogleSignIn-iOS" ~> 4.1
```
 - Update your dependencies:
```
$ carthage update GoogleSignIn-iOS --platform ios
```
 - Add `GoogleSignIn.framework` (at `Carthage/Build/iOS`) to your project.
 - Add `GoogleSignIn.framework/GoogleSignIn.bundle` to your Xcode project's **Copy Bundle Resources** build phase.
 - In the **Project > Target > Info > URL Types** panel, create a new item and paste your `REVERSED_CLIENT_ID` into the **URL Schemes** field. You can find your `REVERSED_CLIENT_ID` in the `GoogleService-Info.plist file`.
 - Follow these [instructions](https://developers.google.com/identity/sign-in/ios/sign-in?ver=swift) as if you *manually installed the SDK*.

# Version

 - XCode 8.3
 - iOS 9.3
