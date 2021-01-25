## react-native-ls-drawer-layout [![styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

A platform-agnostic drawer layout. It uses a pure JavaScript implementation on every platform to ensure consistency. We try to keep it up to date with the implementation of [DrawerLayoutAndroid](https://facebook.github.io/react-native/docs/drawerlayoutandroid.html#content) and add features we consider necessary as well.

## Add it to your project

1. Run `npm install react-native-ls-drawer-layout --save`
2. Import the component by using one of these:
  - `var DrawerLayout = require('react-native-ls-drawer-layout').default;`
  - `import DrawerLayout from 'react-native-ls-drawer-layout';`
3. Follow the [DrawerLayoutAndroid](https://facebook.github.io/react-native/docs/drawerlayoutandroid.html#content) docs -- the API is the same. Everything that differs is explained below

## API
This includes the differences between our implementation and the official one [DrawerLayoutAndroid](https://facebook.github.io/react-native/docs/drawerlayoutandroid.html#content). Every breaking change is (hopefully) hidden behind a feature flag, so that this implementation may also be used as polyfill.

## Demo

![](https://raw.githubusercontent.com/leandrosimoes/react-native-drawer-layout/master/example.gif)

## Examples

- [Normal usage](https://github.com/DanielMSchmidt/DrawerLayoutExample)
- [Heavy Load](https://github.com/DanielMSchmidt/DrawerLayoutHeavyLoadExample)

To run the demo, please run `npm install` in the `DrawerLayoutExample/` directory and start the demo up from there like any other React Native application.

## Support

| React Native Version      | react-native-ls-drawer-layout Version |
|---------------------------|---------------------------------------|
| >= 11 & < 23              | NO SUPPORT                            |
| >= 23                     | NO SUPPORT                            |
| >= 35                     | >= 2.0.1                              |

If you experience any further restrictions with other versions, please let us know.

## Restrictions

- Currently, there is no support for setting the status bar color in iOS. If you know any workaround, we would be glad to see an idea or a PR.
- The overlay to close the drawer has a `zIndex` of 1000 so setting a higher `zIndex` somewhere else may lead to inconsistencies.