# [`react-native-navigation`](https://github.com/wix/react-native-navigation) with [`expo-modules`](https://github.com/expo/expo)

### Usage

```bash
> git clone https://github.com/kanzitelli/rnn-with-expo.git App && cd App
> yarn && yarn ios:pods

> yarn ios
> yarn android
```

### Steps

```bash
> npx react-native init RNNWithExpo --template react-native-template-typescript
> yarn add react-native-navigation expo
> npx rnn-link
> # make changes from https://docs.expo.dev/bare/installing-expo-modules/#manual-installation
> npx pod-install
> npx react-native run android # or with Android Studio
> npx react-native run ios # or with XCode
```