[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["generic/AccountId"](../modules/_generic_accountid_.md) › [AccountId](_generic_accountid_.accountid.md)

# Class: AccountId

**`name`** AccountId

**`description`** 
A wrapper around an AccountId/PublicKey representation. Since we are dealing with
underlying PublicKeys (32 bytes in length), we extend from U8aFixed which is
just a Uint8Array wrapper with a fixed length.

## Hierarchy

  ↳ [U8aFixed](_codec_u8afixed_.u8afixed.md)

  ↳ **AccountId**

## Implements

* [IU8a](../interfaces/_types_interfaces_.iu8a.md)

## Indexable

* \[ **index**: *number*\]: number

**`name`** AccountId

**`description`** 
A wrapper around an AccountId/PublicKey representation. Since we are dealing with
underlying PublicKeys (32 bytes in length), we extend from U8aFixed which is
just a Uint8Array wrapper with a fixed length.

## Index

### Constructors

* [constructor](_generic_accountid_.accountid.md#constructor)

### Properties

* [registry](_generic_accountid_.accountid.md#readonly-registry)

### Accessors

* [encodedLength](_generic_accountid_.accountid.md#encodedlength)
* [hash](_generic_accountid_.accountid.md#hash)
* [isEmpty](_generic_accountid_.accountid.md#isempty)
* [length](_generic_accountid_.accountid.md#length)

### Methods

* [bitLength](_generic_accountid_.accountid.md#bitlength)
* [eq](_generic_accountid_.accountid.md#eq)
* [subarray](_generic_accountid_.accountid.md#subarray)
* [toHex](_generic_accountid_.accountid.md#tohex)
* [toHuman](_generic_accountid_.accountid.md#tohuman)
* [toJSON](_generic_accountid_.accountid.md#tojson)
* [toRawType](_generic_accountid_.accountid.md#torawtype)
* [toString](_generic_accountid_.accountid.md#tostring)
* [toU8a](_generic_accountid_.accountid.md#tou8a)
* [encode](_generic_accountid_.accountid.md#static-encode)
* [with](_generic_accountid_.accountid.md#static-with)

## Constructors

###  constructor

\+ **new AccountId**(`registry`: [Registry](../interfaces/_types_registry_.registry.md), `value`: [AnyU8a](../modules/_types_helpers_.md#anyu8a)): *[AccountId](_generic_accountid_.accountid.md)*

*Overrides [U8aFixed](_codec_u8afixed_.u8afixed.md).[constructor](_codec_u8afixed_.u8afixed.md#constructor)*

*Defined in [packages/types/src/generic/AccountId.ts:32](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/generic/AccountId.ts#L32)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`registry` | [Registry](../interfaces/_types_registry_.registry.md) | - |
`value` | [AnyU8a](../modules/_types_helpers_.md#anyu8a) | new Uint8Array() |

**Returns:** *[AccountId](_generic_accountid_.accountid.md)*

## Properties

### `Readonly` registry

• **registry**: *[Registry](../interfaces/_types_registry_.registry.md)*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md).[registry](../interfaces/_types_interfaces_.iu8a.md#readonly-registry)*

*Inherited from [Raw](_codec_raw_.raw.md).[registry](_codec_raw_.raw.md#readonly-registry)*

*Defined in [packages/types/src/codec/Raw.ts:30](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/Raw.ts#L30)*

## Accessors

###  encodedLength

• **get encodedLength**(): *number*

*Inherited from [Raw](_codec_raw_.raw.md).[encodedLength](_codec_raw_.raw.md#encodedlength)*

*Defined in [packages/types/src/codec/Raw.ts:41](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/Raw.ts#L41)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Inherited from [Raw](_codec_raw_.raw.md).[hash](_codec_raw_.raw.md#hash)*

*Defined in [packages/types/src/codec/Raw.ts:48](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/Raw.ts#L48)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Inherited from [Raw](_codec_raw_.raw.md).[isEmpty](_codec_raw_.raw.md#isempty)*

*Defined in [packages/types/src/codec/Raw.ts:55](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/Raw.ts#L55)*

**`description`** Returns true if the type wraps an empty/default all-0 value

**Returns:** *boolean*

___

###  length

• **get length**(): *number*

*Inherited from [Raw](_codec_raw_.raw.md).[length](_codec_raw_.raw.md#length)*

*Overrides [IU8a](../interfaces/_types_interfaces_.iu8a.md).[length](../interfaces/_types_interfaces_.iu8a.md#readonly-length)*

*Defined in [packages/types/src/codec/Raw.ts:62](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/Raw.ts#L62)*

**`description`** The length of the value

**Returns:** *number*

## Methods

###  bitLength

▸ **bitLength**(): *number*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Inherited from [Raw](_codec_raw_.raw.md).[bitLength](_codec_raw_.raw.md#bitlength)*

*Defined in [packages/types/src/codec/Raw.ts:70](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/Raw.ts#L70)*

**`description`** Returns the number of bits in the value

**Returns:** *number*

___

###  eq

▸ **eq**(`other?`: unknown): *boolean*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Overrides [Raw](_codec_raw_.raw.md).[eq](_codec_raw_.raw.md#eq)*

*Defined in [packages/types/src/generic/AccountId.ts:44](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/generic/AccountId.ts#L44)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | unknown |

**Returns:** *boolean*

___

###  subarray

▸ **subarray**(`begin`: number, `end?`: undefined | number): *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

*Inherited from [Raw](_codec_raw_.raw.md).[subarray](_codec_raw_.raw.md#subarray)*

*Overrides [IU8a](../interfaces/_types_interfaces_.iu8a.md).[subarray](../interfaces/_types_interfaces_.iu8a.md#subarray)*

*Defined in [packages/types/src/codec/Raw.ts:91](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/Raw.ts#L91)*

**`description`** Create a new subarray from the actual buffer. This is needed for compat reasons since a new Uint8Array gets returned here

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`begin` | number | The position to start at |
`end?` | undefined &#124; number | The position to end at  |

**Returns:** *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

___

###  toHex

▸ **toHex**(): *string*

*Inherited from [Raw](_codec_raw_.raw.md).[toHex](_codec_raw_.raw.md#tohex)*

*Defined in [packages/types/src/codec/Raw.ts:98](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/Raw.ts#L98)*

**`description`** Returns a hex string representation of the value

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(): *string*

*Overrides [Raw](_codec_raw_.raw.md).[toHuman](_codec_raw_.raw.md#tohuman)*

*Defined in [packages/types/src/generic/AccountId.ts:51](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/generic/AccountId.ts#L51)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Returns:** *string*

___

###  toJSON

▸ **toJSON**(): *string*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Overrides [Raw](_codec_raw_.raw.md).[toJSON](_codec_raw_.raw.md#tojson)*

*Defined in [packages/types/src/generic/AccountId.ts:58](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/generic/AccountId.ts#L58)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *string*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Overrides [U8aFixed](_codec_u8afixed_.u8afixed.md).[toRawType](_codec_u8afixed_.u8afixed.md#torawtype)*

*Defined in [packages/types/src/generic/AccountId.ts:72](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/generic/AccountId.ts#L72)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Overrides [Raw](_codec_raw_.raw.md).[toString](_codec_raw_.raw.md#tostring)*

*Defined in [packages/types/src/generic/AccountId.ts:65](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/generic/AccountId.ts#L65)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

*Inherited from [Raw](_codec_raw_.raw.md).[toU8a](_codec_raw_.raw.md#tou8a)*

*Defined in [packages/types/src/codec/Raw.ts:135](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/Raw.ts#L135)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value has none of the type-specific prefixes (internal)  |

**Returns:** *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

___

### `Static` encode

▸ **encode**(`value`: [Uint8Array](_codec_raw_.raw.md#static-uint8array), `ss58Format?`: undefined | number): *string*

*Defined in [packages/types/src/generic/AccountId.ts:37](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/generic/AccountId.ts#L37)*

**Parameters:**

Name | Type |
------ | ------ |
`value` | [Uint8Array](_codec_raw_.raw.md#static-uint8array) |
`ss58Format?` | undefined &#124; number |

**Returns:** *string*

___

### `Static` with

▸ **with**(`bitLength`: [BitLength](../modules/_codec_u8afixed_.md#bitlength), `typeName?`: undefined | string): *[Constructor](../interfaces/_types_codec_.constructor.md)‹[U8aFixed](_codec_u8afixed_.u8afixed.md)›*

*Inherited from [U8aFixed](_codec_u8afixed_.u8afixed.md).[with](_codec_u8afixed_.u8afixed.md#static-with)*

*Defined in [packages/types/src/codec/U8aFixed.ts:49](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/types/src/codec/U8aFixed.ts#L49)*

**Parameters:**

Name | Type |
------ | ------ |
`bitLength` | [BitLength](../modules/_codec_u8afixed_.md#bitlength) |
`typeName?` | undefined &#124; string |

**Returns:** *[Constructor](../interfaces/_types_codec_.constructor.md)‹[U8aFixed](_codec_u8afixed_.u8afixed.md)›*
