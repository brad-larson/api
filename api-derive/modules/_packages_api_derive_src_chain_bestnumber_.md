[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/api-derive/src/chain/bestNumber"](_packages_api_derive_src_chain_bestnumber_.md)

# Module: "packages/api-derive/src/chain/bestNumber"

## Index

### Functions

* [bestNumber](_packages_api_derive_src_chain_bestnumber_.md#bestnumber)

## Functions

###  bestNumber

▸ **bestNumber**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/chain/bestNumber.ts:25](https://github.com/polkadot-js/api/blob/afa0e63ae8/packages/api-derive/src/chain/bestNumber.ts#L25)*

**`name`** bestNumber

**`example`** 
<BR>

```javascript
api.derive.chain.bestNumber((blockNumber) => {
  console.log(`the current best block is #${blockNumber}`);
});
```

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

The latest block number.

▸ (): *Observable‹BlockNumber›*
