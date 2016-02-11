# Flexbox

React Native uses Flexbox to control layout. Here, I will try to go over scenarios you may run into, with solutions for those scenarios.

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
