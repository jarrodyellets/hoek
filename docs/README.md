
# @hapi/hoek

## Index

### Modules

* [applyToDefaults](modules/applytodefaults.md)
* [clone](modules/clone.md)
* [contain](modules/contain.md)
* [deepEqual](modules/deepequal.md)
* [internals](modules/internals.md)
* [intersect](modules/intersect.md)
* [merge](modules/merge.md)
* [reach](modules/reach.md)
* [ts](modules/ts.md)

### Classes

* [Bench](classes/bench.md)

### Functions

* [assert](README.md#assert)
* [block](README.md#block)
* [escapeHeaderAttribute](README.md#escapeheaderattribute)
* [escapeHtml](README.md#escapehtml)
* [escapeJson](README.md#escapejson)
* [escapeRegex](README.md#escaperegex)
* [flatten](README.md#flatten)
* [ignore](README.md#ignore)
* [once](README.md#once)
* [reachTemplate](README.md#reachtemplate)
* [stringify](README.md#stringify)
* [wait](README.md#wait)

## Functions

###  assert

▸ **assert**(`condition`: any, `error`: Error): *void*

Throw an error if condition is falsy.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`condition` | any | If `condition` is not truthy, an exception is thrown. |
`error` | Error | The error thrown if the condition fails.  |

**Returns:** *void*

Does not return a value but throws if the `condition` is falsy.

▸ **assert**(`condition`: any, ...`args`: any): *void*

Throw an error if condition is falsy.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`condition` | any | If `condition` is not truthy, an exception is thrown. |
`...args` | any | Any number of values, concatenated together (space separated) to create the error message.  |

**Returns:** *void*

Does not return a value but throws if the `condition` is falsy.

___

###  block

▸ **block**(): *Promise‹void›*

Returns a Promise that never resolves.

**Returns:** *Promise‹void›*

___

###  escapeHeaderAttribute

▸ **escapeHeaderAttribute**(`attribute`: string): *string*

Escape string for usage as an attribute value in HTTP headers.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`attribute` | string | The string to be escaped.  |

**Returns:** *string*

The escaped string. Will throw on invalid characters that are not supported to be escaped.

___

###  escapeHtml

▸ **escapeHtml**(`string`: string): *string*

Escape string for usage in HTML.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`string` | string | The string to be escaped.  |

**Returns:** *string*

The escaped string.

___

###  escapeJson

▸ **escapeJson**(`string`: string): *string*

Escape string for usage in JSON.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`string` | string | The string to be escaped.  |

**Returns:** *string*

The escaped string.

___

###  escapeRegex

▸ **escapeRegex**(`string`: string): *string*

Escape string for Regex construction by prefixing all reserved characters with a backslash.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`string` | string | The string to be escaped.  |

**Returns:** *string*

The escaped string.

___

###  flatten

▸ **flatten**<**T**>(`array`: ArrayLike‹T | ReadonlyArray‹T››, `target?`: ArrayLike‹T | ReadonlyArray‹T››): *T[]*

Flatten an array with sub arrays

**Type parameters:**

▪ **T**

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`array` | ArrayLike‹T &#124; ReadonlyArray‹T›› | an array of items or other arrays to flatten. |
`target?` | ArrayLike‹T &#124; ReadonlyArray‹T›› | if provided, an array to shallow copy the flattened `array` items to  |

**Returns:** *T[]*

a flat array of the provided values (appended to `target` is provided).

___

###  ignore

▸ **ignore**(...`ignore`: any): *void*

A reusable no-op function.

**Parameters:**

Name | Type |
------ | ------ |
`...ignore` | any |

**Returns:** *void*

___

###  once

▸ **once**<**T**>(`method`: T): *T*

Wraps a function to ensure it can only execute once.

**Type parameters:**

▪ **T**: *Function*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`method` | T | The function to be wrapped.  |

**Returns:** *T*

The wrapped function.

___

###  reachTemplate

▸ **reachTemplate**(`obj`: object | null, `template`: string, `options?`: [Options](interfaces/reach.options.md)): *string*

Replace string parameters (using format "{path.to.key}") with their corresponding object key values using `Hoek.reach()`.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`obj` | object &#124; null | the object from which to look up the value. |
`template` | string | the string containing {} enclosed key paths to be replaced.  |
`options?` | [Options](interfaces/reach.options.md) | - |

**Returns:** *string*

The template string with the {} enclosed keys replaced with looked-up values.

___

###  stringify

▸ **stringify**(`value`: any, `replacer?`: any, `space?`: string | number): *string*

Converts a JavaScript value to a JavaScript Object Notation (JSON) string with protection against thrown errors.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | any | A JavaScript value, usually an object or array, to be converted. |
`replacer?` | any | The JSON.stringify() `replacer` argument. |
`space?` | string &#124; number | Adds indentation, white space, and line break characters to the return-value JSON text to make it easier to read.  |

**Returns:** *string*

The JSON string. If the operation fails, an error string value is returned (no exception thrown).

___

###  wait

▸ **wait**(`timeout?`: number): *Promise‹void›*

Returns a Promise that resolves after the requested timeout.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`timeout?` | number | The number of milliseconds to wait before resolving the Promise.  |

**Returns:** *Promise‹void›*

A Promise.
