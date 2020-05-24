# react-native-img-placeholder [![npm version](https://badge.fury.io/js/react-native-img-placeholder.svg)](https://badge.fury.io/js/react-native-img-placeholder)

[![NPM](https://nodei.co/npm/react-native-img-placeholder.png?downloads=true)](https://nodei.co/npm/react-native-img-placeholder/)

- Support Android and iOS.
- The image component that supports shows placeholderSource when load image network.
- Show placeholderSource if the main source can't be loaded or error.
- Support custom ActivityIndicator loading.

## Require

React-native >= 0.46.x

## What's new

Fixed render inside <ImagePlaceholder /> component

## Installation

```bash
npm i --save react-native-img-placeholder
```

Please file an issue if you have any trouble!

## Usage

```jsx
import ImagePlaceholder from 'react-native-img-placeholder';

....

<ImagePlaceholder
    style={{ width: 320, height: 250 }}
    loadingStyle={{ size: 'large', color: 'blue' }}
    source={{ uri: 'https://via.placeholder.com/300/09f/fff.png' }}
/>
```

## Options

Supports all [Image](https://facebook.github.io/react-native/docs/images.html) properties.

| Option                             | Default                             | Info                                                               |
| ---------------------------------- | ----------------------------------- | ------------------------------------------------------------------ |
| placeholderSource                  | require('./Images/empty-image.png') | Show `placeholderSource` if the `source` can't be loaded or error. |
| loadingStyle                       | size: 'small'; color: 'gray'        | Style ActivityIndicator                                            |
| isShowActivity                     | true                                | Show ActivityIndicator loading                                     |
| placeholderStyle                   |                                     | Style placeholder image                                            |
| customImagePlaceholderDefaultStyle |                                     | Custom style image placeholder default                             |
| borderRadius                       |                                     | Border radius                                                      |

## License

ISC
