## react-native-show-more-button

### Installation

```
npm install react-native-show-more-button --save
```

```javascript
import ShowMore from 'react-native-show-more-button';
```

![Example](https://raw.githubusercontent.com/AmyrAhmady/react-native-show-more-button/master/example.gif)


## Props

```
height -> height of component when it's closed. Default value is 250.
showMoreText -> Show More button text. Default string is "Show More".
showLessText -> Show Less button text. Default string is "Show Less".
buttonColor -> color of show more/less text. Default value is "#AAAAFF".
```

### Usage (without props)

```javascript
// import component
import ShowMore from 'react-native-show-more-button';


//usage:
<ShowMore>

</ShowMore>
```

## Usage (with props)
```javascript
// import component
import ShowMore from 'react-native-show-more-button';

//usage:
<ShowMore height={400} buttonColor={"#FF0000"} showMoreText="Open" showLessText="Close">

</ShowMore>
```

## Example Code

```javascript
import React from 'react';
import { Image, Text, View, ScrollView } from 'react-native';
import ShowMore from 'react-native-show-more-button';

export default class App extends React.Component {
  constructor(props) {
    super(props);
  }

  render() {
    return (

      <View>
        <ScrollView>
          <ShowMore>
            <View style={{ justifyContent: 'center', alignItems: 'center' }}>

              <Image source={require('./1.png')} />

              <Text>wowowowowowowowowowwowo</Text>
              <Text>What a LOGO!</Text>
              <Text>This is just a test script</Text>
              <Text>for Show More react-native module</Text>
              <Text>Dope, right?</Text>

              <Image source={require('./2.jpg')} />

              <Text>This is a logo with number 6 in it</Text>
              <Text>We are going to see if this package works well!</Text>
              <Text>------------------------------------</Text>
              <Text>Well, looks like it works, right?</Text>
              <Text>Easy to use!</Text>
              <Text>react-native-show-more-button</Text>

              <Image source={require('./2.jpg')} />

              <Text>Okay.</Text>

            </View>
          </ShowMore>
        </ScrollView>
      </View>
    );
  }
}
```