---
layout: default
title: Current Application
category: Actions
permalink: /actions/current-app
sublinks: ["currentApp.isSpringBoard()", "currentApp.bundleID()", "currentApp.name()"]
---

# Current Application
## currentApp.isSpringBoard() ##
#### Syntax
```js
var clipboard = currentApp.get();
```

#### Return value
A `Boolean` representing whether the currently open application is SpringBoard


## currentApp.bundleID() ##
#### Syntax
```js
var bundleID = currentApp.bundleID();
```

#### Return value
A `String` containing the current app's bundle identifier


## currentApp.name() ##
#### Syntax
```js
var name = currentApp.name();
```

#### Return value
A `String` containing the current app's display name
