
# Interface: Options

## Hierarchy

* **Options**

## Index

### Properties

* [deepFunction](deepequal.options.md#optional-deepfunction)
* [part](deepequal.options.md#optional-part)
* [prototype](deepequal.options.md#optional-prototype)
* [skip](deepequal.options.md#optional-skip)
* [symbols](deepequal.options.md#optional-symbols)

## Properties

### `Optional` deepFunction

• **deepFunction**? : *boolean*

Compare functions with difference references by comparing their internal code and properties.

**`default`** false

___

### `Optional` part

• **part**? : *boolean*

Allow partial match.

**`default`** false

___

### `Optional` prototype

• **prototype**? : *boolean*

Compare the objects' prototypes.

**`default`** true

___

### `Optional` skip

• **skip**? : *string | symbol[]*

List of object keys to ignore different values of.

**`default`** null

___

### `Optional` symbols

• **symbols**? : *boolean*

Compare symbol properties.

**`default`** true
