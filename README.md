# WhatBrowser.js
Detect current browser name and version with javascript. No dependency needed.

## How to use:
* Include the `what-browser-min.js` to your html: `<script src="../dist/what-browser-min.js"></script>`
* calling `WhatBrowser()` function will expose callback which return an object containing `name` and `version` of the browser. Use that information for whatever you want.

## Example

Basic use:
```javascript
whatBrowser(function(browser){
  var name = browser.name;
  var version = browser.version;

  // Do what you want with that information here
});
``

Check if browser is Internet Explorer 9 or below and add class to body with jQuery:
```javascript
jQuery(function() {
  whatBrowser(function(browser){
    if (browser.name === "Explorer" && browser.version >= 9) {
      // Add class to the body
      jQuery("body").addClass("oldies")
    }
  });
});
```
