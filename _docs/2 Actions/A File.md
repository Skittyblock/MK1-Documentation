---
layout: default
title: Files
category: Actions
permalink: /actions/files
sublinks: ["file.read()", "file.write()", "file.readPlist()", "file.writePlist()", "file.writePreferencesPlist()"]
---

# Files
## file.read() ##
#### Syntax
```js
var data = file.read(path);
```

#### Parameters
`path`: A `String` containing the file path you're reading

#### Return value
A `String` containing the file's contents


## file.write() ##
#### Syntax
```js
file.write(path, string);
```

#### Parameters
`path`: A `String` containing the file path you're writing to  
`string`: A `String` that you want to be written to the file


## file.readPlist() ##
#### Syntax
```js
var data = file.readPlist(path);
```

#### Parameters
`path`: A `String` containing the file path you're reading

#### Return value
An `Object` containing the plist file's contents


## file.writePlist() ##
#### Syntax
```js
file.writePlist(path, data);
```

#### Parameters
`path`: A `String` containing the file path you're writing to  
`data`: An `Object` that you want to be written to the plist file


## file.writePreferencesPlist() ##
#### Syntax
```js
file.writePreferencesPlist(domain, data);
```

#### Parameters
`domain`: A `String` containing the preference domain you're writing to  
`data`: An `Object` with data that you want to be written to the preference file

#### Note
This action is best used with `sendDarwinNotif` to update tweak preferences without respringing
