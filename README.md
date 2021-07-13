# Keyri SDK

## INSTALLATION

_Before using the Keyri SDK, you must install a number of dependencie._  
To install the stable version:

`npm install react-native-keyri-sdk @react-native-async-storage/async-storage react-native-camera react-native-device-info react-native-linear-gradient react-native-qrcode-scanner react-native-sensitive-info`

or if you are using yarn

`yarn add react-native-keyri-sdk @react-native-async-storage/async-storage react-native-device-info react-native-camera react-native-linear-gradient react-native-qrcode-scanner react-native-sensitive-info`

And put the line in your package.json file depending:  
`"react-native-sodium": "https://github.com/glancemoney/react-native-sodium"`

**Your dependencies will look approximately (package versions may differ from the example):**

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

**Please insert the following line in android/app/build.gradle inside defaultConfig block either:**
`missingDimensionStrategy 'react-native-camera', 'general'`

## USAGE

        import React from 'react';
        import {SafeAreaView, useColorScheme} from 'react-native';
        import {Colors} from 'react-native/Libraries/NewAppScreen';
        import Keyri from 'react-native-keyri-sdk';

        const App: React.FC = () => {
        const isDarkMode = useColorScheme() === 'dark';

        const backgroundStyle = {
          backgroundColor: isDarkMode ? Colors.darker : Colors.lighter,
        };

        return (
          <SafeAreaView style={backgroundStyle}>
            <Keyri apiKey="your service api key" />
          </SafeAreaView>
        );
        };

## START

**1. Start Metro**

`npm start`

or if you are using yarn

`yarn start`

**2. Start on device**

_in new terminal:_

`npm android`/`yarn android` - for start application on **android**;

`npm ios`/`yarn ios` - for start apllication on **iOS**;

##REQUIRED OPTIONS##

| **option** | **type** | **description**                                                                                                                      |
| ---------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| apiKey     | string   | Api key of your service. Can be viewed on the Admin page for users who have registered or authenticated on [Keyri](https://keyri.co) |

<div  align="center" target="_blank">
  <a href="https://keyri.co" target="_blank">Keyri</a>
</div>
