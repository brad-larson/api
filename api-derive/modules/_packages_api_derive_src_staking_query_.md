[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/api-derive/src/staking/query"](_packages_api_derive_src_staking_query_.md)

# Module: "packages/api-derive/src/staking/query"

## Index

### Functions

* [query](_packages_api_derive_src_staking_query_.md#query)
* [queryMulti](_packages_api_derive_src_staking_query_.md#querymulti)

## Functions

###  query

▸ **query**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/query.ts:109](https://github.com/polkadot-js/api/blob/8b492021af/packages/api-derive/src/staking/query.ts#L109)*

**`description`** From a stash, retrieve the controllerId and all relevant details

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`accountId`: Uint8Array | string): *Observable‹DeriveStakingQuery›*

**Parameters:**

Name | Type |
------ | ------ |
`accountId` | Uint8Array &#124; string |

___

###  queryMulti

▸ **queryMulti**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/query.ts:117](https://github.com/polkadot-js/api/blob/8b492021af/packages/api-derive/src/staking/query.ts#L117)*

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (`accountIds`: string | Uint8Array‹›[]): *Observable‹DeriveStakingQuery[]›*

**Parameters:**

Name | Type |
------ | ------ |
`accountIds` | string &#124; Uint8Array‹›[] |
