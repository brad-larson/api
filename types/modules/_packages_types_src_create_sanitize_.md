[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/types/src/create/sanitize"](_packages_types_src_create_sanitize_.md)

# Module: "packages/types/src/create/sanitize"

## Index

### Functions

* [alias](_packages_types_src_create_sanitize_.md#alias)
* [cleanupCompact](_packages_types_src_create_sanitize_.md#cleanupcompact)
* [findClosing](_packages_types_src_create_sanitize_.md#findclosing)
* [flattenSingleTuple](_packages_types_src_create_sanitize_.md#flattensingletuple)
* [removeColons](_packages_types_src_create_sanitize_.md#removecolons)
* [removeGenerics](_packages_types_src_create_sanitize_.md#removegenerics)
* [removePairOf](_packages_types_src_create_sanitize_.md#removepairof)
* [removeTraits](_packages_types_src_create_sanitize_.md#removetraits)
* [removeWrap](_packages_types_src_create_sanitize_.md#removewrap)
* [sanitize](_packages_types_src_create_sanitize_.md#sanitize)

## Functions

###  alias

▸ **alias**(`src`: string[], `dest`: string, `withChecks`: boolean): *Mapper*

*Defined in [packages/types/src/create/sanitize.ts:64](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L64)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`src` | string[] | - |
`dest` | string | - |
`withChecks` | boolean | true |

**Returns:** *Mapper*

___

###  cleanupCompact

▸ **cleanupCompact**(): *Mapper*

*Defined in [packages/types/src/create/sanitize.ts:79](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L79)*

**Returns:** *Mapper*

___

###  findClosing

▸ **findClosing**(`value`: string, `start`: number): *number*

*Defined in [packages/types/src/create/sanitize.ts:46](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L46)*

**Parameters:**

Name | Type |
------ | ------ |
`value` | string |
`start` | number |

**Returns:** *number*

___

###  flattenSingleTuple

▸ **flattenSingleTuple**(): *Mapper*

*Defined in [packages/types/src/create/sanitize.ts:97](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L97)*

**Returns:** *Mapper*

___

###  removeColons

▸ **removeColons**(): *Mapper*

*Defined in [packages/types/src/create/sanitize.ts:103](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L103)*

**Returns:** *Mapper*

___

###  removeGenerics

▸ **removeGenerics**(): *Mapper*

*Defined in [packages/types/src/create/sanitize.ts:131](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L131)*

**Returns:** *Mapper*

___

###  removePairOf

▸ **removePairOf**(): *Mapper*

*Defined in [packages/types/src/create/sanitize.ts:159](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L159)*

**Returns:** *Mapper*

___

###  removeTraits

▸ **removeTraits**(): *Mapper*

*Defined in [packages/types/src/create/sanitize.ts:176](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L176)*

**Returns:** *Mapper*

___

###  removeWrap

▸ **removeWrap**(`_check`: string): *Mapper*

*Defined in [packages/types/src/create/sanitize.ts:195](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L195)*

**Parameters:**

Name | Type |
------ | ------ |
`_check` | string |

**Returns:** *Mapper*

___

###  sanitize

▸ **sanitize**(`value`: string, `options?`: SanitizeOptions): *string*

*Defined in [packages/types/src/create/sanitize.ts:216](https://github.com/polkadot-js/api/blob/023c7588e5/packages/types/src/create/sanitize.ts#L216)*

**Parameters:**

Name | Type |
------ | ------ |
`value` | string |
`options?` | SanitizeOptions |

**Returns:** *string*
