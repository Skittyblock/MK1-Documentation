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
| `HWBUTTON-VOLUP`         | Volume up press |
| `HWBUTTON-VOLDOWN`       | Volume down press |
| `HWBUTTON-VOLUP+VOLDOWN` | Volume up and down press |
| `HWBUTTON-POWER`         | Power button press |
| `HWBUTTON-HOME`          | Home button press |
| `HWBUTTON-HOME+VOLUP`    | Home and volume up press |
| `HWBUTTON-HOME+VOLDOWN`  | Home and volume down press |
| `HWBUTTON-HOME+POWER`    | Home and power button press |
| `HWBUTTON-RINGERTOGGLE`  | Ringer switch |
| `HWBUTTON-TOUCHID`       | Touch ID press |

### Status Bar

| Trigger | Description |
|:--|:--|
| `STATUSBAR-SINGLETAP`  | Status bar single tap |
| `STATUSBAR-DOUBLETAP`  | Status bar double tap |
| `STATUSBAR-LONGPRESS`  | Status bar long press |
| `STATUSBAR-SWIPELEFT`  | Status bar swipe from right to left |
| `STATUSBAR-SWIPERIGHT` | Status bar swipe from left to right |

### Battery

| Trigger | Description |
|:--|:--|
| `BATTERY-STATECHANGE` | Battery charging state change |
| `BATTERY-LEVELCHANGE` | Battery level change |
| `BATTERY-LEVEL50`     | Battery level 50% |
| `BATTERY-LEVEL20`     | Battery level 20% |

### Wi-Fi

| Trigger | Description |
|:--|:--|
| `WIFI-ENABLED`       | Wi-Fi enabled |
| `WIFI-DISABLED`      | Wi-Fi disabled |
| `WIFI-NETWORKCHANGE` | Wi-Fi network change |

### Bluetooth

| Trigger | Description |
|:--|:--|
| `BLUETOOTH-CONNECTEDCHANGE` | Bluetooth device connection change |

### VPN

| Trigger | Description |
|:--|:--|
| `VPN-CONNECTED`    | VPN enabled |
| `VPN-DISCONNECTED` | VPN disabled |

### Device

| Trigger | Description |
|:--|:--|
| `APPLICATION-LAUNCH`    | An application is launched |
| `DEVICE-DARKMODETOGGLE` | Dark mode enabled/disabled |
| `DEVICE-SHAKE`          | Device is shaken |
| `DEVICE-LOCK`           | Device is locked |
| `DEVICE-UNLOCK`         | Device is unlocked |

### Media

| Trigger | Description |
|:--|:--|
| `MEDIA-NOWPLAYINGCHANGE` | Music begins playing |
| `VOLUME-MEDIACHANGE`     | Volume changes |
| `VOLUME-RINGERCHANGE`    | Ringer switch state changes |

### Notifications

| Trigger | Description |
|:--|:--|
| `NOTIFICATION-RECEIVE` | A notification is recieved |

#### Note
This trigger also defines JavaScript variables you can use in your script.  

| Variable | Description |
|:--|:--|
| `NOTIFICATION_HEADER` | Notification header |
| `NOTIFICATION_TITLE` | Notification title |
| `NOTIFICATION_MESSAGE` | Notification message |
| `NOTIFICATION_SUBTITLE` | Notification subtitle |
| `NOTIFICATION_TOPIC` | Notification topic |

### Control Center

| Trigger | Description |
|:--|:--|
| `CONTROLCENTER-MODULE` | The control center toggle is pressed |

#### Note
This trigger can only be used if the MK1 Control Center toggle package is installed.
