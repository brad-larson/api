[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/api-derive/src/balances/all"](_packages_api_derive_src_balances_all_.md)

# Module: "packages/api-derive/src/balances/all"

## Index

### Functions

* [all](_packages_api_derive_src_balances_all_.md#all)

## Functions

###  all

▸ **all**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/balances/all.ts:126](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api-derive/src/balances/all.ts#L126)*

**`name`** all

**`example`** 
<BR>

```javascript
const ALICE = 'F7Hs';

api.derive.balances.all(ALICE, ({ accountId, lockedBalance }) => {
  console.log(`The account ${accountId} has a locked balance ${lockedBalance} units.`);
});
```

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

An object containing the results of various balance queries

▸ (`address`: AccountIndex | AccountId | Address | string): *Observable‹DeriveBalancesAll›*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`address` | AccountIndex &#124; AccountId &#124; Address &#124; string | An accounts Id in different formats. |
