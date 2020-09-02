<div align="center">

<h1>React Native Swipeable Panel Modified Version</h1>

**swipeable-panel** is a swipeable, easy to use bottom panel for your React Native projects. You can extend panel by swiping up, make it small or close by swiping down with pan gestures. Feel free to redesign inside of the panel.

<h4>React Native Swipeable Panel ( Original Version )</h4>
(https://www.npmjs.com/package/rn-swipeable-panel)

</div>

<br/>

<div align="center" style="margin-bottom:1em">
    <img src="https://user-images.githubusercontent.com/19428358/82732219-913fb680-9d14-11ea-8128-55b20b0f7d1c.gif" width="auto" height="600"/>
</div>

<br/>

## ⚙️ Installation

```
Clone Code
```

```
Put on your project as folder
```
```
import { SwipeablePanel } from '../Modal/Panel';
```

✅ It is done!

<!-- ## Usage -->

## 🚀 How to use

```javascript
import React from 'react';
import { StyleSheet, Text, View } from 'react-native';

import { SwipeablePanel } from '../Modal/Panel';

export default App = () => {
  const [panelProps, setPanelProps] = useState({
    fullWidth: true,
    openLarge: true,
    showCloseButton: true,
    onClose: () => closePanel(),
    onPressCloseButton: () => closePanel(),
    // ...or any prop you want
  });
  const [isPanelActive, setIsPanelActive] = useState(false);

  const openPanel = () => {
    setIsPanelActive(true);
  };

  const closePanel = () => {
    setIsPanelActive(false);
  };

  return (
    <View style={styles.container}>
      <Text style={styles.welcome}>Welcome to React Native!</Text>
      <Text style={styles.instructions}>To get started, edit App.js</Text>
      <SwipeablePanel {...panelProps} isActive={isPanelActive}>
        <PanelContent /> {/* Your Content Here */}
      </SwipeablePanel>
    </View>
  );
};
```

## ☝️ Options

<br/>

| Properties              | Type       | Description                                              | Default |
| ----------------------- | ---------- | -------------------------------------------------------- | ------- |
| **isActive**            | `bool`     | Show/Hide the panel                                      | `false` |
| **onClose**             | `Function` | Fired when the panel is closed                           |         |
| **showCloseButton**     | `bool`     | Set true if you want to show close button                |         |
| **fullWidth**           | `bool`     | Set true if you want to make full with panel             | `false` |
| **openLarge**           | `bool`     | Set true if you want to open panel large by default      | `false` |
| **onlyLarge**           | `bool`     | Set true if you want to let panel open just large mode   | `false` |
| **onlySmall**           | `bool`     | Set true if you want to let panel open just small mode   | `false` |
| **noBackgroundOpacity** | `bool`     | Set true if you want to disable black background opacity | `false` |
| **style**               | `Object`   | Use this prop to override panel style                    | `{}`    |
| **closeRootStyle**      | `Object`   | Use this prop to override close button background style  | `{}`    |
| **closeIconStyle**      | `Object`   | Use this prop to override close button icon style        | `{}`    |
| **barStyle**            | `Object`   | Use this prop to override bar style                      | `{}`    |
| **closeOnTouchOutside** | `bool`     | Set true if you want to close panel by touching outside  | `false` |
| **allowTouchOutside**   | `bool`     | Set true if you want to make toucable outside of panel   | `false` |
| **noBar**               | `bool`     | Set true if you want to remove gray bar                  | `false` |



#### 👏 Contributing
@enesozturk
