---
layout: default
title: Bluetooth
category: Actions
permalink: /actions/bluetooth
sublinks: ["bluetooth.isEnabled()", "bluetooth.setEnabled()", "bluetooth.connectedDevices()", "bluetooth.pairedDevices()", "bluetoothDevice.name()", "bluetoothDevice.address()", "bluetoothDevice.paired()", "bluetoothDevice.unpair()"]
---

# Bluetooth
## bluetooth.isEnabled() ##
#### Syntax
```js
var enabled = bluetooth.isEnabled();
```

#### Return value
A `Boolean` with the enabled status of bluetooth

## bluetooth.setEnabled() ##
#### Syntax
```js
bluetooth.setEnabled(enabled);
```

#### Parameters
`enabled`: A `Boolean` to set bluetooth enabled status


## bluetooth.connectedDevices() ##
#### Syntax
```js
var devices = bluetooth.connectedDevices();
```

#### Return value
A `Array` filled with bluetooth device id  `String`s


## bluetooth.pairedDevices() ##
#### Syntax
```js
var devices = bluetooth.pairedDevices();
```

#### Return value
A `Array` filled with bluetooth device id  `String`s


# Bluetooth Device
## bluetoothDevice.name() ##
#### Syntax
```js
var name = bluetoothDevice.name(id);
```

#### Parameters
`id`: A `String` representing a bluetooth device id

#### Return value
A `String` with the name of the bluetooth device


## bluetoothDevice.address() ##
#### Syntax
```js
var address = bluetoothDevice.address(id);
```

#### Parameters
`id`: A `String` representing a bluetooth device id

#### Return value
A `String` representing the device address


## bluetoothDevice.paired() ##
#### Syntax
```js
var paired = bluetoothDevice.paired(id);
```

#### Parameters
`id`: A `String` representing a bluetooth device id

#### Return value
A `Boolean` representing whether the device is paired or not


## bluetoothDevice.unpair() ##
#### Syntax
```js
bluetoothDevice.unpair(id);
```

#### Parameters
`id`: A `String` representing a bluetooth device id
