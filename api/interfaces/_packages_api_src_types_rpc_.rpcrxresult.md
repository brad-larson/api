[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/api/src/types/rpc"](../modules/_packages_api_src_types_rpc_.md) › [RpcRxResult](_packages_api_src_types_rpc_.rpcrxresult.md)

# Interface: RpcRxResult ‹**F**›

## Type parameters

▪ **F**: *AnyFunction*

## Hierarchy

* [RxResult](_packages_api_src_types_base_.rxresult.md)‹F›

  ↳ **RpcRxResult**

## Callable

▸ (...`args`: Parameters‹F›): *Observable‹[ObsInnerType](../modules/_packages_api_src_types_base_.md#obsinnertype)‹ReturnType‹F›››*

*Defined in [packages/api/src/types/base.ts:50](https://github.com/polkadot-js/api/blob/66884febea/packages/api/src/types/base.ts#L50)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | Parameters‹F› |

**Returns:** *Observable‹[ObsInnerType](../modules/_packages_api_src_types_base_.md#obsinnertype)‹ReturnType‹F›››*

▸ ‹**T**›(...`args`: Parameters‹F›): *Observable‹T›*

*Defined in [packages/api/src/types/base.ts:51](https://github.com/polkadot-js/api/blob/66884febea/packages/api/src/types/base.ts#L51)*

**Type parameters:**

▪ **T**

**Parameters:**

Name | Type |
------ | ------ |
`...args` | Parameters‹F› |

**Returns:** *Observable‹T›*

## Index

### Methods

* [raw](_packages_api_src_types_rpc_.rpcrxresult.md#raw)

## Methods

###  raw

▸ **raw**(...`args`: Parameters‹F›): *Observable‹Uint8Array & Codec›*

*Defined in [packages/api/src/types/rpc.ts:12](https://github.com/polkadot-js/api/blob/66884febea/packages/api/src/types/rpc.ts#L12)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | Parameters‹F› |

**Returns:** *Observable‹Uint8Array & Codec›*
