---
layout: default
title: Creating a Script
category: Getting Started
permalink: /getting-started/creating-a-script
---

# Creating a Script
## Using the App
MK1 comes with a companion application that lets you create, delete, and completely manage all your scripts without ever leaving it. To create a new script, simply press on the add button on the home page, enter a name for your script, and press create.

## Doing it manually
MK1 scripts are stored at `/Library/MK1/Scripts`. To create a new one, make a new folder in that directory with the name of the script. Inside that folder, you'll need to create an `index.js` file and, optionally, a `Script.plist` file.

### Script.plist
The `Script.plist` file contains metadata for your script. Below you can find the available keys.

| Key | Type | Description |
|:--|:--|:--|
| `author` | String | Name of the script author |
