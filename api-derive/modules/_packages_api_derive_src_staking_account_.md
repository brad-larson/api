[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/api-derive/src/staking/account"](_packages_api_derive_src_staking_account_.md)

# Module: "packages/api-derive/src/staking/account"

## Index

### Functions

* [account](_packages_api_derive_src_staking_account_.md#account)
* [accounts](_packages_api_derive_src_staking_account_.md#accounts)

## Functions

###  account

▸ **account**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/account.ts:93](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/api-derive/src/staking/account.ts#L93)*

**`description`** From a stash, retrieve the controllerId and fill in all the relevant staking details

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`accountId`: Uint8Array | string): *Observable‹DeriveStakingAccount›*

**Parameters:**

Name | Type |
------ | ------ |
`accountId` | Uint8Array &#124; string |

___

###  accounts

▸ **accounts**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/account.ts:78](https://github.com/polkadot-js/api/blob/eed5e23e65/packages/api-derive/src/staking/account.ts#L78)*

**`description`** From a list of stashes, fill in all the relevant staking details

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`accountIds`: string | Uint8Array‹›[]): *Observable‹DeriveStakingAccount[]›*

**Parameters:**

Name | Type |
------ | ------ |
`accountIds` | string &#124; Uint8Array‹›[] |
