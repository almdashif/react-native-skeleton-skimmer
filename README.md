#### React Native Skeleton Skimmer <img src="src/Images/tsLogo.png" alt="TS" width="26" />

A Simple  Skeleton Loader with Skimmer effect in React Native  :fire: :rocket: :star2:

![npm](https://img.shields.io/npm/v/react-native-skeleton-skimmer) ![LICENSE MIT](https://img.shields.io/badge/license-MIT-brightgreen.svg)   [![NPM](https://static.npmjs.com/b0f1a8318363185cc2ea6a40ac23eeb2.png)](https://www.npmjs.com/package/react-native-skeleton-skimmer/)



![Loading Animation](src/Images/skimmer.gif)


### Installation
```js
npm i react-native-skeleton-skimmer --save
cd ios && pod install
cd android && ./gradlew clean
```
or
```js
yarn add react-native-skeleton-skimmer
cd ios && pod install
cd android && ./gradlew clean
```
### Usage
```js
import React from 'react';
import { View, Text, StyleSheet } from 'react-native';
import SkeletonSkimmer, { EanimationType } from 'react-native-skeleton-skimmer';

const App = () => {
  return (
    <View style={styles.container}>
      <Text style={styles.title}>Loading...</Text>
      {/* Basic usage of SkeletonSkimmer */}
      <SkeletonSkimmer />

      {/* Custom usage with different props */}
      <SkeletonSkimmer
        width={250}
        height={40}
        color="#D3D3D3"
        highlightColor="#A9A9A9"
        duration={3000}
        animationType={EanimationType.bounce}
        style={styles.customStyle}
        animationStyle={styles.customAnimationStyle}
      />
    </View>
  );
};

const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#fff',
  },
  title: {
    fontSize: 24,
    marginBottom: 20,
  },
  customStyle: {
    marginTop: 20,
    borderRadius: 5,
  },
  customAnimationStyle: {
    opacity: 0.5,
  },
});

export default App;

 

```


### Properties
|Prop	|Type	|Description	|Required	|Default|
| ----------------------- | --- | ------- | --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|width	| number|	Width of the loader container	|No	|300|
|height|	number|	Height of the loader container	|No	|30|
|color	|string	|Background color of the loader container|	No	|'#E0E0E0'|
|highlightColor|	string|	Color of the animated highlight effect	|No|	'#F7F7F7'|
|style	|object|	Additional styles for the container|	No|	{}|
|animationStyle	|object	|Additional styles for the animated highlight element|	No	|{}|
|duration	|number|	Duration of the animation in milliseconds	|No|	2000|
|animationType	|`EanimationType` (enum)|	Type of animation for the effect (linear, bounce, etc.)|	No	|`EanimationType.linear` |
---

### `EanimationType` Enum Values

The `EanimationType` enum defines the type of animation effect applied to the `SkeletonSkimmer`. Below are the available animation types:

- **`linear`**: A smooth, continuous animation with a constant speed. (Default)
- **`bounce`**: A bouncing animation that adds a playful effect.
- **`circle`**: A circular animation, creating a rotating effect.
- **`ease`**: A smooth easing animation that accelerates and decelerates in a natural motion (ease-in-out).

### Contributing

Contributions are always welcome! If you’d like to contribute, feel free to fork the repository and submit a pull request with your improvements.

For bug reports, feature requests, or any issues, please open an issue on the GitHub repository or contact me directly at ashifalmohammed@gmail.com.

Thank you for your interest in contributing!



## Author
[almdashif](https://github.com/almdashif)

## License
[MIT Licensed](https://github.com/almdashif/react-native-skeleton-skimmer/blob/main/LICENSE) SkeletonSkimmer is under BSD license. © Mohammed Ashif  2024 - present






















