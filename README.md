# [RNN](https://github.com/wix/react-native-navigation) with [Expo](https://github.com/expo/expo)

This is a minimalistic starter with [React Native Navigation](https://github.com/wix/react-native-navigation) and [Expo Modules](https://github.com/expo/expo) set up and running together without any issues.

[React Native](https://github.com/facebook/react-native) version is `0.69.5`. [Expo](https://github.com/expo/expo) version is `46.0.9`.

## Quickstart

1. Clone the repo

```bash
npx degit starters-dev/rnn-with-expo app
```

2. Install packages and pods

```bash
cd app && yarn && yarn ios:pods
```

3. Run it

Open XCode or Android Studio to run the project (recommended) or do

```bash
yarn ios
yarn android
```

---

If you need to rename the app, do the following (based on [react-native-rename](https://github.com/junedomingo/react-native-rename)):

```bash
yarn rename "NewApp" -b com.yourcompany.newapp
yarn ios:pods
```

> Troubleshooting on Android. You can see that after running `rename` script, it doesn't change package name and imports for files under `newarchitecture` folder. You will need do that manually.

## What's inside

- [React Native Navigation](https://github.com/wix/react-native-navigation) - truly native navigation experience for iOS and Android.
- [Expo Modules](https://github.com/expo/expo) - libraries and modules from [Expo](https://expo.dev) ecosystem.
- [RNN Screens](https://github.com/kanzitelli/rnn-screens) - simplifed and predictable Navigation for React Native. Built on top of [React Native Navigation](https://github.com/wix/react-native-navigation).

## Other

- [kanzitelli/rnn-starter](https://github.com/kanzitelli/rnn-starter) - is a more advanced starter that is powered by cli-rn, React Native Navigation, Expo Modules, RNN Screens, RN UI lib, MMKV, Mobx, Reanimated 2, Dark Mode, Localization, Notifications, Permissions, and much more.

> Originally bootstrapped from [react-native-community/react-native-template-typescript](https://github.com/react-native-community/react-native-template-typescript).

## License

This project is [MIT licensed](/LICENSE.md)
