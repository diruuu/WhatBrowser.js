# WhatBrowser.js
Detect current browser name and version with javascript. No dependency needed.

## How to use:
* Include the `what-browser-min.js` to your html: `<script src="../dist/what-browser-min.js"></script>`
* calling `WhatBrowser()` function will expose callback which return an object containing `name` and `version`. Use that information for whatever you want.

## Example
```javascript
whatBrowser(function(browser){
  var name = browser.name;
  var version = browser.version;

  // Do what you want with that information here
});
``
