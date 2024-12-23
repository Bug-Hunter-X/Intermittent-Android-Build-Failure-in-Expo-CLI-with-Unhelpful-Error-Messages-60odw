# Expo CLI Intermittent Android Build Failure

This repository demonstrates an uncommon bug encountered while building Android APKs using Expo CLI. The build process fails intermittently with vague error messages, making debugging extremely challenging.  The project may build successfully on iOS without issue, and the errors appear to be random. 

## Bug Reproduction

1. Clone this repository.
2. Run `expo prebuild`.
3. Run `expo build:android`.  Observe that the build may succeed on some attempts and fail on others with cryptic error messages.

## Potential Causes

* **Native Module Conflicts:** Conflicting versions of native modules or dependencies.
* **Gradle Issues:** Problems with the Android Gradle build system.
* **Expo CLI Bugs:** Rare, intermittent bugs within the Expo CLI itself.

## Solution

The provided `bugSolution.js` file contains potential solutions, including checking Android build tools versions, cleaning the project cache and investigating for native dependency conflicts. 