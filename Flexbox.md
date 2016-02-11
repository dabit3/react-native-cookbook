# Flexbox

React Native uses Flexbox to control layout. Here, I will try to go over scenarios you may run into, with solutions for those scenarios.

All of the Flexbox properties of React Native can be found [here](https://facebook.github.io/react-native/docs/flexbox.html#content)

1.Align items center vertically

```
import {
  StyleSheet
} from 'react-native'

<View style={ styles.container }>
  <Text>This text will be centered vertically</Text>
</View>

var styles = StyleSheet.create({
    container: {
      justifyContent: 'center',
    }
})
```

2.Align items top

```
import {
  StyleSheet
} from 'react-native'

<View style={ styles.container }>
  <Text>This text will be centered vertically</Text>
</View>

var styles = StyleSheet.create({
    container: {
      justifyContent: 'flex-start',
    }
})
```

3.Align items bottom

```
import {
  StyleSheet
} from 'react-native'

<View style={ styles.container }>
  <Text>This text will be centered vertically</Text>
</View>

var styles = StyleSheet.create({
    container: {
      justifyContent: 'flex-end',
    }
})
```

4.space-between

`space-between` basically places all items equally along the main axis. Any leftover space that the flex items don't take up is equally distributed between the items.

```
import {
  StyleSheet
} from 'react-native'

<View style={ styles.container }>
  <Text>This text will be centered vertically</Text>
  <Text>This text will be centered vertically</Text>
  <Text>This text will be centered vertically</Text>
</View>

var styles = StyleSheet.create({
    container: {
      justifyContent: 'space-between',
      height:100,
      backgroundColor: 'ededed'
    }
})
```
