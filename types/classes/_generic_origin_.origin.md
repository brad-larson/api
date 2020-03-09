[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["generic/Origin"](../modules/_generic_origin_.md) › [Origin](_generic_origin_.origin.md)

# Class: Origin

**`name`** Origin

**`description`** 
Where Origin occurs, it should be ignored as an internal-only value, so it should
never actually be constructed

## Hierarchy

* [Null](_primitive_null_.null.md)

  ↳ **Origin**

## Implements

* [Codec](../interfaces/_types_codec_.codec.md)

## Index

### Constructors

* [constructor](_generic_origin_.origin.md#constructor)

### Properties

* [registry](_generic_origin_.origin.md#registry)

### Accessors

* [encodedLength](_generic_origin_.origin.md#encodedlength)
* [hash](_generic_origin_.origin.md#hash)
* [isEmpty](_generic_origin_.origin.md#isempty)

### Methods

* [eq](_generic_origin_.origin.md#eq)
* [toHex](_generic_origin_.origin.md#tohex)
* [toHuman](_generic_origin_.origin.md#tohuman)
* [toJSON](_generic_origin_.origin.md#tojson)
* [toRawType](_generic_origin_.origin.md#torawtype)
* [toString](_generic_origin_.origin.md#tostring)
* [toU8a](_generic_origin_.origin.md#tou8a)

## Constructors

###  constructor

\+ **new Origin**(`registry`: [Registry](../interfaces/_types_registry_.registry.md)): *[Origin](_generic_origin_.origin.md)*

*Overrides [Null](_primitive_null_.null.md).[constructor](_primitive_null_.null.md#constructor)*

*Defined in [packages/types/src/generic/Origin.ts:15](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/generic/Origin.ts#L15)*

**Parameters:**

Name | Type |
------ | ------ |
`registry` | [Registry](../interfaces/_types_registry_.registry.md) |

**Returns:** *[Origin](_generic_origin_.origin.md)*

## Properties

###  registry

• **registry**: *[Registry](../interfaces/_types_registry_.registry.md)*

*Implementation of [Codec](../interfaces/_types_codec_.codec.md).[registry](../interfaces/_types_codec_.codec.md#registry)*

*Inherited from [Null](_primitive_null_.null.md).[registry](_primitive_null_.null.md#registry)*

*Defined in [packages/types/src/primitive/Null.ts:16](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L16)*

## Accessors

###  encodedLength

• **get encodedLength**(): *number*

*Inherited from [Null](_primitive_null_.null.md).[encodedLength](_primitive_null_.null.md#encodedlength)*

*Defined in [packages/types/src/primitive/Null.ts:25](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L25)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Inherited from [Null](_primitive_null_.null.md).[hash](_primitive_null_.null.md#hash)*

*Defined in [packages/types/src/primitive/Null.ts:32](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L32)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Inherited from [Null](_primitive_null_.null.md).[isEmpty](_primitive_null_.null.md#isempty)*

*Defined in [packages/types/src/primitive/Null.ts:39](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L39)*

**`description`** Checks if the value is an empty value (always true)

**Returns:** *boolean*

## Methods

###  eq

▸ **eq**(`other?`: any): *boolean*

*Implementation of [Codec](../interfaces/_types_codec_.codec.md)*

*Inherited from [Null](_primitive_null_.null.md).[eq](_primitive_null_.null.md#eq)*

*Defined in [packages/types/src/primitive/Null.ts:46](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L46)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | any |

**Returns:** *boolean*

___

###  toHex

▸ **toHex**(): *string*

*Inherited from [Null](_primitive_null_.null.md).[toHex](_primitive_null_.null.md#tohex)*

*Defined in [packages/types/src/primitive/Null.ts:53](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L53)*

**`description`** Returns a hex string representation of the value

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(): *null*

*Inherited from [Null](_primitive_null_.null.md).[toHuman](_primitive_null_.null.md#tohuman)*

*Defined in [packages/types/src/primitive/Null.ts:60](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L60)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Returns:** *null*

___

###  toJSON

▸ **toJSON**(): *null*

*Implementation of [Codec](../interfaces/_types_codec_.codec.md)*

*Inherited from [Null](_primitive_null_.null.md).[toJSON](_primitive_null_.null.md#tojson)*

*Defined in [packages/types/src/primitive/Null.ts:67](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L67)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *null*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [Codec](../interfaces/_types_codec_.codec.md)*

*Inherited from [Null](_primitive_null_.null.md).[toRawType](_primitive_null_.null.md#torawtype)*

*Defined in [packages/types/src/primitive/Null.ts:74](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L74)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [Codec](../interfaces/_types_codec_.codec.md)*

*Inherited from [Null](_primitive_null_.null.md).[toString](_primitive_null_.null.md#tostring)*

*Defined in [packages/types/src/primitive/Null.ts:81](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L81)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

*Inherited from [Null](_primitive_null_.null.md).[toU8a](_primitive_null_.null.md#tou8a)*

*Defined in [packages/types/src/primitive/Null.ts:90](https://github.com/polkadot-js/api/blob/8ad3d35dd2/packages/types/src/primitive/Null.ts#L90)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value has none of the type-specific prefixes (internal)  |

**Returns:** *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*