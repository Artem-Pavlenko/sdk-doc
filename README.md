# Keyri SDK

## INSTALLATION

_Before using the Keyri SDK, you must install a number of dependencie._  
To install the stable version:

`npm install @react-native-async-storage/async-storage react-native-device-info react-native-linear-gradient react-native-qrcode-scanner react-native-sensitive-info`

> or if you are using yarn

`yarn add @react-native-async-storage/async-storage react-native-device-info react-native-linear-gradient react-native-qrcode-scanner react-native-sensitive-info`

And put the line in your package.json file depending:  
`"react-native-sodium": "https://github.com/glancemoney/react-native-sodium"`

**Your dependencies will look approximately (package versions may differ from the example):**

`"dependencies": {`  
`.....`  
` "@react-native-async-storage/async-storage": "^1.15.5",`  
` "react": "17.0.1",`  
` "react-native": "0.64.1",`  
` "react-native-camera": "^3.44.3",`  
` "react-native-device-info": "^8.1.3",`  
` "react-native-keyri-sdk": "0.0.1",`  
` "react-native-linear-gradient": "^2.5.6",`  
` "react-native-permissions": "^3.0.5",`  
` "react-native-qrcode-scanner": "^1.5.4",`  
` "react-native-sensitive-info": "^5.5.8",`  
` "react-native-sodium": "https://github.com/glancemoney/react-native-sodium"`  
`.....`  
`},`

##START##

`npm start`

> or if you are using yarn

`yarn start`

> and in new terminal:

`npm android`

> for start application on **android**;

`npm ios`

> for start apllication on **iOS**;

##REQUIRED OPTIONS##

| **option** | **type** | **description**                                                                                                                       |
| ---------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| apiKey     | string   | Api key of your service. Can be viewed on the Admin page for users who have registered or authenticated on [Keyri]((https://keyri.co) |

**[Keyri](https://keyri.co)**
