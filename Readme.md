# JsColor picker

JsColor is a web color picker component that aims to be super easy both for developers to install and for the end users to use.

See [JsColor site](http://jscolor.com)

## TypeScript

This version of JsColor picker has been rewritten in TypeScript.
The typescript files are compiled to the `dist` folder.

The original jscolor is available in javascript as `jscolor-picker.js` where the `jscolor` global is exported via `module.exports = jscolor` for use with NodeJS.

## Installation in two lines

```html
<script src="JsColor.js"></script>

Color: <input data-jscolor="" value="ab2567" />
```

## Node Usage (simulated browser environment)

```js
import JsColor from "jscolor-211";
const opts = {
  // ...
};
const pickerContainerElement = document.getElementById("#picker");
picker = new JSColor(pickerContainerElement, opts);
picker.show();
```

## Usage examples

Explore various examples of usage at [Examples](http://jscolor.com/examples/)

## Features

- **No framework needed:**
  jscolor is a completely self-sufficient JavaScript library consisting of only one JS file. It doesn't need any frameworks (jQuery, Dojo, MooTools etc.) but it can certainly coexist with them.

* **Cross-browser:**
  All modern browsers are supported, including:
  Edge, Firefox, Chrome, Safari, Opera, Internet Explorer 7 and above and others...

- **Highly customizable:**
  Whether you need to change the color picker's size/colors or attach a function to the onchange event, jscolor can be fine-tuned to perfectly suit your web project.

## Website

For more info on jscolor project, see [jscolor website](http://jscolor.com)

## Pull requests

Please do not submit any pull requests see [CONTRIBUTING](CONTRIBUTING.md)
Sorry for any inconvenience caused.

## Notes

The rewritten TypeScript library is still untested.

Some of the methods might still need to be reshaped to the form `xxxx = () => {}` in order that `this` is maintained correctly when used as a callback, such as an event handler. Most of the methods have been modified already, so give it a shot.
