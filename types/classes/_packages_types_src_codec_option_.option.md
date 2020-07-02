[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/types/src/codec/Option"](../modules/_packages_types_src_codec_option_.md) › [Option](_packages_types_src_codec_option_.option.md)

# Class: Option ‹**T**›

**`name`** Option

**`description`** 
An Option is an optional field. Basically the first byte indicates that there is
is value to follow. If the byte is `1` there is an actual value. So the Option
implements that - decodes, checks for optionality and wraps the required structure
with a value if/as required/found.

## Type parameters

▪ **T**: *[Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

## Hierarchy

* [Base](_packages_types_src_codec_base_.base.md)‹T›

  ↳ **Option**

## Implements

* [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)

## Index

### Constructors

* [constructor](_packages_types_src_codec_option_.option.md#constructor)

### Properties

* [registry](_packages_types_src_codec_option_.option.md#readonly-registry)

### Accessors

* [encodedLength](_packages_types_src_codec_option_.option.md#encodedlength)
* [hash](_packages_types_src_codec_option_.option.md#hash)
* [isEmpty](_packages_types_src_codec_option_.option.md#isempty)
* [isNone](_packages_types_src_codec_option_.option.md#isnone)
* [isSome](_packages_types_src_codec_option_.option.md#issome)
* [value](_packages_types_src_codec_option_.option.md#value)

### Methods

* [eq](_packages_types_src_codec_option_.option.md#eq)
* [toHex](_packages_types_src_codec_option_.option.md#tohex)
* [toHuman](_packages_types_src_codec_option_.option.md#tohuman)
* [toJSON](_packages_types_src_codec_option_.option.md#tojson)
* [toRawType](_packages_types_src_codec_option_.option.md#torawtype)
* [toString](_packages_types_src_codec_option_.option.md#tostring)
* [toU8a](_packages_types_src_codec_option_.option.md#tou8a)
* [unwrap](_packages_types_src_codec_option_.option.md#unwrap)
* [unwrapOr](_packages_types_src_codec_option_.option.md#unwrapor)
* [unwrapOrDefault](_packages_types_src_codec_option_.option.md#unwrapordefault)
* [with](_packages_types_src_codec_option_.option.md#static-with)

## Constructors

###  constructor

\+ **new Option**(`registry`: [Registry](../interfaces/_packages_types_src_types_registry_.registry.md), `typeName`: [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹T› | keyof InterfaceTypes, `value?`: unknown): *[Option](_packages_types_src_codec_option_.option.md)*

*Overrides void*

*Defined in [packages/types/src/codec/Option.ts:52](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L52)*

**Parameters:**

Name | Type |
------ | ------ |
`registry` | [Registry](../interfaces/_packages_types_src_types_registry_.registry.md) |
`typeName` | [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹T› &#124; keyof InterfaceTypes |
`value?` | unknown |

**Returns:** *[Option](_packages_types_src_codec_option_.option.md)*

## Properties

### `Readonly` registry

• **registry**: *[Registry](../interfaces/_packages_types_src_types_registry_.registry.md)*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md).[registry](../interfaces/_packages_types_src_types_codec_.codec.md#readonly-registry)*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[registry](_packages_types_src_codec_base_.base.md#readonly-registry)*

*Defined in [packages/types/src/codec/Base.ts:17](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Base.ts#L17)*

## Accessors

###  encodedLength

• **get encodedLength**(): *number*

*Overrides [Base](_packages_types_src_codec_base_.base.md).[encodedLength](_packages_types_src_codec_base_.base.md#encodedlength)*

*Defined in [packages/types/src/codec/Option.ts:73](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L73)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[hash](_packages_types_src_codec_base_.base.md#hash)*

*Defined in [packages/types/src/codec/Base.ts:36](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Base.ts#L36)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Overrides [Base](_packages_types_src_codec_base_.base.md).[isEmpty](_packages_types_src_codec_base_.base.md#isempty)*

*Defined in [packages/types/src/codec/Option.ts:81](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L81)*

**`description`** Checks if the Option has no value

**Returns:** *boolean*

___

###  isNone

• **get isNone**(): *boolean*

*Defined in [packages/types/src/codec/Option.ts:88](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L88)*

**`description`** Checks if the Option has no value

**Returns:** *boolean*

___

###  isSome

• **get isSome**(): *boolean*

*Defined in [packages/types/src/codec/Option.ts:95](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L95)*

**`description`** Checks if the Option has a value

**Returns:** *boolean*

___

###  value

• **get value**(): *[Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/Option.ts:102](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L102)*

**`description`** The actual value for the Option

**Returns:** *[Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

## Methods

###  eq

▸ **eq**(`other?`: unknown): *boolean*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Overrides [Base](_packages_types_src_codec_base_.base.md).[eq](_packages_types_src_codec_base_.base.md#eq)*

*Defined in [packages/types/src/codec/Option.ts:109](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L109)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | unknown |

**Returns:** *boolean*

___

###  toHex

▸ **toHex**(): *string*

*Overrides [Base](_packages_types_src_codec_base_.base.md).[toHex](_packages_types_src_codec_base_.base.md#tohex)*

*Defined in [packages/types/src/codec/Option.ts:120](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L120)*

**`description`** Returns a hex string representation of the value

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(`isExtended?`: undefined | false | true): *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[toHuman](_packages_types_src_codec_base_.base.md#tohuman)*

*Defined in [packages/types/src/codec/Base.ts:64](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Base.ts#L64)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Parameters:**

Name | Type |
------ | ------ |
`isExtended?` | undefined &#124; false &#124; true |

**Returns:** *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

___

###  toJSON

▸ **toJSON**(): *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[toJSON](_packages_types_src_codec_base_.base.md#tojson)*

*Defined in [packages/types/src/codec/Base.ts:71](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Base.ts#L71)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

___

###  toRawType

▸ **toRawType**(`isBare?`: undefined | false | true): *string*

*Overrides [Base](_packages_types_src_codec_base_.base.md).[toRawType](_packages_types_src_codec_base_.base.md#torawtype)*

*Defined in [packages/types/src/codec/Option.ts:131](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L131)*

**`description`** Returns the base runtime type name for this instance

**Parameters:**

Name | Type |
------ | ------ |
`isBare?` | undefined &#124; false &#124; true |

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[toString](_packages_types_src_codec_base_.base.md#tostring)*

*Defined in [packages/types/src/codec/Base.ts:78](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Base.ts#L78)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Overrides [Base](_packages_types_src_codec_base_.base.md).[toU8a](_packages_types_src_codec_base_.base.md#tou8a)*

*Defined in [packages/types/src/codec/Option.ts:143](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L143)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value has none of the type-specific prefixes (internal)  |

**Returns:** *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

___

###  unwrap

▸ **unwrap**(): *T*

*Defined in [packages/types/src/codec/Option.ts:161](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L161)*

**`description`** Returns the value that the Option represents (if available), throws if null

**Returns:** *T*

___

###  unwrapOr

▸ **unwrapOr**‹**O**›(`defaultValue`: O): *T | O*

*Defined in [packages/types/src/codec/Option.ts:173](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L173)*

**`description`** Returns the value that the Option represents (if available) or defaultValue if none

**Type parameters:**

▪ **O**

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`defaultValue` | O | The value to return if the option isNone  |

**Returns:** *T | O*

___

###  unwrapOrDefault

▸ **unwrapOrDefault**(): *T*

*Defined in [packages/types/src/codec/Option.ts:183](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L183)*

**`description`** Returns the value that the Option represents (if available) or defaultValue if none

**Returns:** *T*

___

### `Static` with

▸ **with**‹**O**›(`Type`: [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹O› | keyof InterfaceTypes): *[Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹[Option](_packages_types_src_codec_option_.option.md)‹O››*

*Defined in [packages/types/src/codec/Option.ts:62](https://github.com/polkadot-js/api/blob/1922676bd7/packages/types/src/codec/Option.ts#L62)*

**Type parameters:**

▪ **O**: *[Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

**Parameters:**

Name | Type |
------ | ------ |
`Type` | [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹O› &#124; keyof InterfaceTypes |

**Returns:** *[Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹[Option](_packages_types_src_codec_option_.option.md)‹O››*
