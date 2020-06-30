[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/api-derive/src/staking/erasRewards"](_packages_api_derive_src_staking_erasrewards_.md)

# Module: "packages/api-derive/src/staking/erasRewards"

## Index

### Functions

* [_erasRewards](_packages_api_derive_src_staking_erasrewards_.md#_erasrewards)
* [erasRewards](_packages_api_derive_src_staking_erasrewards_.md#erasrewards)

## Functions

###  _erasRewards

▸ **_erasRewards**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/erasRewards.ts:24](https://github.com/polkadot-js/api/blob/023c7588e5/packages/api-derive/src/staking/erasRewards.ts#L24)*

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`eras`: EraIndex[], `withActive`: boolean): *Observable‹DeriveEraRewards[]›*

**Parameters:**

Name | Type |
------ | ------ |
`eras` | EraIndex[] |
`withActive` | boolean |

___

###  erasRewards

▸ **erasRewards**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/erasRewards.ts:56](https://github.com/polkadot-js/api/blob/023c7588e5/packages/api-derive/src/staking/erasRewards.ts#L56)*

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`withActive?`: undefined | false | true): *Observable‹DeriveEraRewards[]›*

**Parameters:**

Name | Type |
------ | ------ |
`withActive?` | undefined &#124; false &#124; true |
