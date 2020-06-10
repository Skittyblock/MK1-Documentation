---
layout: default
title: Wi-Fi
category: Actions
permalink: /actions/wifi
sublinks: ["wifi.isEnabled()", "wifi.setEnabled()", "wifi.networkName()", "wifi.signalRSSI()"]
---

# Wi-Fi
## wifi.isEnabled() ##
#### Syntax
```js
var enabled = wifi.enabled();
```

#### Return value
A `Boolean` representing the Wi-Fi enabled status


## wifi.setEnabled() ##
#### Syntax
```js
wifi.setEnabled(enabled);
```

#### Parameters
`enabled`: A `Boolean` to set Wi-Fi enabled status


## wifi.networkName() ##
#### Syntax
```js
var name = wifi.networkName();
```

#### Return value
A `String` representing the current Wi-Fi network's name


## wifi.signalRSSI() ##
#### Syntax
```js
var strength = wifi.signalRSSI();
```

#### Return value
A `Number` representing the current Wi-Fi network's RSSI signal strength
