
# Class: Bench

A benchmarking timer, using the internal node clock for maximum accuracy.

## Hierarchy

* **Bench**

## Index

### Constructors

* [constructor](bench.md#constructor)

### Properties

* [ts](bench.md#ts)

### Methods

* [elapsed](bench.md#elapsed)
* [reset](bench.md#reset)
* [now](bench.md#static-now)

## Constructors

###  constructor

\+ **new Bench**(): *[Bench](bench.md)*

**Returns:** *[Bench](bench.md)*

## Properties

###  ts

• **ts**: *number*

The starting timestamp expressed in the number of milliseconds since the epoch.

## Methods

###  elapsed

▸ **elapsed**(): *number*

The time in milliseconds since the object was created.

**Returns:** *number*

___

###  reset

▸ **reset**(): *void*

Reset the `ts` value to now.

**Returns:** *void*

___

### `Static` now

▸ **now**(): *number*

The current time in milliseconds since the epoch.

**Returns:** *number*
