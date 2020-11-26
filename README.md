[![npm](https://img.shields.io/npm/v/@kronos-integration/message.svg)](https://www.npmjs.com/package/@kronos-integration/message)
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
[![minified size](https://badgen.net/bundlephobia/min/@kronos-integration/message)](https://bundlephobia.com/result?p=@kronos-integration/message)
[![downloads](http://img.shields.io/npm/dm/@kronos-integration/message.svg?style=flat-square)](https://npmjs.org/package/@kronos-integration/message)
[![Styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

kronos-message
=====
The message object is the 'data' object which will be send from step to step

# API Reference

* <a name="createMessage"></a>

## createMessage(newData, oldRequestMessage)
Creates a new request message structure. It will merge the new data into a copy of the old request.
Only thf fields 'info' and 'hops' will be copied

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| newData | <code>object</code> | This json is new generated data by the step. It has the follwing structure. 	                       newData : {                           "info" : {},                           "payload" :                         } |
| oldRequestMessage | <code>object</code> | The request message this step has received |


* <a name="addHop"></a>

## addHop(message, stepName, stepType, endpoint)
Adds a new way point to the message

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| message | <code>object</code> | The message to add the new hop |
| stepName | <code>string</code> | The name of the current step which issues this way point |
| stepType | <code>string</code> | The typeName of the step |
| endpoint | <code>string</code> | The name of endpoint the message is routed through |


* * *

install
=======

With [npm](http://npmjs.org) do:

```shell
npm install kronos-message
```

license
=======

BSD-2-Clause
