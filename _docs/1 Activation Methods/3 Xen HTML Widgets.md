---
layout: default
title: Xen HTML Widgets
category: Activation Methods
permalink: /activation-methods/xen-widgets
---

# Xen HTML Widgets
There is an MK1 addon package that implements a system for communicating between Xen HTML widgets and MK1. To use the below methods in your widget, make sure to add `Depends: xyz.skitty.mk1xen` to your control file when packaging it.

## URL Schemes
Scripts can be run and triggers can be activated through the same url scheme the MK1 application implements, except the application won't be opened. 
```html
<a href="mk1://runScript/Example/">Run Example Script</a>
```

## mk1Message()
MK1 also exposes the `mk1Message()` JavaScript function to your widget. To use, simply call it with the message action and body. To run the example script: `mk1Message("runScript", "Example");`.

### mk1Callback()
MK1 also supports scripts that return an expression, however it's limited. First of all, scripts will automatically return whatever the last evaluated expression was. For example:
```js
if (!lpm.getEnabled()) {
  lpm.setEnabled(true);
  true;
} else {
  lpm.setEnabled(false);
  false;
}
```

That script will return whether or not low power mode is activated after toggling it. To get this value after calling your script, you'll need to implement the `mk1Callback()` function, with an example being:
```js
function mk1Callback(data) {
  alert(JSON.stringify(data));
}
```

If you call the above script while low power mode is off, the callback function will return with the data
```json
{
  "message": {
    "action": "runScript",
    "body": "Example"
  },
  "return": true
}
```
