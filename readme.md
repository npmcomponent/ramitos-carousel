*This repository is a mirror of the [component](http://component.io) module [ramitos/carousel](http://github.com/ramitos/carousel). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/ramitos-carousel`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# carousel

image carousel [demo](http://ramitos.github.com/carousel)

## installation

for [component](https://github.com/component/component):

    $ component install ramitos/carousel

## usage

```js
var carousel = require('carousel');
var cats = carousel(document.getElementById('carousel-container'));

setInterval(function () {
  var height = Math.floor(Math.random() * 500) + 100;
  var width = Math.floor(Math.random() * 500) + 100;
  var url = "http://placekitten.com/g/" + width + "/" + height;
  carousel.add(url);
}, 1000)
```

## api

#### void add(url: string)

add an image url to the carousel

#### number image()

retrieve the selected image position

#### void disable()

disable all carousel controls

#### void enable()

enable all carousel controls

## license

MIT