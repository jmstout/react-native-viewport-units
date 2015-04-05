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

## License
MIT © [Jeff Stout](http://jmstout.com)