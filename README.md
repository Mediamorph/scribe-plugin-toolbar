# scribe-plugin-toolbar [![Build Status](https://travis-ci.org/guardian/scribe-plugin-toolbar.svg?branch=master)](https://travis-ci.org/guardian/scribe-plugin-toolbar)

A toolbar of buttons and shortcuts for Scribe

**This is a fork that intends to solve just specific issues of integrating with MM:**

* Added deamdify to be able to use in commonJS build without global transformation that breaks other libraries.

## Installation
```
bower install scribe-plugin-toolbar
```

Alternatively, you can [access the distribution files through GitHub releases](https://github.com/guardian/scribe-plugin-toolbar/releases).

## Usage Example

scribe-plugin-toolbar is an AMD module:

``` js
require(['scribe', 'scribe-plugin-toolbar'], function (Scribe, scribePluginToolbar) {
  var scribeElement = document.querySelector('.scribe');
  // Create an instance of Scribe
  var scribe = new Scribe(scribeElement);

  var toolbarElement = document.querySelector('.toolbar');
  scribe.use(scribePluginToolbar(toolbarElement));
});
```

For more documentation see the [project wiki](https://github.com/guardian/scribe-plugin-toolbar/wiki)

## Options

Set the `shared` key to true to enable the shared toolbar functionality.

## Development

After cloning the repo:

* `npm install`
* `bower install`
* `npm run test`

If the tests run green then you are good to start developing
