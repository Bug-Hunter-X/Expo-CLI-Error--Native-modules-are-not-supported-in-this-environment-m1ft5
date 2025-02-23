# Expo CLI Error: Native Modules Not Supported

This repository demonstrates a common error in Expo projects where using libraries with native modules results in the message: "Native modules are not supported in this environment".  The example shows how this issue arises and provides a solution.

## Problem

Attempting to use a library that relies on native code (iOS/Android) within an Expo managed workflow will result in this error because Expo's build process is designed to avoid direct native module integration.

## Solution

The solution generally involves:

1. **Replacing the library:** Finding an alternative library with pure JavaScript implementation.
2. **Using an Expo-compatible module:** If a suitable alternative doesn't exist, explore if an Expo-compatible module offers similar functionality.
3. **Ejecting from Expo (Advanced and generally not recommended):** This moves away from the managed workflow to allow complete native module integration, but it significantly increases the project's complexity and makes updates harder.

This example highlights using an alternative library as the simplest approach.