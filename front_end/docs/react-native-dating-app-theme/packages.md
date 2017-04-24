# Packages Used

_package.json_

<pre class="line-numbers"><code class="language-json">
{
  "name": "StrapDatingApp",
  "version": "7.0.0",
  "private": true,
  "devDependencies": {
    "react-native-scripts": "0.0.26",
    "jest-expo": "^0.3.0",
    "react-test-renderer": "~15.4.1",
     "babel-jest": "17.0.0",
    "babel-preset-react-native": "1.9.0",
    "chai": "^3.5.0",
    "jest": "17.0.0",
    "jest-react-native": "17.0.0",
    "mocha": "^2.5.3",
    "remote-redux-devtools": "^0.3.3",
    "remote-redux-devtools-on-debugger": "^0.4.6"
  },
  "main": "./node_modules/react-native-scripts/build/bin/crna-entry.js",
  "scripts": {
    "postinstall": "remotedev-debugger",
    "start": "react-native-scripts start",
    "eject": "react-native-scripts eject",
    "android": "react-native-scripts android",
    "ios": "react-native-scripts ios",
    "test": "node node_modules/jest/bin/jest.js --watch"
  },
  "jest": {
    "preset": "jest-expo"
  },
  "dependencies": {
    "expo": "^15.1.0",
    "react": "~15.4.0",
    "react-native": "0.42.3",
    "lodash": "^4.13.1",
    "moment": "^2.13.0",
    "native-base": "2.1.0-rc.2",
    "react-native-camera-roll-picker": "^1.1.9",
    "react-native-gifted-chat": "0.1.3",
    "react-native-modalbox": "^1.3.7",
    "react-native-multi-slider": "^0.3.5",
    "react-native-router-flux": "^3.38.0",
    "react-native-scrollable-tab-view": "^0.7.2",
    "react-native-swiper": "^1.5.4",
    "react-redux": "^4.4.5",
    "redux": "^3.5.2",
    "redux-persist": "^3.2.2",
    "redux-thunk": "^2.1.0",
    "@expo/vector-icons": "~4.0.0"
  }
}</code></pre>
