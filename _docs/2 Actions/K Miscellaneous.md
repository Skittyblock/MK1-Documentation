---
layout: default
title: Miscellaneous
category: Actions
permalink: /actions/miscellaneous
sublinks: ["setTimeout()", "setInterval()", "clearTimeout()", "clearInterval()", "alert()", "confirm()", "prompt()", "menu()", "shellrun()", "openURL()", "openApp()", "sendDarwinNotif()", "sendRocketBootstrapMessage()", "textToSpeech()", "toggleReachability()", "takeScreenshot()"]
---

# Miscellaneous
## Note
Some of these actions are custom implementations of functions you usually see in JavaScript, but don't exist in JavaScriptCore (without a web browser).

## setTimeout() ##
[Mozilla reference](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setTimeout)


## setInterval() ##
[Mozilla reference](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setInterval)


## clearTimeout() ##
[Mozilla reference](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/clearTimeout)


## clearInterval() ##
[Mozilla reference](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/clearInterval)


## alert() ##
#### Syntax
```js
alert(title, message);
```

#### Parameters
`title`: A `String` containing the title of your alert  
`message`: A `String` containing the message of your alert


## confirm() ##
#### Syntax
```js
confirm(title, message, callback);
```

#### Parameters
`title`: A `String` containing the title of your alert  
`message`: A `String` containing the message of your alert  
`callback`: A callback function that's called with a `Boolean` representing whether OK or Cancel was pressed


## prompt() ##
#### Syntax
```js
prompt(title, message, callback);
```

#### Parameters
`title`: A `String` containing the title of your alert  
`message`: A `String` containing the message of your alert  
`callback`: A callback function that's called with a `String` containing what was entered


## menu() ##
#### Syntax
```js
menu(title, message, options, callback);
```

#### Parameters
`title`: A `String` containing the title of your alert  
`message`: A `String` containing the message of your alert  
`option`: An `Array` of `Strings` containing the titles of your options  
`callback`: A callback function that's called with a `Number` representing the index of the option chosen


## shellrun() ##
#### Syntax
```js
shellrun(command, callback);
```

#### Parameters
`command`: A `String` containing the command you want sent  
`callback`: An optional callback function that's called with a `Number` representing the exit status, a `String` containing stdout, and a `String` containing stderr.


## openURL() ##
#### Syntax
```js
openURL(url);
```

#### Parameters
`url`: A `String` containing the URL you want to open


## openApp() ##
#### Syntax
```js
openApp(id);
```

#### Parameters
`id`: A `String` containing the bundle identifier of the app you want to open


## sendDarwinNotif() ##
#### Syntax
```js
sendDarwinNotif(string);
```

#### Parameters
`string`: A `String` containing the darwin notification identifier you want to send


## sendRocketBootstrapMessage() ##
#### Syntax
```js
sendRocketBootstrapMessage(center, message, userInfo);
```

#### Parameters
`center`: A `String` containing the rocket bootstrap center to send the message  
`message`: A `String` containing the message to send  
`userInfo`: An `Object` containing the data to send


## textToSpeech() ##
#### Syntax
```js
textToSpeech(text);
```

#### Parameters
`text`: A `String` containing the text to be spoken


## toggleReachability() ##
#### Syntax
```js
toggleReachability();
```


## takeScreenshot() ##
#### Syntax
```js
takeScreenshot();
```
