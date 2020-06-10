---
layout: default
title: Device
category: Actions
permalink: /actions/device
sublinks: ["device.name()", "device.systemName()", "device.systemVersion()", "device.model()", "device.identifierForVendor()", "device.orientation()", "device.isPortrait()", "device.isLandscape()", "device.isLocked()", "device.isScreenOn()", "device.batteryLevel()", "device.batteryState()", "device.shutdown()", "device.reboot()", "device.respring()", "device.safemode()", "device.lock()"]
---

# Device
## device.name() ##
#### Syntax
```js
var name = device.name();
```

#### Return value
A `String` containing the device's name


## device.systemName() ##
#### Syntax
```js
var systemName = device.systemName();
```

#### Return value
A `String` containing the device's system name (e.g. iOS)


## device.systemVersion() ##
#### Syntax
```js
var version = device.systemVersion();
```

#### Return value
A `Number` representing the device's system version (e.g. 13.5)


## device.model() ##
#### Syntax
```js
var model = device.model();
```

#### Return value
A `String` containing the device's model (e.g. iPhone)


## device.identifierForVendor() ##
#### Syntax
```js
var id = device.identifierForVendor();
```

#### Return value
A `String` containing the device's vendor identifier


## device.orientation() ##
#### Syntax
```js
var orientation = device.orientation();
```

#### Return value
A `Number` representing the device's orientation (1 is portrait, [etc.](https://developer.apple.com/documentation/uikit/uideviceorientation))


## device.isPortrait() ##
#### Syntax
```js
var portrait = device.isPortrait();
```

#### Return value
A `Boolean` representing whether the device is in portrait orientation or not


## device.isLandscape() ##
#### Syntax
```js
var landscape = device.isLandscape();
```

#### Return value
A `Boolean` representing whether the device is in landscape orientation or not


## device.isLocked() ##
#### Syntax
```js
var locked = device.isLocked();
```

#### Return value
A `Boolean` representing whether the device is locked or not


## device.isScreenOn() ##
#### Syntax
```js
var screenOn = device.isScreenOn();
```

#### Return value
A `Boolean` representing whether the device's screen is on or not


## device.batteryLevel() ##
#### Syntax
```js
var batteryLevel = device.batteryLevel();
```

#### Return value
A `Number` between 0 and 100 representing the device's battery level


## device.batteryState() ##
#### Syntax
```js
var batteryState = device.batteryState();
```

#### Return value
A `Number` representing the device's battery charging state (1 is unplugged, [etc.](https://developer.apple.com/documentation/uikit/uidevicebatterystate))


## device.shutdown() ##
#### Syntax
```js
device.shutdown();
```

## device.reboot() ##
#### Syntax
```js
device.reboot();
```

## device.respring() ##
#### Syntax
```js
device.respring();
```

## device.safemode() ##
#### Syntax
```js
device.safemode();
```

## device.lock() ##
#### Syntax
```js
device.lock();
```
