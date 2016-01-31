# Buttons

Buttons can be created with the following components:

[Text](https://facebook.github.io/react-native/docs/text.html#content)

[TouchableHighlight](https://facebook.github.io/react-native/docs/touchablehighlight.html#content)

[TouchableNativeFeedback](https://facebook.github.io/react-native/docs/touchablenativefeedback.html#content)

[TouchableOpacity](https://facebook.github.io/react-native/docs/touchableopacity.html#content)

[TouchableWithoutFeedback](https://facebook.github.io/react-native/docs/touchablewithoutfeedback.html#content)

### Examples

Here are a few examples of styling buttons:

```
<TouchableOpacity underlayColor="efefef" style={ styles.button }>
	 <Text style={ styles.buttonText }>Button Text</Text>
</TouchableOpacity>

button: {
	height: 80,
	marginLeft:40, 
	marginRight:40,
	backgroundColor: 'ededed', 
	justifyContent: 'center',
	alignItems: 'center'
}
buttonText: {
	fontSize:18
}
```

```
<TouchableHighlight underlayColor="efefef" style={ styles.button }>
	 <Text style={ styles.buttonText }>Button Text</Text>
</TouchableHighlight>

button: {
	height: 80,
	marginLeft:40, 
	marginRight:40,
	backgroundColor: 'ededed', 
	justifyContent: 'center',
	alignItems: 'center'
}
buttonText: {
	fontSize:18
}
```