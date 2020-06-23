[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["staking/validators"](_staking_validators_.md)

# Module: "staking/validators"

## Index

### Functions

* [nextElected](_staking_validators_.md#nextelected)
* [validators](_staking_validators_.md#validators)

## Functions

###  nextElected

▸ **nextElected**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/validators.ts:14](https://github.com/polkadot-js/api/blob/e5c2c6a228/packages/api-derive/src/staking/validators.ts#L14)*

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (): *Observable‹AccountId[]›*

___

###  validators

▸ **validators**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/staking/validators.ts:30](https://github.com/polkadot-js/api/blob/e5c2c6a228/packages/api-derive/src/staking/validators.ts#L30)*

**`description`** Retrieve latest list of validators

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

▸ (): *Observable‹DeriveStakingValidators›*
