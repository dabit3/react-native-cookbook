# Routing

There are two out of the box ways to implement routing in React Native:

1. [Navigator](https://facebook.github.io/react-native/docs/navigator.html)
2. [NavigatorIOS](https://facebook.github.io/react-native/docs/navigatorios.html)

### Implementations

1. Navigator

`initialRoute` - This route is loaded when the Navigator is loaded.
`renderScene` - This is the function that the navigator uses to render the scene for a given route.
`React.createElement` - Allows you to manually create a React element. To add properties to an element, we pass a properties object as the second argument and you can also optionally pass children to the third argument.

import {
  Navigator,
  Component
} from 'react-native'

class Navigation extends Component {
  render() {
    return (
      <Navigator
       initialRoute={{ name: 'Main', component: Main, index: 0 }}
       renderScene={ (route, navigator) => {
         return React.createElement(route.component, { ...this.props, ...route.passProps, navigator, route } );
      }} />
    )
  }
}

this.props.navigator.push({
  component: NextComponent,
  passProps: {
    myVar: 'some variable'
  }
})
