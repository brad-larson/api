[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/types/src/codec/StructAny"](../modules/_packages_types_src_codec_structany_.md) › [StructAny](_packages_types_src_codec_structany_.structany.md)

# Class: StructAny

**`name`** Json

**`description`** 
Wraps the a JSON structure retrieve via RPC. It extends the standard JS Map with. While it
implements a Codec, it is limited in that it can only be used with input objects via RPC,
i.e. no hex decoding. Unlike a struct, this waps a JSON object with unknown keys

## Hierarchy

* [Map](_packages_types_src_codec_struct_.struct.md#static-map)‹string, any›

  ↳ **StructAny**

## Implements

* [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)

## Index

### Constructors

* [constructor](_packages_types_src_codec_structany_.structany.md#constructor)

### Properties

* [registry](_packages_types_src_codec_structany_.structany.md#readonly-registry)
* [Map](_packages_types_src_codec_structany_.structany.md#static-map)

### Accessors

* [encodedLength](_packages_types_src_codec_structany_.structany.md#encodedlength)
* [hash](_packages_types_src_codec_structany_.structany.md#hash)
* [isEmpty](_packages_types_src_codec_structany_.structany.md#isempty)

### Methods

* [eq](_packages_types_src_codec_structany_.structany.md#eq)
* [toHex](_packages_types_src_codec_structany_.structany.md#tohex)
* [toHuman](_packages_types_src_codec_structany_.structany.md#tohuman)
* [toJSON](_packages_types_src_codec_structany_.structany.md#tojson)
* [toRawType](_packages_types_src_codec_structany_.structany.md#torawtype)
* [toString](_packages_types_src_codec_structany_.structany.md#tostring)
* [toU8a](_packages_types_src_codec_structany_.structany.md#tou8a)

## Constructors

###  constructor

\+ **new StructAny**(`registry`: [Registry](../interfaces/_packages_types_src_types_registry_.registry.md), `value?`: Record‹string, unknown› | null): *[StructAny](_packages_types_src_codec_structany_.structany.md)*

*Defined in [packages/types/src/codec/StructAny.ts:29](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L29)*

**Parameters:**

Name | Type |
------ | ------ |
`registry` | [Registry](../interfaces/_packages_types_src_types_registry_.registry.md) |
`value?` | Record‹string, unknown› &#124; null |

**Returns:** *[StructAny](_packages_types_src_codec_structany_.structany.md)*

## Properties

### `Readonly` registry

• **registry**: *[Registry](../interfaces/_packages_types_src_types_registry_.registry.md)*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md).[registry](../interfaces/_packages_types_src_types_codec_.codec.md#readonly-registry)*

*Defined in [packages/types/src/codec/StructAny.ts:29](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L29)*

___

### `Static` Map

▪ **Map**: *MapConstructor*

Defined in node_modules/typescript/lib/lib.es2015.collection.d.ts:36

## Accessors

###  encodedLength

• **get encodedLength**(): *number*

*Defined in [packages/types/src/codec/StructAny.ts:56](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L56)*

**`description`** Always 0, never encodes as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Defined in [packages/types/src/codec/StructAny.ts:63](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L63)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Defined in [packages/types/src/codec/StructAny.ts:70](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L70)*

**`description`** Checks if the value is an empty value

**Returns:** *boolean*

## Methods

###  eq

▸ **eq**(`other?`: unknown): *boolean*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/StructAny.ts:77](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L77)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | unknown |

**Returns:** *boolean*

___

###  toHex

▸ **toHex**(): *string*

*Defined in [packages/types/src/codec/StructAny.ts:84](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L84)*

**`description`** Unimplemented, will throw

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(): *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

*Defined in [packages/types/src/codec/StructAny.ts:91](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L91)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Returns:** *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

___

###  toJSON

▸ **toJSON**(): *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/StructAny.ts:98](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L98)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/StructAny.ts:109](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L109)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/StructAny.ts:116](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L116)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Defined in [packages/types/src/codec/StructAny.ts:124](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/StructAny.ts#L124)*

**`description`** Unimplemented, will throw

**Parameters:**

Name | Type |
------ | ------ |
`isBare?` | undefined &#124; false &#124; true |

**Returns:** *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*
