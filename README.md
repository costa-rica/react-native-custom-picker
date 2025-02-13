# React Native Custom Picker

A customizable picker for React Native that adapts to both iOS and Android. This picker will fit in small spaces that need to be efficient with the space around it.

## Features

- iOS: Uses `@react-native-picker/picker`
  - this dependecy will automatically install once this package is installed.
- Android: Uses `ScrollView` for a native-like experience
- Customizable width, font size, background color

## Demos

### iOS

![Demo iOS](docs/demoiOS_small.gif)

### Android

![Demo Android](docs/demoAndroid_small.gif)

## Installation

1. clone this repo to your machine: `git clone https://github.com/costa-rica/react-native-custom-picker.git`

2. in your project folder:
   `yarn add file:/path/to/react-native-custom-picker`
   or
   `npm install /path/to/react-native-custom-picker`

## Usage

```js
import CustomPicker from "react-native-custom-picker";
import { useRef, useEffect } from "react";
const [selectedItem, setSelectedItem] = useState("Apple");

<CustomPicker
  arrayElements={["Apple", "Banana", "Orange"]}
  selectedElement={selectedItem}
  setSelectedElement={setSelectedItem}
  itemHeight={40}
  width={120}
  fontSize={16}
/>;
```
