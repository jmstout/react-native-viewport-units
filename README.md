# react-native-viewport-units
Incredibly simple utility for (sort of) using viewport units with [React Native](https://github.com/facebook/react-native).

## Install
```sh
$ npm install react-native-viewport-units --save
```

## Usage
```javascript
var {vw, vh, vmin, vmax} = require('react-native-viewport-units');
```

Notice the required operator/syntax: __x * vw__
```javascript
<View style={{height:50*vh, width:50*vw}}/>
```

```javascript
var styles = StyleSheet.create({
  lookingGood: {
    width: 15*vmin,
    height: 10*vmax,
    padding: 2*vw,
    margin: 4*vh,
  }
});
```

## Roadmap
I would like to add support for orientation changes and reflowing components that use viewport units. I am, however, waiting until something official lands. Keeping a close eye on [418](https://github.com/facebook/react-native/pull/418).

## License
MIT © [Jeff Stout](http://jmstout.com)