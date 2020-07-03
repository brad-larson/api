[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/types/src/primitive/Text"](../modules/_packages_types_src_primitive_text_.md) › [Text](_packages_types_src_primitive_text_.text.md)

# Class: Text

**`name`** Text

**`description`** 
This is a string wrapper, along with the length. It is used both for strings as well
as items such as documentation. It simply extends the standard JS `String` built-in
object, inheriting all methods exposed from `String`.

## Hierarchy

* [String](_packages_types_src_primitive_text_.text.md#static-string)

  ↳ **Text**

  ↳ [Type](_packages_types_src_primitive_type_.type.md)

## Implements

* [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)

## Indexable

* \[ **index**: *number*\]: string

**`name`** Text

**`description`** 
This is a string wrapper, along with the length. It is used both for strings as well
as items such as documentation. It simply extends the standard JS `String` built-in
object, inheriting all methods exposed from `String`.

## Index

### Constructors

* [constructor](_packages_types_src_primitive_text_.text.md#constructor)

### Properties

* [registry](_packages_types_src_primitive_text_.text.md#readonly-registry)
* [String](_packages_types_src_primitive_text_.text.md#static-string)

### Accessors

* [encodedLength](_packages_types_src_primitive_text_.text.md#encodedlength)
* [hash](_packages_types_src_primitive_text_.text.md#hash)
* [isEmpty](_packages_types_src_primitive_text_.text.md#isempty)
* [length](_packages_types_src_primitive_text_.text.md#length)

### Methods

* [eq](_packages_types_src_primitive_text_.text.md#eq)
* [setOverride](_packages_types_src_primitive_text_.text.md#setoverride)
* [toHex](_packages_types_src_primitive_text_.text.md#tohex)
* [toHuman](_packages_types_src_primitive_text_.text.md#tohuman)
* [toJSON](_packages_types_src_primitive_text_.text.md#tojson)
* [toRawType](_packages_types_src_primitive_text_.text.md#torawtype)
* [toString](_packages_types_src_primitive_text_.text.md#tostring)
* [toU8a](_packages_types_src_primitive_text_.text.md#tou8a)

## Constructors

###  constructor

\+ **new Text**(`registry`: [Registry](../interfaces/_packages_types_src_types_registry_.registry.md), `value`: [Text](_packages_types_src_primitive_text_.text.md) | string | [AnyU8a](../modules/_packages_types_src_types_helpers_.md#anyu8a) | object): *[Text](_packages_types_src_primitive_text_.text.md)*

*Defined in [packages/types/src/primitive/Text.ts:53](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L53)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`registry` | [Registry](../interfaces/_packages_types_src_types_registry_.registry.md) | - |
`value` | [Text](_packages_types_src_primitive_text_.text.md) &#124; string &#124; [AnyU8a](../modules/_packages_types_src_types_helpers_.md#anyu8a) &#124; object | "" |

**Returns:** *[Text](_packages_types_src_primitive_text_.text.md)*

## Properties

### `Readonly` registry

• **registry**: *[Registry](../interfaces/_packages_types_src_types_registry_.registry.md)*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md).[registry](../interfaces/_packages_types_src_types_codec_.codec.md#readonly-registry)*

*Defined in [packages/types/src/primitive/Text.ts:51](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L51)*

___

### `Static` String

▪ **String**: *StringConstructor*

Defined in node_modules/typescript/lib/lib.es5.d.ts:527

Allows manipulation and formatting of text strings and determination and location of substrings within strings.

## Accessors

###  encodedLength

• **get encodedLength**(): *number*

*Defined in [packages/types/src/primitive/Text.ts:64](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L64)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Defined in [packages/types/src/primitive/Text.ts:71](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L71)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Defined in [packages/types/src/primitive/Text.ts:78](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L78)*

**`description`** Checks if the value is an empty value

**Returns:** *boolean*

___

###  length

• **get length**(): *number*

*Overrides [RegistryMetadataText](../interfaces/_packages_types_src_types_registry_.registrymetadatatext.md).[length](../interfaces/_packages_types_src_types_registry_.registrymetadatatext.md#readonly-length)*

*Defined in [packages/types/src/primitive/Text.ts:85](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L85)*

**`description`** The length of the value

**Returns:** *number*

## Methods

###  eq

▸ **eq**(`other?`: unknown): *boolean*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/primitive/Text.ts:93](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L93)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | unknown |

**Returns:** *boolean*

___

###  setOverride

▸ **setOverride**(`override`: string): *void*

*Defined in [packages/types/src/primitive/Text.ts:102](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L102)*

**`description`** Set an override value for this

**Parameters:**

Name | Type |
------ | ------ |
`override` | string |

**Returns:** *void*

___

###  toHex

▸ **toHex**(): *string*

*Defined in [packages/types/src/primitive/Text.ts:109](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L109)*

**`description`** Returns a hex string representation of the value

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(): *string*

*Defined in [packages/types/src/primitive/Text.ts:118](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L118)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Returns:** *string*

___

###  toJSON

▸ **toJSON**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/primitive/Text.ts:125](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L125)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *string*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Defined in [packages/types/src/primitive/Text.ts:132](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L132)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [Codec](../interfaces/_packages_types_src_types_codec_.codec.md)*

*Overrides [RegistryMetadataText](../interfaces/_packages_types_src_types_registry_.registrymetadatatext.md).[toString](../interfaces/_packages_types_src_types_registry_.registrymetadatatext.md#tostring)*

*Defined in [packages/types/src/primitive/Text.ts:139](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L139)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Defined in [packages/types/src/primitive/Text.ts:147](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/types/src/primitive/Text.ts#L147)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value has none of the type-specific prefixes (internal)  |

**Returns:** *[Uint8Array](_packages_types_src_codec_raw_.raw.md#static-uint8array)*
