# [RNN](https://github.com/wix/react-native-navigation) with [Expo](https://github.com/expo/expo)

This is a minimalistic starter with [React Native Navigation](https://github.com/wix/react-native-navigation) (`v7.29.0`) and [Expo Modules](https://github.com/expo/expo) (`v46.0.10`) set up and running together without any issues.

[React Native](https://github.com/facebook/react-native) version is `0.70.0`.

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

### Rename

If you need to rename the app, do the following (based on [react-native-rename](https://github.com/junedomingo/react-native-rename)):

```bash
yarn rename "NewApp" -b com.yourcompany.newapp
yarn ios:pods
```

⚠️ Troubleshooting on Android. You can see that after running `rename` script, it doesn't change package name and imports for files under `newarchitecture` folder.

<details>
<summary>You will need do these steps manually</summary>

1. Open all `.java` files under `android/app/src/main/java/your/bundle/newarchitecture/` folder.

2. Open `MainApplication.java`.

3. Find all packages and imports which contain `io.batyr.rnnwithexpo` and change them to yours.

</details>

## What's inside

- [React Native Navigation](https://github.com/wix/react-native-navigation) - truly native navigation experience for iOS and Android.
- [Expo Modules](https://github.com/expo/expo) - libraries and modules from [Expo](https://expo.dev) ecosystem.
- [RNN Screens](https://github.com/kanzitelli/rnn-screens) - simplifed and predictable Navigation for React Native. Built on top of [React Native Navigation](https://github.com/wix/react-native-navigation).

#### Extra helpful libraries

- [Patch Package](https://github.com/ds300/patch-package) - useful for fixing node modules instantly.

## Known issues

- **[iOS]** _Hermes framework not found/loaded_. There are some cases when `hermes.framework` is not found/loaded in XCode with React Native 0.70. Check [this comment](https://github.com/facebook/react-native/issues/34601#issuecomment-1243232921) for potential solution.
- **[iOS]** _Large title is not shown on 2nd+ tab_. This [issue](https://github.com/software-mansion/react-native-screens/issues/649) exists. So you can find the patch file for fixing that in `patches/react-native+0.70.0.patch`.
- **[Android]** _Issue after renaming on Android_. This happens when you [rename](#rename) the app using `yarn rename` script. Check [Rename](#rename) section for possible solution.

## Other

- [kanzitelli/rnn-starter](https://github.com/kanzitelli/rnn-starter) - is a more advanced starter that is powered by cli-rn, React Native Navigation, Expo Modules, RNN Screens, RN UI lib, MMKV, Mobx, Reanimated 2, Dark Mode, Localization, Notifications, Permissions, and much more.

> Originally bootstrapped from [react-native-community/react-native-template-typescript](https://github.com/react-native-community/react-native-template-typescript).

## License

This project is [MIT licensed](/LICENSE.md)
