---
layout: default
title: MK1
category: Actions
permalink: /actions/mk1
sublinks: ["MK1.runScript()", "MK1.runTrigger()", "MK1.setAlertOnError()", "MK1.version", "MK1.commit", "MK1.copyright", "MK1.scriptDataDir"]
---

# MK1
## MK1.runScript() ##
#### Syntax
```js
MK1.runScript(name, argument);
```

#### Parameters
`name`: A `String` containing the name of the script to run  
`argument`: An optional `String` passed into the script and saved in the `MK1_ARG` variable

## MK1.runTrigger() ##
#### Syntax
```js
MK1.runTrigger(name, argument);
```

#### Parameters
`name`: A `String` containing the name of the trigger to activate  
`argument`: An optional `String` passed into each script and saved in the `MK1_ARG` variable

## MK1.setAlertOnError() ##
#### Syntax
```js
MK1.setAlertOnError(alert);
```

#### Parameters
`alert`: A `Boolean` representing whether you want MK1 to shown an alert when an error occurs or not


## MK1.version ##
#### Syntax
```js
var version = MK1.version;
```


## MK1.commit ##
#### Syntax
```js
var commit = MK1.commit;
```


## MK1.copyright ##
#### Syntax
```js
var copyright = MK1.copyright;
```


## MK1.scriptDataDir ##
#### Syntax
```js
var dataDirectory = MK1.scriptDataDir;
```
