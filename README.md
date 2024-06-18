[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
<h1 align="center">
  <img width="32" alt="icon" src="https://github.com/Ernest2026/expo-gl-image-filters/docusaurus/website/static/img/favicon_32.ico">
  @ernesto_tech/expo-gl-image-filters
</h1>

<p align="center">
  <a href="https://github.com/Ernest2026/expo-gl-image-filters/blob/master/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="react-native-gl-image-filters is released under the MIT license." />
  </a>
  <a href="https://www.npmjs.org/package/react-native-gl-image-filters">
    <img src="https://img.shields.io/npm/v/react-native-gl-image-filters" alt="Current npm package version." />
  </a>
  <a href="https://www.npmjs.com/package/react-native-gl-image-filters">
    <img src="https://img.shields.io/npm/dm/react-native-gl-image-filters.svg" alt="Current npm package downloads." />
  </a>
  <a href="https://snack.expo.io/@gregoryrn/expo-gregorynative-react-native-gl-image-filters">
    <img src="https://badgen.net/badge/expo/snack/blue?icon=https://symbols.getvecta.com/stencil_79/82_expo-icon.11a3983570.svg" alt="Expo snack." />
  </a>
  <a href="https://stackblitz.com/edit/react-native-gl-image-filters-web-example">
    <img src="https://badgen.net/badge/web/blitz/purple?icon=bitcoin-lightning" alt="Stackblitz project." />
  </a>
</p>

[](https://badgen.net/badge/expo/snack/blue?icon=https://symbols.getvecta.com/stencil_79/82_expo-icon.11a3983570.svg)
OpenGL bindings for React Native to implement complex effects over images and components, in the descriptive VDOM paradigm. You can use predefined filters:
  - blur
  - contrast
  - saturation
  - brightness
  - hue
  - negative
  - sepia
  - sharpen
  - temperature
  - exposure. 

![](https://github.com/Ernest2026/expo-gl-image-filters/blob/master/cat-gl-filters.gif)

**`gl-react-native` is an implementation of `gl-react` for `react-native`. Please [read the main gl-react README](https://github.com/gre/gl-react) and [gl-react-native README](https://github.com/gre/gl-react/tree/master/packages/gl-react-native) for more information.**

Table of Contents
=================
<!--ts-->
  * [API](#api)
     * [Props](#props)
     * [Constants](#constants)
        * [DefaultValues](#defaultvalues)
           * [Usage example](#usage-example)
        * [DefaultPresets](#defaultpresets)
           * [Usage example](#usage-example-1)
     * [Presets](#presets)
     * [Utils](#utils)
        * [createPreset](#createpreset)
  * [Recommended Min and Max range for each filter](#recommended-min-and-max-range-for-each-filter)
  * [Installation](#installation)
     * [Installation for React Native](#installation-for-react-native)
        * [Configure your React Native Application](#configure-your-react-native-application)
     * [Installation on Expo](#installation-on-expo)
     * [Installation on React Web](#installation-on-react-web)
  * [Usage](#usage)
     * [Usage with React Native](#usage-with-react-native)
     * [Usage with Expo](#usage-with-expo)
     * [Usage with React web](#usage-with-react-web)
<!--te-->

## API
- [`Props`](#props)
- [`Constants`](#constants)
- [`Presets`](#presets)
- [`Utils`](#utils)

### `Props`
Props for ImageFilters Component

| Name | Description | Type | Required | Default Value |
| :--- | :----- | :--- | :---: | :---: |
| children | Inner component or url for image | Any | + |  |
| width | Width of component | Number | + |  |
| height | Height of component | Number | + |  |
| hue | Hue filter | Number |   | 0 |
| blur | Blur filter | Number |   | 0 |
| sepia | Sepia filter | Number |   | 0 |
| sharpen | Sharpen filter | Number |   | 0 |
| negative | Negative filter | Number |   | 0 |
| contrast | Contrast filter | Number |   | 1 |
| saturation | Saturation filter | Number |   | 1 |
| brightness | Brightness filter | Number |   | 1 |
| temperature | Temperature filter | Number |   | 6500 |
| exposure | Exposure filter | Number |   | 0 |
| 🆕 colorOverlay | Color Overlay with the length of 4 (RGBA format). Values must be a real value between 0 and 255. | Array |   | [0.0, 0.0, 0.0, 0.0] |

### `Constants`
- [`DefaultValues`](#defaultvalues)
- [`DefaultPresets`](#defaultpresets)

#### `DefaultValues`
Can be used to set filter to default one manually. 

