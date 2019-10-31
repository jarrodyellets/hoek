
# Module: applyToDefaults

## Callable

▸ **applyToDefaults**<**T**>(`defaults`: Partial‹T›, `source`: Partial‹T› | boolean | null, `options?`: [Options](../interfaces/applytodefaults.options.md)): *Partial‹T›*

Apply source to a copy of the defaults.

**Type parameters:**

▪ **T**: *object*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`defaults` | Partial‹T› | An object with the default values to use of `options` does not contain the same keys. |
`source` | Partial‹T› &#124; boolean &#124; null | The source used to override the `defaults`. |
`options?` | [Options](../interfaces/applytodefaults.options.md) | Optional settings.  |

**Returns:** *Partial‹T›*

A copy of `defaults` with `source` keys overriding any conflicts.

## Index

### Interfaces

* [Options](../interfaces/applytodefaults.options.md)
