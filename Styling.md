# Styling

Styles can be applied in the following ways:

1.Inline

```
<Text style={{ fontSize:22, color: 'white' = }}>Hello World</Text>
```

2.With a StyleSheet

```
import React, {
  StyleSheet
} = from 'react-native';

let styles = StyleSheet.create({
    header: {
      color: 'white',
      fontSize:22
    }
})

<Text style={ styles.header }>Hello World</Text>
```

3.Multiple styles from a StyleSheet

```
let styles = StyleSheet.create({
    header: {
      color: 'white',
      fontSize:22
    },
    orange: {
      color: 'orange'
    }
})

<Text style={[ styles.header, styles.orange ]}>Hello World</Text>
```

4.Multiple styles, inline and from a StyleSheet:

```
<Text style={[ styles.header, { color: 'orange' } ]}>Hello World</Text>
```

5.Dynamically (1)

```
let styles = StyleSheet.create({
    shaded: {
      backgroundColor: 'ededed'
    }
})

let checkIndex = (i) => {
  if((i % 2) == 0) {
    return styles.shaded
  }
}

let people = [ { name: 'chris' }, { name: 'ashley' }, { name: 'justin' }, { name: 'amy' } ]

let content = people.map((p, i) => {
  return <View key={ i } style={ checkIndex(i) }><Text>{ p.name }</Text></View>
})

```

Dynamically (2)

```
let styles = StyleSheet.create({
    chosen: {
      backgroundColor: 'blue'
    }
})

let people = [ { name: 'chris', chosen: true }, { name: 'ashley', chosen: true }, { name: 'justin', chosen: false }, { name: 'amy', chosen: true } ]

let content = people.map((p, i) => {
  return <View key={ i } style={ p.chosen && styles.chosen }><Text>{ p.name }</Text></View>
})
```
