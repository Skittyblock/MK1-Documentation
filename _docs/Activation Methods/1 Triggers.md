---
layout: default
title: Triggers
category: 1Activation Methods
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

| Trigger | Description |
|:--|:--|
| `HWBUTTON-VOLUP` | Volume up button press |
