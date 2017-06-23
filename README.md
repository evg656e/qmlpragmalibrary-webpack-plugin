# QmlPragmaLibrary Webpack Plugin

Adds a `.pragma library` declaration the beginning of a file as mentioned in [Defining JavaScript Resources In QML](http://doc.qt.io/qt-5/qtqml-javascript-resources.html#shared-javascript-resources-libraries).

## Install

With npm:
```
npm install qmlpragmalibrary-webpack-plugin --save-dev
```

## Usage

```javascript
const QmlPragmaLibraryWebpackPlugin = require('qmlpragmalibrary-webpack-plugin');

module.exports = {
  entry: 'factorial.js',
  output: {
    path: path.resolve(__dirname, 'assets'),
    filename: 'factorial.qml.js'
  },
  plugins: [
    new QmlPragmaLibraryWebpackPlugin()
  ]
};
```
