[![Build Status](https://travis-ci.org/mapbox/strxml.svg)](https://travis-ci.org/mapbox/strxml)

# strxml-updated

This is merely a newly packaged version of strxml that can be `npm install`ed normally.

Create xml with strings and concatenation.

## install

    npm install --save strxml

## api

* `tag(el, [attributes], contents)`
* `tagClose(el, attributes)`
* `encode(str)`
* `attr(attributes)`

## example

```js

var tag = require('strxml').tag;

tag('Layer',
    tag('StyleName', 'style-' + i) +
    tag('Datasource', {
      name: 'layer-' + i,
      srs: WGS84
    }));
```
