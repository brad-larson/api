[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/types/src/generic/Vote"](../modules/_packages_types_src_generic_vote_.md) › [Vote](_packages_types_src_generic_vote_.vote.md)

# Class: Vote

**`name`** Vote

**`description`** 
A number of lock periods, plus a vote, one way or the other.

## Hierarchy

  ↳ [U8aFixed](_packages_types_src_codec_u8afixed_.u8afixed.md)

  ↳ **Vote**

## Implements

* [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md)

## Indexable

* \[ **index**: *number*\]: number

**`name`** Vote

**`description`** 
A number of lock periods, plus a vote, one way or the other.

## Index

### Constructors

* [constructor](_packages_types_src_generic_vote_.vote.md#constructor)

### Properties

* [registry](_packages_types_src_generic_vote_.vote.md#readonly-registry)

### Accessors

* [conviction](_packages_types_src_generic_vote_.vote.md#conviction)
* [encodedLength](_packages_types_src_generic_vote_.vote.md#encodedlength)
* [hash](_packages_types_src_generic_vote_.vote.md#hash)
* [isAye](_packages_types_src_generic_vote_.vote.md#isaye)
* [isEmpty](_packages_types_src_generic_vote_.vote.md#isempty)
* [isNay](_packages_types_src_generic_vote_.vote.md#isnay)
* [length](_packages_types_src_generic_vote_.vote.md#length)

### Methods

* [bitLength](_packages_types_src_generic_vote_.vote.md#bitlength)
* [eq](_packages_types_src_generic_vote_.vote.md#eq)
* [subarray](_packages_types_src_generic_vote_.vote.md#subarray)
* [toHex](_packages_types_src_generic_vote_.vote.md#tohex)
* [toHuman](_packages_types_src_generic_vote_.vote.md#tohuman)
* [toJSON](_packages_types_src_generic_vote_.vote.md#tojson)
* [toRawType](_packages_types_src_generic_vote_.vote.md#torawtype)
* [toString](_packages_types_src_generic_vote_.vote.md#tostring)
* [toU8a](_packages_types_src_generic_vote_.vote.md#tou8a)
* [with](_packages_types_src_generic_vote_.vote.md#static-with)

## Constructors

###  constructor

\+ **new Vote**(`registry`: [Registry](../interfaces/_packages_types_src_types_registry_.registry.md), `value?`: InputTypes): *[Vote](_packages_types_src_generic_vote_.vote.md)*

*Overrides [U8aFixed](_packages_types_src_codec_u8afixed_.u8afixed.md).[constructor](_packages_types_src_codec_u8afixed_.u8afixed.md#constructor)*

*Defined in [packages/types/src/generic/Vote.ts:64](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/generic/Vote.ts#L64)*

**Parameters:**

Name | Type |
------ | ------ |
`registry` | [Registry](../interfaces/_packages_types_src_types_registry_.registry.md) |
`value?` | InputTypes |

**Returns:** *[Vote](_packages_types_src_generic_vote_.vote.md)*

## Properties

### `Readonly` registry

• **registry**: *[Registry](../interfaces/_packages_types_src_types_registry_.registry.md)*

*Implementation of [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md).[registry](../interfaces/_packages_types_src_types_interfaces_.iu8a.md#readonly-registry)*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[registry](_packages_types_src_codec_raw_.raw.md#readonly-registry)*

*Defined in [packages/types/src/codec/Raw.ts:30](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L30)*

## Accessors

###  conviction

• **get conviction**(): *Conviction*

*Defined in [packages/types/src/generic/Vote.ts:81](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/generic/Vote.ts#L81)*

**`description`** returns a V2 conviction

**Returns:** *Conviction*

___

###  encodedLength

• **get encodedLength**(): *number*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[encodedLength](_packages_types_src_codec_raw_.raw.md#encodedlength)*

*Defined in [packages/types/src/codec/Raw.ts:41](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L41)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[hash](_packages_types_src_codec_raw_.raw.md#hash)*

*Defined in [packages/types/src/codec/Raw.ts:48](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L48)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isAye

• **get isAye**(): *boolean*

*Defined in [packages/types/src/generic/Vote.ts:88](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/generic/Vote.ts#L88)*

**`description`** true if the wrapped value is a positive vote

**Returns:** *boolean*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[isEmpty](_packages_types_src_codec_raw_.raw.md#isempty)*

*Defined in [packages/types/src/codec/Raw.ts:55](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L55)*

**`description`** Returns true if the type wraps an empty/default all-0 value

**Returns:** *boolean*

___

###  isNay

• **get isNay**(): *boolean*

*Defined in [packages/types/src/generic/Vote.ts:95](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/generic/Vote.ts#L95)*

**`description`** true if the wrapped value is a negative vote

**Returns:** *boolean*

___

###  length

• **get length**(): *number*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[length](_packages_types_src_codec_raw_.raw.md#length)*

*Overrides [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md).[length](../interfaces/_packages_types_src_types_interfaces_.iu8a.md#readonly-length)*

*Defined in [packages/types/src/codec/Raw.ts:62](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L62)*

**`description`** The length of the value

**Returns:** *number*

## Methods

###  bitLength

▸ **bitLength**(): *number*

*Implementation of [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md)*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[bitLength](_packages_types_src_codec_raw_.raw.md#bitlength)*

*Defined in [packages/types/src/codec/Raw.ts:70](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L70)*

**`description`** Returns the number of bits in the value

**Returns:** *number*

___

###  eq

▸ **eq**(`other?`: unknown): *boolean*

*Implementation of [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md)*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[eq](_packages_types_src_codec_raw_.raw.md#eq)*

*Defined in [packages/types/src/codec/Raw.ts:77](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L77)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | unknown |

**Returns:** *boolean*

___

###  subarray

▸ **subarray**(`begin`: number, `end?`: undefined | number): *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[subarray](_packages_types_src_codec_raw_.raw.md#subarray)*

*Overrides [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md).[subarray](../interfaces/_packages_types_src_types_interfaces_.iu8a.md#subarray)*

*Defined in [packages/types/src/codec/Raw.ts:91](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L91)*

**`description`** Create a new subarray from the actual buffer. This is needed for compat reasons since a new Uint8Array gets returned here

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`begin` | number | The position to start at |
`end?` | undefined &#124; number | The position to end at  |

**Returns:** *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

___

###  toHex

▸ **toHex**(): *string*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[toHex](_packages_types_src_codec_raw_.raw.md#tohex)*

*Defined in [packages/types/src/codec/Raw.ts:98](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L98)*

**`description`** Returns a hex string representation of the value

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(`isExpanded?`: undefined | false | true): *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

*Implementation of [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md)*

*Overrides [Raw](_packages_types_src_codec_raw_.raw.md).[toHuman](_packages_types_src_codec_raw_.raw.md#tohuman)*

*Defined in [packages/types/src/generic/Vote.ts:102](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/generic/Vote.ts#L102)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Parameters:**

Name | Type |
------ | ------ |
`isExpanded?` | undefined &#124; false &#124; true |

**Returns:** *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

___

###  toJSON

▸ **toJSON**(): *string*

*Implementation of [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md)*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[toJSON](_packages_types_src_codec_raw_.raw.md#tojson)*

*Defined in [packages/types/src/codec/Raw.ts:112](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L112)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *string*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md)*

*Overrides [U8aFixed](_packages_types_src_codec_u8afixed_.u8afixed.md).[toRawType](_packages_types_src_codec_u8afixed_.u8afixed.md#torawtype)*

*Defined in [packages/types/src/generic/Vote.ts:112](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/generic/Vote.ts#L112)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md)*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[toString](_packages_types_src_codec_raw_.raw.md#tostring)*

*Overrides [IU8a](../interfaces/_packages_types_src_types_interfaces_.iu8a.md).[toString](../interfaces/_packages_types_src_types_interfaces_.iu8a.md#tostring)*

*Defined in [packages/types/src/codec/Raw.ts:126](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L126)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Inherited from [Raw](_packages_types_src_codec_raw_.raw.md).[toU8a](_packages_types_src_codec_raw_.raw.md#tou8a)*

*Defined in [packages/types/src/codec/Raw.ts:135](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/Raw.ts#L135)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value has none of the type-specific prefixes (internal)  |

**Returns:** *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

___

### `Static` with

▸ **with**(`bitLength`: [BitLength](../modules/_packages_types_src_codec_u8afixed_.md#bitlength), `typeName?`: undefined | string): *[Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹[U8aFixed](_packages_types_src_codec_u8afixed_.u8afixed.md)›*

*Inherited from [U8aFixed](_packages_types_src_codec_u8afixed_.u8afixed.md).[with](_packages_types_src_codec_u8afixed_.u8afixed.md#static-with)*

*Defined in [packages/types/src/codec/U8aFixed.ts:50](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/codec/U8aFixed.ts#L50)*

**Parameters:**

Name | Type |
------ | ------ |
`bitLength` | [BitLength](../modules/_packages_types_src_codec_u8afixed_.md#bitlength) |
`typeName?` | undefined &#124; string |

**Returns:** *[Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹[U8aFixed](_packages_types_src_codec_u8afixed_.u8afixed.md)›*
