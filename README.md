monic-loader
============

Using [Monic](https://github.com/MonicBuilder/Monic) with [WebPack](http://webpack.github.io).

[![NPM version](http://img.shields.io/npm/v/monic-loader.svg?style=flat)](http://badge.fury.io/js/monic-loader)
[![NPM dependencies](http://img.shields.io/david/MonicBuilder/monic-loader.svg?style=flat)](https://david-dm.org/MonicBuilder/monic-loader)
[![Build Status](http://img.shields.io/travis/MonicBuilder/monic-loader.svg?style=flat&branch=master)](https://travis-ci.org/MonicBuilder/monic-loader)

## Install

```bash
npm install monic-loader --save-dev
```

## Usage

**webpack.config.json**

```js
var webpack = require('webpack');

webpack({
  entry: {
      readme: './readme.md'
  },

  output: {
      filename: '[name].bundle.js'
  },

  module: {
    loaders: [
      {
        test: /\.md$/,
        exclude: /node_modules/,
        loader: 'monic-loader'
      }
    ]
  }
}), function (err, stats) {
    // ...
});
```

## [Options](https://github.com/MonicBuilder/Monic#using-in-nodejs)
## [License](https://github.com/MonicBuilder/gulp-monic/blob/master/LICENSE)

The MIT License.
