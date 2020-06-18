[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["chain/bestNumberLag"](_chain_bestnumberlag_.md)

# Module: "chain/bestNumberLag"

## Index

### Functions

* [bestNumberLag](_chain_bestnumberlag_.md#bestnumberlag)

## Functions

###  bestNumberLag

▸ **bestNumberLag**(`api`: ApiInterfaceRx): *function*

*Defined in [packages/api-derive/src/chain/bestNumberLag.ts:26](https://github.com/polkadot-js/api/blob/5c5db2709b/packages/api-derive/src/chain/bestNumberLag.ts#L26)*

**`name`** bestNumberLag

**`description`** Calculates the lag between finalized head and best head

**`example`** 
<BR>

```javascript
api.derive.chain.bestNumberLag((lag) => {
  console.log(`finalized is ${lag} blocks behind head`);
});
```

**Parameters:**

Name | Type |
------ | ------ |
`api` | ApiInterfaceRx |

**Returns:** *function*

A number of blocks

▸ (): *Observable‹BlockNumber›*
