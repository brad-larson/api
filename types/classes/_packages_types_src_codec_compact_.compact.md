[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/types/src/codec/Compact"](../modules/_packages_types_src_codec_compact_.md) › [Compact](_packages_types_src_codec_compact_.compact.md)

# Class: Compact ‹**T**›

**`name`** Compact

**`description`** 
A compact length-encoding codec wrapper. It performs the same function as Length, however
differs in that it uses a variable number of bytes to do the actual encoding. This is mostly
used by other types to add length-prefixed encoding, or in the case of wrapped types, taking
a number and making the compact representation thereof

## Type parameters

▪ **T**: *[CompactEncodable](../interfaces/_packages_types_src_codec_compact_.compactencodable.md)*

## Hierarchy

* [Base](_packages_types_src_codec_base_.base.md)‹T›

  ↳ **Compact**

## Implements

* [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)
* [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)‹T›

## Index

### Constructors

* [constructor](_packages_types_src_codec_compact_.compact.md#constructor)

### Properties

* [registry](_packages_types_src_codec_compact_.compact.md#readonly-registry)
* [addLengthPrefix](_packages_types_src_codec_compact_.compact.md#static-addlengthprefix)
* [decodeU8a](_packages_types_src_codec_compact_.compact.md#static-decodeu8a)
* [encodeU8a](_packages_types_src_codec_compact_.compact.md#static-encodeu8a)

### Accessors

* [encodedLength](_packages_types_src_codec_compact_.compact.md#encodedlength)
* [hash](_packages_types_src_codec_compact_.compact.md#hash)
* [isEmpty](_packages_types_src_codec_compact_.compact.md#isempty)

### Methods

* [bitLength](_packages_types_src_codec_compact_.compact.md#bitlength)
* [eq](_packages_types_src_codec_compact_.compact.md#eq)
* [toBn](_packages_types_src_codec_compact_.compact.md#tobn)
* [toHex](_packages_types_src_codec_compact_.compact.md#tohex)
* [toHuman](_packages_types_src_codec_compact_.compact.md#tohuman)
* [toJSON](_packages_types_src_codec_compact_.compact.md#tojson)
* [toNumber](_packages_types_src_codec_compact_.compact.md#tonumber)
* [toRawType](_packages_types_src_codec_compact_.compact.md#torawtype)
* [toString](_packages_types_src_codec_compact_.compact.md#tostring)
* [toU8a](_packages_types_src_codec_compact_.compact.md#tou8a)
* [unwrap](_packages_types_src_codec_compact_.compact.md#unwrap)
* [stripLengthPrefix](_packages_types_src_codec_compact_.compact.md#static-striplengthprefix)
* [with](_packages_types_src_codec_compact_.compact.md#static-with)

## Constructors

###  constructor

\+ **new Compact**(`registry`: [Registry](../interfaces/_packages_types_src_types_registry_.registry.md), `Type`: [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹T› | keyof InterfaceTypes, `value`: [Compact](_packages_types_src_codec_compact_.compact.md)‹T› | [AnyNumber](../modules/_packages_types_src_types_helpers_.md#anynumber)): *[Compact](_packages_types_src_codec_compact_.compact.md)*

*Overrides void*

*Defined in [packages/types/src/codec/Compact.ts:30](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L30)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`registry` | [Registry](../interfaces/_packages_types_src_types_registry_.registry.md) | - |
`Type` | [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹T› &#124; keyof InterfaceTypes | - |
`value` | [Compact](_packages_types_src_codec_compact_.compact.md)‹T› &#124; [AnyNumber](../modules/_packages_types_src_types_helpers_.md#anynumber) | 0 |

**Returns:** *[Compact](_packages_types_src_codec_compact_.compact.md)*

## Properties

### `Readonly` registry

• **registry**: *[Registry](../interfaces/_packages_types_src_types_registry_.registry.md)*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md).[registry](../interfaces/_packages_types_src_types_interfaces_.icompact.md#readonly-registry)*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[registry](_packages_types_src_codec_base_.base.md#readonly-registry)*

*Defined in [packages/types/src/codec/Base.ts:17](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Base.ts#L17)*

___

### `Static` addLengthPrefix

▪ **addLengthPrefix**: *compactAddLength* = compactAddLength

*Defined in [packages/types/src/codec/Compact.ts:55](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L55)*

Prepend a Uint8Array with its compact length.

**`param`** The Uint8Array to be prefixed

___

### `Static` decodeU8a

▪ **decodeU8a**: *compactFromU8a* = compactFromU8a

*Defined in [packages/types/src/codec/Compact.ts:57](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L57)*

___

### `Static` encodeU8a

▪ **encodeU8a**: *compactToU8a* = compactToU8a

*Defined in [packages/types/src/codec/Compact.ts:59](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L59)*

## Accessors

###  encodedLength

• **get encodedLength**(): *number*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[encodedLength](_packages_types_src_codec_base_.base.md#encodedlength)*

*Defined in [packages/types/src/codec/Base.ts:29](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Base.ts#L29)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[hash](_packages_types_src_codec_base_.base.md#hash)*

*Defined in [packages/types/src/codec/Base.ts:36](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Base.ts#L36)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[isEmpty](_packages_types_src_codec_base_.base.md#isempty)*

*Defined in [packages/types/src/codec/Base.ts:43](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Base.ts#L43)*

**`description`** Checks if the value is an empty value

**Returns:** *boolean*

## Methods

###  bitLength

▸ **bitLength**(): *number*

*Defined in [packages/types/src/codec/Compact.ts:83](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L83)*

**`description`** Returns the number of bits in the value

**Returns:** *number*

___

###  eq

▸ **eq**(`other?`: unknown): *boolean*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)*

*Overrides [Base](_packages_types_src_codec_base_.base.md).[eq](_packages_types_src_codec_base_.base.md#eq)*

*Defined in [packages/types/src/codec/Compact.ts:90](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L90)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | unknown |

**Returns:** *boolean*

___

###  toBn

▸ **toBn**(): *BN*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)*

*Defined in [packages/types/src/codec/Compact.ts:101](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L101)*

**`description`** Returns the BN representation of the number

**Returns:** *BN*

___

###  toHex

▸ **toHex**(`isLe?`: undefined | false | true): *string*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[toHex](_packages_types_src_codec_base_.base.md#tohex)*

*Defined in [packages/types/src/codec/Base.ts:57](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Base.ts#L57)*

**`description`** Returns a hex string representation of the value. isLe returns a LE (number-only) representation

**Parameters:**

Name | Type |
------ | ------ |
`isLe?` | undefined &#124; false &#124; true |

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(`isExtended?`: undefined | false | true): *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[toHuman](_packages_types_src_codec_base_.base.md#tohuman)*

*Defined in [packages/types/src/codec/Base.ts:64](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Base.ts#L64)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Parameters:**

Name | Type |
------ | ------ |
`isExtended?` | undefined &#124; false &#124; true |

**Returns:** *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

___

###  toJSON

▸ **toJSON**(): *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[toJSON](_packages_types_src_codec_base_.base.md#tojson)*

*Defined in [packages/types/src/codec/Base.ts:71](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Base.ts#L71)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *[AnyJson](../modules/_packages_types_src_types_helpers_.md#anyjson)*

___

###  toNumber

▸ **toNumber**(): *number*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)*

*Defined in [packages/types/src/codec/Compact.ts:108](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L108)*

**`description`** Returns the number representation for the value

**Returns:** *number*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)*

*Overrides [Base](_packages_types_src_codec_base_.base.md).[toRawType](_packages_types_src_codec_base_.base.md#torawtype)*

*Defined in [packages/types/src/codec/Compact.ts:115](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L115)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)*

*Inherited from [Base](_packages_types_src_codec_base_.base.md).[toString](_packages_types_src_codec_base_.base.md#tostring)*

*Defined in [packages/types/src/codec/Base.ts:78](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Base.ts#L78)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Overrides [Base](_packages_types_src_codec_base_.base.md).[toU8a](_packages_types_src_codec_base_.base.md#tou8a)*

*Defined in [packages/types/src/codec/Compact.ts:124](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L124)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value has none of the type-specific prefixes (internal)  |

**Returns:** *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

___

###  unwrap

▸ **unwrap**(): *T*

*Implementation of [ICompact](../interfaces/_packages_types_src_types_interfaces_.icompact.md)*

*Defined in [packages/types/src/codec/Compact.ts:131](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L131)*

**`description`** Returns the embedded [UInt](_packages_types_src_codec_uint_.uint.md) or [Moment](../interfaces/_packages_types_src_augment_registry_._registry_.interfacetypes.md#moment) value

**Returns:** *T*

___

### `Static` stripLengthPrefix

▸ **stripLengthPrefix**(`u8a`: [Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array), `bitLength`: [UIntBitLength](../modules/_packages_types_src_codec_abstractint_.md#uintbitlength)): *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Defined in [packages/types/src/codec/Compact.ts:61](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L61)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`u8a` | [Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array) | - |
`bitLength` | [UIntBitLength](../modules/_packages_types_src_codec_abstractint_.md#uintbitlength) | DEFAULT_BITLENGTH |

**Returns:** *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

___

### `Static` with

▸ **with**‹**T**›(`Type`: [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹T› | keyof InterfaceTypes): *[Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹[Compact](_packages_types_src_codec_compact_.compact.md)‹T››*

*Defined in [packages/types/src/codec/Compact.ts:42](https://github.com/polkadot-js/api/blob/bbc30ec9dc/packages/types/src/codec/Compact.ts#L42)*

**Type parameters:**

▪ **T**: *[CompactEncodable](../interfaces/_packages_types_src_codec_compact_.compactencodable.md)*

**Parameters:**

Name | Type |
------ | ------ |
`Type` | [Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹T› &#124; keyof InterfaceTypes |

**Returns:** *[Constructor](../interfaces/_packages_types_src_types_codec_.constructor.md)‹[Compact](_packages_types_src_codec_compact_.compact.md)‹T››*
