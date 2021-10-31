---
title: EAS Build
sidebar_title: Introduction
---

**EAS Build** is a hosted service for building app binaries for your Expo and React Native projects.

It makes building your apps for distribution simple and easy to automate by providing defaults that work well for Expo and React Native projects out of the box, and by handling your app signing credentials for you (if you wish). It also makes sharing builds with your team easier than ever with [internal distribution](internal-distribution.md) (using ad hoc and/or enterprise "universal" provisioning), deeply integrates with EAS Submit for app store submissions, and has first-class support for the [`expo-updates`](updates.md) library to send updates. See the full pitch for EAS Build and other services on [expo.dev/eas](https://expo.dev/eas).

It's the next generation of the [`expo build:[ios/android]`](/distribution/building-standalone-apps.md) command &mdash; designed to work for any native project, whether or not you also use the managed workflow. It's the fastest way to get from `expo init` or `npx react-native init` to app stores. <!-- TODO: link to eas build / expo build comparison page -->

### Get started

- [Creating your first build](setup.md): it should only take a few minutes in total to get up and running for iOS and/or Android.
- [Learning about the limitations](/build-reference/limitations.md): EAS Build is a new and rapidly evolving service, so we recommend getting familiar with the current limitations.
