[![License](https://img.shields.io/badge/License-0BSD-blue.svg)](https://spdx.org/licenses/0BSD.html)
[![GitHub Issues](https://img.shields.io/github/issues/Kronos-Integration/message.svg?style=flat-square)](https://github.com/Kronos-Integration/message/issues)
[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FKronos-Integration%2Fmessage%2Fbadge\&style=flat)](https://actions-badge.atrox.dev/Kronos-Integration/message/goto)
[![Styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![Known Vulnerabilities](https://snyk.io/test/github/Kronos-Integration/message/badge.svg)](https://snyk.io/test/github/Kronos-Integration/message)
[![Coverage Status](https://coveralls.io/repos/Kronos-Integration/message/badge.svg)](https://coveralls.io/github/Kronos-Integration/message)

# @kronos-integration/message

The message object is the 'data' object which will be send from step to step

# API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

*   [createMessage](#createmessage)
    *   [Parameters](#parameters)
*   [addHop](#addhop)
    *   [Parameters](#parameters-1)

## createMessage

Creates a new request message structure. It will merge the new data into a copy of the old request.
Only the fields 'info' and 'hops' will be copied

### Parameters

*   `newData`  {object} This json is new generated data by the step. It has the follwing structure.
    newData : {
    "info" : {},
    "payload" :
    }
*   `oldRequestMessage`  {object} The request message this step has received

## addHop

Adds a new way point to the message

### Parameters

*   `message`  {object} The message to add the new hop
*   `stepName`  {string} The name of the current step which issues this way point
*   `stepType`  {string} The typeName of the step
*   `endpoint`  {string} The name of endpoint the message is routed through

# install

With [npm](http://npmjs.org) do:

```shell
npm install @kronos-integration/message
```

# license

BSD-2-Clause
