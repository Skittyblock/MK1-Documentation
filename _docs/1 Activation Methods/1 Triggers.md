---
layout: default
title: Triggers
category: Activation Methods
permalink: /activation-methods/triggers
---

# Triggers
## What are triggers?
Triggers are the main activation method of MK1. They're events that can activate an MK1 script when they occur.

## Setting a script trigger
Using the MK1 app, triggers can be selected from the script settings by opening up your script and pressing the ellipsis in the top right corner.

To set a trigger manually, you'll need to edit the plist located at `/Library/MK1/scripts.plist`. An example plist can be seen below, with the script name being used as a key for a dictionary.
```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>Example</key>
	<dict>
		<key>triggers</key>
		<array>
			<string>STATUSBAR-DOUBLETAP</string>
		</array>
	</dict>
</dict>
</plist>
```

## Trigger List
### Hardware Buttons

| Trigger | Description |
|:--|:--|
| `HWBUTTON-VOLUP` | Volume up button press |
| `HWBUTTON-VOLDOWN` | Description |
| `HWBUTTON-VOLUP+VOLDOWN` | Description |
| `HWBUTTON-POWER` | Description |
| `HWBUTTON-HOME` | Description |
| `HWBUTTON-HOME+VOLUP` | Description |
| `HWBUTTON-HOME+VOLDOWN` | Description |
| `HWBUTTON-HOME+POWER` | Description |
| `HWBUTTON-RINGERTOGGLE` | Description |
| `HWBUTTON-TOUCHID` | Description |

### Status Bar

| Trigger | Description |
|:--|:--|
| `STATUSBAR-SINGLETAP` | Description |
| `STATUSBAR-DOUBLETAP` | Description |
| `STATUSBAR-LONGPRESS` | Description |
| `STATUSBAR-SWIPELEFT` | Description |
| `STATUSBAR-SWIPERIGHT` | Description |

### Battery

| Trigger | Description |
|:--|:--|
| `BATTERY-STATECHANGE` | Description |
| `BATTERY-LEVELCHANGE` | Description |
| `BATTERY-LEVEL20` | Description |
| `BATTERY-LEVEL50` | Description |

### Wi-Fi

| Trigger | Description |
|:--|:--|
| `WIFI-ENABLED` | Description |
| `WIFI-DISABLED` | Description |
| `WIFI-NETWORKCHANGE` | Description |

### Bluetooth

| Trigger | Description |
|:--|:--|
| `BLUETOOTH-CONNECTEDCHANGE` | Description |

### VPN

| Trigger | Description |
|:--|:--|
| `VPN-CONNECTED` | Description |
| `VPN-CONNECTED` | Description |

### Device

| Trigger | Description |
|:--|:--|
| `APPLICATION-LAUNCH` | Description |
| `DEVICE-DARKMODETOGGLE` | Description |
| `DEVICE-SHAKE` | Description |
| `DEVICE-LOCK` | Description |
| `DEVICE-UNLOCK` | Description |

### Media

| Trigger | Description |
|:--|:--|
| `MEDIA-NOWPLAYINGCHANGE` | Description |
| `VOLUME-MEDIACHANGE` | Description |
| `VOLUME-RINGERCHANGE` | Description |

### Notifications

| Trigger | Description |
|:--|:--|
| `NOTIFICATION-RECEIVE` | Description |

#### Note
This trigger also defines JavaScript variables you can use in your script.

### Control Center

| Trigger | Description |
|:--|:--|
| `CONTROLCENTER-MODULE` | Description |

#### Note
This trigger can only be used if the MK1 Control Center toggle package is installed.
