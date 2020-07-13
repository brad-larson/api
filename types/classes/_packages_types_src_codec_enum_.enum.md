[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/types/src/codec/Enum"](../modules/_packages_types_src_codec_enum_.md) › [Enum](_packages_types_src_codec_enum_.enum.md)

# Class: Enum

**`name`** Enum

**`description`** 
This implements an enum, that based on the value wraps a different type. It is effectively
an extension to enum where the value type is determined by the actual index.

## Hierarchy

* **Enum**

  ↳ [ExtrinsicEra](_packages_types_src_extrinsic_extrinsicera_.extrinsicera.md)

  ↳ [Result](_packages_types_src_codec_result_.result.md)

  ↳ [Data](_packages_types_src_primitive_data_.data.md)

## Implements

* [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)

## Index

### Constructors

* [constructor](_packages_types_src_codec_enum_.enum.md#constructor)

### Properties

* [registry](_packages_types_src_codec_enum_.enum.md#readonly-registry)

### Accessors

* [defEntries](_packages_types_src_codec_enum_.enum.md#defentries)
* [defKeys](_packages_types_src_codec_enum_.enum.md#defkeys)
* [encodedLength](_packages_types_src_codec_enum_.enum.md#encodedlength)
* [hash](_packages_types_src_codec_enum_.enum.md#hash)
* [index](_packages_types_src_codec_enum_.enum.md#index)
* [isBasic](_packages_types_src_codec_enum_.enum.md#isbasic)
* [isEmpty](_packages_types_src_codec_enum_.enum.md#isempty)
* [isNone](_packages_types_src_codec_enum_.enum.md#isnone)
* [isNull](_packages_types_src_codec_enum_.enum.md#isnull)
* [type](_packages_types_src_codec_enum_.enum.md#type)
* [value](_packages_types_src_codec_enum_.enum.md#value)

### Methods

* [eq](_packages_types_src_codec_enum_.enum.md#eq)
* [toHex](_packages_types_src_codec_enum_.enum.md#tohex)
* [toHuman](_packages_types_src_codec_enum_.enum.md#tohuman)
* [toJSON](_packages_types_src_codec_enum_.enum.md#tojson)
* [toNumber](_packages_types_src_codec_enum_.enum.md#tonumber)
* [toRawType](_packages_types_src_codec_enum_.enum.md#torawtype)
* [toString](_packages_types_src_codec_enum_.enum.md#tostring)
* [toU8a](_packages_types_src_codec_enum_.enum.md#tou8a)
* [with](_packages_types_src_codec_enum_.enum.md#static-with)

## Constructors

###  constructor

\+ **new Enum**(`registry`: [Registry](../interfaces/_packages_types_src_types_registry_.registry.md), `def`: Record‹string, keyof InterfaceTypes | [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)› | string[], `value?`: unknown, `index?`: undefined | number): *[Enum](_packages_types_src_codec_enum_.enum.md)*

*Defined in [packages/types/src/codec/Enum.ts:130](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L130)*

**Parameters:**

Name | Type |
------ | ------ |
`registry` | [Registry](../interfaces/_packages_types_src_types_registry_.registry.md) |
`def` | Record‹string, keyof InterfaceTypes &#124; [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)› &#124; string[] |
`value?` | unknown |
`index?` | undefined &#124; number |

**Returns:** *[Enum](_packages_types_src_codec_enum_.enum.md)*

## Properties

### `Readonly` registry

• **registry**: *[Registry](../interfaces/_packages_types_src_types_registry_.registry.md)*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md).[registry](../interfaces/_packages_types_src_types_codec_.codec.md#readonly-registry)*

*Defined in [packages/types/src/codec/Enum.ts:120](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L120)*

## Accessors

###  defEntries

• **get defEntries**(): *string[]*

*Defined in [packages/types/src/codec/Enum.ts:232](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L232)*

**`description`** The available keys for this enum

**Returns:** *string[]*

___

###  defKeys

• **get defKeys**(): *string[]*

*Defined in [packages/types/src/codec/Enum.ts:239](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L239)*

**`description`** The available keys for this enum

**Returns:** *string[]*

___

###  encodedLength

• **get encodedLength**(): *number*

*Defined in [packages/types/src/codec/Enum.ts:183](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L183)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Defined in [packages/types/src/codec/Enum.ts:190](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L190)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  index

• **get index**(): *number*

*Defined in [packages/types/src/codec/Enum.ts:197](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L197)*

**`description`** The index of the metadata value

**Returns:** *number*

___

###  isBasic

• **get isBasic**(): *boolean*

*Defined in [packages/types/src/codec/Enum.ts:204](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L204)*

**`description`** true if this is a basic enum (no values)

**Returns:** *boolean*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Defined in [packages/types/src/codec/Enum.ts:211](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L211)*

**`description`** Checks if the value is an empty value

**Returns:** *boolean*

___

###  isNone

• **get isNone**(): *boolean*

*Defined in [packages/types/src/codec/Enum.ts:218](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L218)*

**`description`** Checks if the Enum points to a [Null](_packages_types_src_primitive_null_.null.md) type

**Returns:** *boolean*

___

###  isNull

• **get isNull**(): *boolean*

*Defined in [packages/types/src/codec/Enum.ts:225](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L225)*

**`description`** Checks if the Enum points to a [Null](_packages_types_src_primitive_null_.null.md) type (deprecated, use isNone)

**Returns:** *boolean*

___

###  type

• **get type**(): *string*

*Defined in [packages/types/src/codec/Enum.ts:246](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L246)*

**`description`** The name of the type this enum value represents

**Returns:** *string*

___

###  value

• **get value**(): *[Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/Enum.ts:253](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L253)*

**`description`** The value of the enum

**Returns:** *[Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

## Methods

###  eq

▸ **eq**(`other?`: unknown): *boolean*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/Enum.ts:260](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L260)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | unknown |

**Returns:** *boolean*

___

###  toHex

▸ **toHex**(): *string*

*Defined in [packages/types/src/codec/Enum.ts:283](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L283)*

**`description`** Returns a hex string representation of the value

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(`isExtended?`: undefined | false | true): *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/Enum.ts:290](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L290)*

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

*Defined in [packages/types/src/codec/Enum.ts:299](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L299)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

___

###  toNumber

▸ **toNumber**(): *number*

*Defined in [packages/types/src/codec/Enum.ts:308](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L308)*

**`description`** Returns the number representation for the value

**Returns:** *number*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/Enum.ts:324](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L324)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/codec/Enum.ts:331](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L331)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Defined in [packages/types/src/codec/Enum.ts:341](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L341)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value has none of the type-specific prefixes (internal)  |

**Returns:** *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

___

### `Static` with

▸ **with**(`Types`: Record‹string, keyof InterfaceTypes | [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)› | string[]): *[EnumConstructor](../interfaces/_packages_types_src_codec_enum_.enumconstructor.md)‹[Enum](_packages_types_src_codec_enum_.enum.md)›*

*Defined in [packages/types/src/codec/Enum.ts:144](https://github.com/polkadot-js/api/blob/36232c0289/packages/types/src/codec/Enum.ts#L144)*

**Parameters:**

Name | Type |
------ | ------ |
`Types` | Record‹string, keyof InterfaceTypes &#124; [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)› &#124; string[] |

**Returns:** *[EnumConstructor](../interfaces/_packages_types_src_codec_enum_.enumconstructor.md)‹[Enum](_packages_types_src_codec_enum_.enum.md)›*
