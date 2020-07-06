[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/types/src/codec/Date"](../modules/_packages_types_src_codec_date_.md) › [CodecDate](_packages_types_src_codec_date_.codecdate.md)

# Class: CodecDate

**`name`** Date

**`description`** 
A wrapper around seconds/timestamps. Internally the representation only has
second precicion (aligning with Rust), so any numbers passed an/out are always
per-second. For any encoding/decoding the 1000 multiplier would be applied to
get it in line with JavaScript formats. It extends the base JS `Date` object
and has all the methods available that are applicable to any `Date`

## Hierarchy

* [Date](_packages_types_src_codec_date_.codecdate.md#static-date)

  ↳ **CodecDate**

## Implements

* [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)

## Index

### Constructors

* [constructor](_packages_types_src_codec_date_.codecdate.md#constructor)

### Properties

* [registry](_packages_types_src_codec_date_.codecdate.md#readonly-registry)
* [Date](_packages_types_src_codec_date_.codecdate.md#static-date)

### Accessors

* [encodedLength](_packages_types_src_codec_date_.codecdate.md#encodedlength)
* [hash](_packages_types_src_codec_date_.codecdate.md#hash)
* [isEmpty](_packages_types_src_codec_date_.codecdate.md#isempty)

### Methods

* [bitLength](_packages_types_src_codec_date_.codecdate.md#bitlength)
* [eq](_packages_types_src_codec_date_.codecdate.md#eq)
* [toBn](_packages_types_src_codec_date_.codecdate.md#tobn)
* [toHex](_packages_types_src_codec_date_.codecdate.md#tohex)
* [toHuman](_packages_types_src_codec_date_.codecdate.md#tohuman)
* [toJSON](_packages_types_src_codec_date_.codecdate.md#tojson)
* [toNumber](_packages_types_src_codec_date_.codecdate.md#tonumber)
* [toRawType](_packages_types_src_codec_date_.codecdate.md#torawtype)
* [toString](_packages_types_src_codec_date_.codecdate.md#tostring)
* [toU8a](_packages_types_src_codec_date_.codecdate.md#tou8a)

## Constructors

###  constructor

\+ **new CodecDate**(`registry`: [Registry](../interfaces/_packages_types_src_types_registry_.registry.md), `value`: [CodecDate](_packages_types_src_codec_date_.codecdate.md) | [Date](_packages_types_src_codec_date_.codecdate.md#static-date) | [AnyNumber](../modules/_packages_types_src_types_helpers_.md#anynumber)): *[CodecDate](_packages_types_src_codec_date_.codecdate.md)*

*Defined in [packages/types/src/codec/Date.ts:27](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L27)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`registry` | [Registry](../interfaces/_packages_types_src_types_registry_.registry.md) | - |
`value` | [CodecDate](_packages_types_src_codec_date_.codecdate.md) &#124; [Date](_packages_types_src_codec_date_.codecdate.md#static-date) &#124; [AnyNumber](../modules/_packages_types_src_types_helpers_.md#anynumber) | 0 |

**Returns:** *[CodecDate](_packages_types_src_codec_date_.codecdate.md)*

## Properties

### `Readonly` registry

• **registry**: *[Registry](../interfaces/_packages_types_src_types_registry_.registry.md)*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md).[registry](../interfaces/_packages_types_src_types_codec_.codec.md#readonly-registry)*

*Defined in [packages/types/src/codec/Date.ts:27](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L27)*

___

### `Static` Date

▪ **Date**: *DateConstructor*

Defined in node_modules/typescript/lib/lib.es5.d.ts:907

## Accessors

###  encodedLength

• **get encodedLength**(): *number*

*Defined in [packages/types/src/codec/Date.ts:53](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L53)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Defined in [packages/types/src/codec/Date.ts:60](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L60)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Defined in [packages/types/src/codec/Date.ts:67](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L67)*

**`description`** Checks if the value is an empty value

**Returns:** *boolean*

## Methods

###  bitLength

▸ **bitLength**(): *[UIntBitLength](../modules/_packages_types_src_codec_abstractint_.md#uintbitlength)*

*Defined in [packages/types/src/codec/Date.ts:81](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L81)*

**`description`** Returns the number of bits in the value

**Returns:** *[UIntBitLength](../modules/_packages_types_src_codec_abstractint_.md#uintbitlength)*

___

###  eq

▸ **eq**(`other?`: unknown): *boolean*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/Date.ts:74](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L74)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | unknown |

**Returns:** *boolean*

___

###  toBn

▸ **toBn**(): *BN*

*Defined in [packages/types/src/codec/Date.ts:88](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L88)*

**`description`** Returns the BN representation of the timestamp

**Returns:** *BN*

___

###  toHex

▸ **toHex**(`isLe`: boolean): *string*

*Defined in [packages/types/src/codec/Date.ts:95](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L95)*

**`description`** Returns a hex string representation of the value

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`isLe` | boolean | false |

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(): *string*

*Defined in [packages/types/src/codec/Date.ts:106](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L106)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Returns:** *string*

___

###  toJSON

▸ **toJSON**(): *any*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Overrides void*

*Defined in [packages/types/src/codec/Date.ts:113](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L113)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *any*

___

###  toNumber

▸ **toNumber**(): *number*

*Defined in [packages/types/src/codec/Date.ts:122](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L122)*

**`description`** Returns the number representation for the timestamp

**Returns:** *number*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/Date.ts:129](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L129)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Overrides void*

*Defined in [packages/types/src/codec/Date.ts:136](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L136)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Defined in [packages/types/src/codec/Date.ts:146](https://github.com/polkadot-js/api/blob/28631f7180/packages/types/src/codec/Date.ts#L146)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value has none of the type-specific prefixes (internal)  |

**Returns:** *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*
