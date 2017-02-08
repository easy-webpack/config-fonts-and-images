# @easy-webpack/config-fonts-and-images

[![Greenkeeper badge](https://badges.greenkeeper.io/easy-webpack/config-fonts-and-images.svg)](https://greenkeeper.io/)
Load in fonts and images into webpack bundle using [file-loader] and [url-loader].

Smaller files would be bundled as data URL while larger files will be emitted as a separate file.

The following file extensions are supported:
 - png
 - gif
 - jpg
 - eog
 - svg
 - woff
 - woff2
 - otf
 - ttf

# Installation
```
npm install --save-dev @easy-webpack/config-fonts-and-images
```
[easy-webpack](https://github.com/easy-webpack/core) is also required.

# Usage
```js
// webpack.config.js
const generateConfig = require('@easy-webpack/core').generateConfig;

const baseConfig = { ... }; // project-specific config like the entry file

module.exports = generateConfig(
  baseConfig,

  require('@easy-webpack/config-fonts-and-images')()
);

// This config will 
```

# Options
No options available

[file-loader]: https://github.com/webpack-contrib/file-loader
[url-loader]: https://github.com/webpack-contrib/url-loader