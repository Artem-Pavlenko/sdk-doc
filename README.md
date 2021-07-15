<div  align="center">
  <h1>Keyri SDK</h1>
</div>

## INSTALLATION

_Before using the Keyri SDK, you must install a number of dependencie._  
To install the stable version:

```js
npm install react-native-keyri-sdk @react-native-async-storage/async-storage react-native-camera react-native-device-info react-native-linear-gradient react-native-qrcode-scanner react-native-sensitive-info
```

or if you are using **_yarn_**

```js
yarn add react-native-keyri-sdk @react-native-async-storage/async-storage react-native-device-info react-native-camera react-native-linear-gradient react-native-qrcode-scanner react-native-sensitive-info
```

And put the line in your package.json file depending:

```js
"react-native-sodium": "https://github.com/glancemoney/react-native-sodium"`
```

**Your dependencies will look approximately (_package versions may differ from the example_):**

```js
        "dependencies": {
        ....
        "@react-native-async-storage/async-storage": "^1.15.5",
        "react": "17.0.1",
        "react-native": "0.64.1",
        "react-native-camera": "^3.44.3",
        "react-native-device-info": "^8.1.3",
        "react-native-keyri-sdk": "^0.0.4",
        "react-native-linear-gradient": "^2.5.6",
        "react-native-permissions": "^3.0.5",
        "react-native-qrcode-scanner": "^1.5.4",
        "react-native-sensitive-info": "^5.5.8",
        "react-native-sodium": "https://github.com/glancemoney/react-native-sodium"
        ....
        }
```

**_Please insert the following line in_** `android/app/build.gradle` **_inside_** `defaultConfig` **_block either:_**

```js
missingDimensionStrategy 'react-native-camera', 'general'
```

## USAGE

```js
import React from "react";
import { SafeAreaView, useColorScheme } from "react-native";
import { Colors } from "react-native/Libraries/NewAppScreen";
import Keyri from "react-native-keyri-sdk";

const App: React.FC = () => {
  const isDarkMode = useColorScheme() === "dark";

  const backgroundStyle = {
    backgroundColor: isDarkMode ? Colors.darker : Colors.lighter,
  };

  return (
    <SafeAreaView style={backgroundStyle}>
      <Keyri apiKey="your service api key" />
    </SafeAreaView>
  );
};
```

## START

**1. Start Metro**

```js
npm start
```

or if you are using **_yarn_**

```js
yarn start
```

**2. Start on device**

_in new terminal_

#### for start application on **android**

```js
npm run android
```

or if you are using **_yarn_**

```js
yarn android
```

#### for start apllication on **iOS**

```js
npm run ios
```

or

```js
yarn ios
```

> Happy hacking! :smiley:

## REQUIRED OPTIONS

| **option** | **type** | **description**                                                                                                                      |
| ---------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| _apiKey_   | string   | Api key of your service. Can be viewed on the Admin page for users who have registered or authenticated on [Keyri](https://keyri.co) |

<div  align="center">
  <a href="https://keyri.co" target="_blank">Keyri</a>
</div>
