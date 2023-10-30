# _hyperstars
#### A star rating behavior in _hyperscript.

## Quick start
Several quick start options are available:

* [Download the latest release](https://github.com/adamjhf/hyperstars/archive/main.zip).
* Clone the repo: `git clone https://github.com/adamjhf/hyperstars.git`.

See [examples in action](http://adamjhf.github.io/hyperstars/).

## About
A customisable star rating behavior built in [hyperscript](https://hyperscript.org/), which is fast and touch-friendly, supporting any number of stars or any step size. Current version uses text only, with no images.

Triggers a `rated` event in the DOM, so can be used with HTMX, hyperscript or other client-side libraries for handling rating events.

## Example usage
Import `hyperstars.css` before loading hyperscript:
```
<link href="hyperstars.css" rel="stylesheet" type="text/css" />
<script src="hyperstars._hs" type="text/hyperscript"></script>
<script src="https://unpkg.com/hyperscript.org@0.9.12"></script>
```

For default 5-star rating, simply use by installing Hyperstars behavior on an span or div:
```
<span _="install Hyperstars()"></span>
```

Custom settings using a range input:
```
<span _="install Hyperstars(resettable: true)">
  <input type="range" min="0" max="10" step="0.5" value="5">
</span>
```

## Why Hyperstars
Hyperstars allows you to have a dynamic star rating component without JavaScript or importing libraries like jQuery. It is simple and fast, based on the same methodology as [rateit.js](https://github.com/gjunge/rateit.js).

## Credits
* Inspired by https://github.com/gjunge/rateit.js