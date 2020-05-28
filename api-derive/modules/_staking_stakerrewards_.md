[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["staking/stakerRewards"](_staking_stakerrewards_.md)

# Module: "staking/stakerRewards"

## Index

### Functions

* [_stakerRewards](_staking_stakerrewards_.md#_stakerrewards)
* [_stakerRewardsEras](_staking_stakerrewards_.md#_stakerrewardseras)
* [stakerRewards](_staking_stakerrewards_.md#stakerrewards)
* [stakerRewardsMulti](_staking_stakerrewards_.md#stakerrewardsmulti)

## Functions

###  _stakerRewards

▸ **_stakerRewards**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/stakerRewards.ts:172](https://github.com/polkadot-js/api/blob/b174864804/packages/api-derive/src/staking/stakerRewards.ts#L172)*

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`accountId`: Uint8Array | string, `eras`: EraIndex[], `withActive`: boolean): *Observable‹DeriveStakerReward[]›*

**Parameters:**

Name | Type |
------ | ------ |
`accountId` | Uint8Array &#124; string |
`eras` | EraIndex[] |
`withActive` | boolean |

___

###  _stakerRewardsEras

▸ **_stakerRewardsEras**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/stakerRewards.ts:159](https://github.com/polkadot-js/api/blob/b174864804/packages/api-derive/src/staking/stakerRewards.ts#L159)*

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`eras`: EraIndex[], `withActive`: boolean): *Observable‹ErasResult›*

**Parameters:**

Name | Type |
------ | ------ |
`eras` | EraIndex[] |
`withActive` | boolean |

___

###  stakerRewards

▸ **stakerRewards**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/stakerRewards.ts:192](https://github.com/polkadot-js/api/blob/b174864804/packages/api-derive/src/staking/stakerRewards.ts#L192)*

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`accountId`: Uint8Array | string, `withActive?`: undefined | false | true): *Observable‹DeriveStakerReward[]›*

**Parameters:**

Name | Type |
------ | ------ |
`accountId` | Uint8Array &#124; string |
`withActive?` | undefined &#124; false &#124; true |

___

###  stakerRewardsMulti

▸ **stakerRewardsMulti**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/stakerRewards.ts:200](https://github.com/polkadot-js/api/blob/b174864804/packages/api-derive/src/staking/stakerRewards.ts#L200)*

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`accountIds`: string | Uint8Array‹›[], `withActive?`: undefined | false | true): *Observable‹DeriveStakerReward[][]›*

**Parameters:**

Name | Type |
------ | ------ |
`accountIds` | string &#124; Uint8Array‹›[] |
`withActive?` | undefined &#124; false &#124; true |
