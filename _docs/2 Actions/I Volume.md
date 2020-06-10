---
layout: default
title: Volume
category: Actions
permalink: /actions/volume
sublinks: ["volume.getRinger()", "volume.setRinger()", "volume.getMedia()", "volume.setMedia()"]
---

# Volume
## volume.getRinger() ##
#### Syntax
```js
var ringVolume = volume.getLevel();
```

#### Return value
A `Number` between 0 and 1 representing the current ringer volume


## volume.setRinger() ##
#### Syntax
```js
volume.setRinger(vol);
```

#### Parameters
`vol`: A `Number` between 0 and 1 to set the ringer volume


## volume.getMedia() ##
#### Syntax
```js
var mediaVolume = volume.getMedia();
```

#### Return value
A `Number` between 0 and 1 representing the current media volume


## volume.setMedia() ##
#### Syntax
```js
volume.setMedia(vol);
```

#### Parameters
`vol`: A `Number` between 0 and 1 to set the media volume
