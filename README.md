# mouseenter

mouseenter event emulation

## mouseenter(element, fn)

```js
var mouseenter = require('mouseenter');
var div = document.querySelector(...);

mouseenter(div, function(ev) {
    console.log('the mouse is here');
});
```

## unbind

`mouseenter` returns a function you can use to no longer react to mouseenter events. Call this function and the previously bound event will be unbound.

```js
var unbind = mouseenter(div, function(ev) {
    console.log('the mouse is here');
});

// will listen for mouseenter events

// call `unbind` to stop listening
unbind();
```

## testing

```
$ npm run test-local
```

Then open the url it gives you in a local browser.

## Licence

MIT
