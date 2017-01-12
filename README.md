# [Cordova Backlight](https://github.com/mebibou/cordova-plugin-backlight) [![Release](https://img.shields.io/npm/v/cordova-plugin-backlight.svg?style=flat)](https://github.com/mebibou/cordova-plugin-backlight/releases)

This plugin provides interface to turn on or off the backlight of the screen on your device. This is not like brightness, as this will completely turn off the backlight, showing nothing but a black screen.

Note: this plugin only works for Android for now, help wanted for iOs implementation.

## Setup

Add the plugin using cordova cli:
```bash
cordova plugin add cordova-plugin-backlight
```

## Javascript Interface

```javascript
// turn on backlight
window.cordova.plugins.Backlight.on(function onSuccess() {
  // backlight is on
}, function onError(error) {
  console.error(error);
});

// turn off backlight
window.cordova.plugins.Backlight.off(function onSuccess() {
  // backlight is off
}, function onError(error) {
  console.error(error);
});
```
