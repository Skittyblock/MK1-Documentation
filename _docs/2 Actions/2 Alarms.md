---
layout: default
title: Alarms
category: Actions
permalink: /actions/alarms
sublinks: ["alarm.getTitle()", "alarm.getHour()", "alarm.getMinute()", "alarm.isEnabled()", "alarm.isSnoozed()", "alarm.getNextFireDate()", "alarm.setHour()", "alarm.setMinute()", "alarm.setEnabled()", "alarm.snooze()"]
---

# Alarms

## alarm.getTitle()
#### Syntax
```js
var title = alarm.getTitle(id);
```

#### Parameters
`id`: A `String` representing the alarm identifiers (example: `"43C51F7E-FB89-49B3-B090-114AB2E1FB98"`)

#### Return value
A `String` containing the alarm title

## alarm.getHour()
#### Syntax
```js
var hour = alarm.getHour(id);
```

#### Parameters
`id`: A `String` representing the alarm identifier

#### Return value
A `Number` representing the hour of the alarm target time


## alarm.getMinute()
#### Syntax
```js
var minute = alarm.getMinute(id);
```

#### Parameters
`id`: A `String` representing the alarm identifier

#### Return value
A `Number` representing the minute of the alarm target time


## alarm.isEnabled()
#### Syntax
```js
var snoozed = alarm.isEnabled(id);
```

#### Parameters
`id`: A `String` representing the alarm identifier

#### Return value
A `Boolean` representing whether or not the alarm is enabled


## alarm.isSnoozed()
#### Syntax
```js
var snoozed = alarm.isSnoozed(id);
```

#### Parameters
`id`: A `String` representing the alarm identifier

#### Return value
A `Boolean` representing whether or not the alarm is snoozed


## alarm.getNextFireDate()
#### Syntax
```js
var nextFire = alarm.getNextFireDate(id);
```

#### Parameters
`id`: A `String` representing the alarm identifier

#### Return value
A `Date` object representing the next time the alarm would be activated


## alarm.setHour()
#### Syntax
```js
alarm.setHour(id, hour);
```

#### Parameters
`id`: A `String` representing the alarm identifier  
`hour`: A `Number` representing the hour you'd like to set the alarm to


## alarm.setMinute()
#### Syntax
```js
alarm.setMinute(id, minute);
```

#### Parameters
`id`: A `String` representing the alarm identifier  
`minute`: A `Number` representing the minute you'd like to set the alarm to


## alarm.setEnabled()
#### Syntax
```js
alarm.setEnabled(id, enabled);
```

#### Parameters
`id`: A `String` representing the alarm identifier  
`enabled`: A `Boolean` representing whether alarm should be enabled or disabled


## alarm.snooze()
#### Syntax
```js
alarm.snooze(id);
```

#### Parameters
`id`: A `String` representing the alarm identifier
