[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["rx/Api"](../modules/_rx_api_.md) › [ApiRx](_rx_api_.apirx.md)

# Class: ApiRx

# @polkadot/api/rx

 ## Overview

**`name`** ApiRx

**`description`** 
ApiRx is a powerfull RxJS Observable wrapper around the RPC and interfaces on the Polkadot network. As a full Observable API, all interface calls return RxJS Observables, including the static `.create(...)`. In the same fashion and subscription-based methods return long-running Observables that update with the latest values.

The API is well suited to real-time applications where the latest state is needed, unlocking the subscription-based features of Polkadot (and Substrate) clients. Some familiarity with RxJS is a requirement to use the API, however just understanding `.subscribe` and `.pipe` on Observables will unlock full-scale use thereof.

**`see`** [ApiPromise](_promise_api_.apipromise.md)

## Usage

Making rpc calls -
<BR>

```javascript
import ApiRx from '@polkadot/api/rx';

// initialise via Promise & static create
const api = await ApiRx.create().toPromise();

// make a call to retrieve the current network head
api.rpc.chain.subscribeNewHeads().subscribe((header) => {
  console.log(`Chain is at #${header.number}`);
});
```
<BR>

Subscribing to chain state -
<BR>

```javascript
import { combineLatest } from 'rxjs';
import { pairwise, switchMap } from 'rxjs/operators';
import { ApiRx, WsProvider } from '@polkadot/api';

// initialise a provider with a specific endpoint
const provider = new WsProvider('wss://example.com:9944')

// initialise via isReady & new with specific provider
new ApiRx({ provider })
  .isReady
  .pipe(
    switchMap((api) =>
      combineLatest([
        api.query.timestamp.blockPeriod(),
        api.query.timestamp.now().pipe(pairwise())
      ])
    )
  )
  .subscribe(([blockPeriod, timestamp]) => {
     const elapsed = timestamp[1].toNumber() - timestamp[0].toNumber();
     console.log(`timestamp ${timestamp[1]} \nelapsed ${elapsed} \n(${blockPeriod}s target)`);
  });
```
<BR>

Submitting a transaction -
<BR>

```javascript
import { first, switchMap } from 'rxjs/operators';
import ApiRx from '@polkadot/api/rx';

// import the test keyring (already has dev keys for Alice, Bob, Charlie, Eve & Ferdie)
import testingPairs from '@polkadot/keyring/testingPairs';
const keyring = testingPairs();

// get api via Promise
const api = await ApiRx.create().toPromise();

// retrieve nonce for the account
api.query.system
  .account(keyring.alice.address)
  .pipe(
     first(),
     // pipe nonce into transfer
     switchMap(([nonce]) =>
       api.tx.balances
         // create transfer
         .transfer(keyring.bob.address, 12345)
         // sign the transcation
         .sign(keyring.alice, { nonce })
         // send the transaction
         .send()
     )
  )
  // subscribe to overall result
  .subscribe(({ status }) => {
    if (status.isInBlock) {
      console.log('Completed at block hash', status.asFinalized.toHex());
    }
  });
```

## Hierarchy

* ApiBase‹"rxjs"›

  ↳ **ApiRx**

## Index

### Constructors

* [constructor](_rx_api_.apirx.md#constructor)

### Properties

* [registry](_rx_api_.apirx.md#readonly-registry)

### Accessors

* [consts](_rx_api_.apirx.md#consts)
* [derive](_rx_api_.apirx.md#derive)
* [extrinsicVersion](_rx_api_.apirx.md#extrinsicversion)
* [genesisHash](_rx_api_.apirx.md#genesishash)
* [hasSubscriptions](_rx_api_.apirx.md#hassubscriptions)
* [isConnected](_rx_api_.apirx.md#isconnected)
* [isReady](_rx_api_.apirx.md#isready)
* [libraryInfo](_rx_api_.apirx.md#libraryinfo)
* [query](_rx_api_.apirx.md#query)
* [queryMulti](_rx_api_.apirx.md#querymulti)
* [rpc](_rx_api_.apirx.md#rpc)
* [runtimeMetadata](_rx_api_.apirx.md#runtimemetadata)
* [runtimeVersion](_rx_api_.apirx.md#runtimeversion)
* [rx](_rx_api_.apirx.md#rx)
* [tx](_rx_api_.apirx.md#tx)
* [type](_rx_api_.apirx.md#type)

### Methods

* [clone](_rx_api_.apirx.md#clone)
* [createType](_rx_api_.apirx.md#createtype)
* [disconnect](_rx_api_.apirx.md#disconnect)
* [findCall](_rx_api_.apirx.md#findcall)
* [findError](_rx_api_.apirx.md#finderror)
* [injectMetadata](_rx_api_.apirx.md#injectmetadata)
* [off](_rx_api_.apirx.md#off)
* [on](_rx_api_.apirx.md#on)
* [once](_rx_api_.apirx.md#once)
* [registerTypes](_rx_api_.apirx.md#registertypes)
* [setSigner](_rx_api_.apirx.md#setsigner)
* [sign](_rx_api_.apirx.md#sign)
* [create](_rx_api_.apirx.md#static-create)

## Constructors

###  constructor

\+ **new ApiRx**(`options?`: ApiOptions): *[ApiRx](_rx_api_.apirx.md)*

*Overrides void*

*Defined in [api/src/rx/Api.ts:141](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/rx/Api.ts#L141)*

**`description`** Create an instance of the ApiRx class

**`example`** 
<BR>

```javascript
import { switchMap } from 'rxjs/operators';
import Api from '@polkadot/api/rx';

new Api().isReady
  .pipe(
    switchMap((api) =>
      api.rpc.chain.subscribeNewHeads()
  ))
  .subscribe((header) => {
    console.log(`new block #${header.number.toNumber()}`);
  });
```

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options?` | ApiOptions | Options to create an instance. Can be either [[ApiOptions]] or [[WsProvider]] |

**Returns:** *[ApiRx](_rx_api_.apirx.md)*

## Properties

### `Readonly` registry

• **registry**: *Registry*

*Inherited from [Decorate](_base_decorate_.decorate.md).[registry](_base_decorate_.decorate.md#readonly-registry)*

*Defined in [api/src/base/Decorate.ts:48](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/Decorate.ts#L48)*

## Accessors

###  consts

• **get consts**(): *[Constants](../interfaces/_augment_consts_._metadata_decorated_consts_types_.constants.md)*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[consts](_promise_api_.apipromise.md#consts)*

*Defined in [api/src/base/index.ts:80](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L80)*

**`description`** Contains the parameter types (constants) of all modules.

The values are instances of the appropriate type and are accessible using `section`.`constantName`,

**`example`** 
<BR>

```javascript
console.log(api.consts.democracy.enactmentPeriod.toString())
```

**Returns:** *[Constants](../interfaces/_augment_consts_._metadata_decorated_consts_types_.constants.md)*

___

###  derive

• **get derive**(): *ReturnType‹ApiBase<"rxjs">["_decorateDerive"]›*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[derive](_promise_api_.apipromise.md#derive)*

*Defined in [api/src/base/index.ts:96](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L96)*

**`description`** Derived results that are injected into the API, allowing for combinations of various query results.

**`example`** 
<BR>

```javascript
api.derive.chain.bestNumber((number) => {
  console.log('best number', number);
});
```

**Returns:** *ReturnType‹ApiBase<"rxjs">["_decorateDerive"]›*

___

###  extrinsicVersion

• **get extrinsicVersion**(): *number*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[extrinsicVersion](_promise_api_.apipromise.md#extrinsicversion)*

*Defined in [api/src/base/index.ts:103](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L103)*

**`description`** Returns the version of extrinsics in-use on this chain

**Returns:** *number*

___

###  genesisHash

• **get genesisHash**(): *Hash*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[genesisHash](_promise_api_.apipromise.md#genesishash)*

*Defined in [api/src/base/index.ts:110](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L110)*

**`description`** Contains the genesis Hash of the attached chain. Apart from being useful to determine the actual chain, it can also be used to sign immortal transactions.

**Returns:** *Hash*

___

###  hasSubscriptions

• **get hasSubscriptions**(): *boolean*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[hasSubscriptions](_promise_api_.apipromise.md#hassubscriptions)*

*Overrides [Decorate](_base_decorate_.decorate.md).[hasSubscriptions](_base_decorate_.decorate.md#hassubscriptions)*

*Defined in [api/src/base/index.ts:117](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L117)*

**`description`** `true` when subscriptions are supported

**Returns:** *boolean*

___

###  isConnected

• **get isConnected**(): *Observable‹boolean›*

*Defined in [api/src/rx/Api.ts:179](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/rx/Api.ts#L179)*

**`description`** Observable that carries the connected state for the provider. Results in a boolean flag that is true/false based on the connectivity.

**Returns:** *Observable‹boolean›*

___

###  isReady

• **get isReady**(): *Observable‹[ApiRx](_rx_api_.apirx.md)›*

*Defined in [api/src/rx/Api.ts:186](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/rx/Api.ts#L186)*

**`description`** Observable that returns the first time we are connected and loaded

**Returns:** *Observable‹[ApiRx](_rx_api_.apirx.md)›*

___

###  libraryInfo

• **get libraryInfo**(): *string*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[libraryInfo](_promise_api_.apipromise.md#libraryinfo)*

*Defined in [api/src/base/index.ts:124](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L124)*

**`description`** The library information name & version (from package.json)

**Returns:** *string*

___

###  query

• **get query**(): *[QueryableStorage](../interfaces/_augment_query_._api_types_storage_.queryablestorage.md)‹"rxjs"›*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[query](_promise_api_.apipromise.md#query)*

*Defined in [api/src/base/index.ts:142](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L142)*

**`description`** Contains all the chain state modules and their subsequent methods in the API. These are attached dynamically from the runtime metadata.

All calls inside the namespace, is denoted by `section`.`method` and may take an optional query parameter. As an example, `api.query.timestamp.now()` (current block timestamp) does not take parameters, while `api.query.system.account(<accountId>)` (retrieving the associated nonce & balances for an account), takes the `AccountId` as a parameter.

**`example`** 
<BR>

```javascript
api.query.system.account(<accountId>, ([nonce, balance]) => {
  console.log('new free balance', balance.free, 'new nonce', nonce);
});
```

**Returns:** *[QueryableStorage](../interfaces/_augment_query_._api_types_storage_.queryablestorage.md)‹"rxjs"›*

___

###  queryMulti

• **get queryMulti**(): *[QueryableStorageMulti](../modules/_types_storage_.md#queryablestoragemulti)‹"rxjs"›*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[queryMulti](_promise_api_.apipromise.md#querymulti)*

*Defined in [api/src/base/index.ts:168](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L168)*

**`description`** Allows for the querying of multiple storage entries and the combination thereof into a single result. This is a very optimal way to make multiple queries since it only makes a single connection to the node and retrieves the data over one subscription.

**`example`** 
<BR>

```javascript
const unsub = await api.queryMulti(
  [
    // you can include the storage without any parameters
    api.query.balances.totalIssuance,
    // or you can pass parameters to the storage query
    [api.query.system.account, '5GrwvaEF5zXb26Fz9rcQpDWS57CtERHpNehXCPcNoHGKutQY']
  ],
  ([existential, [, { free }]]) => {
    console.log(`You have ${free.sub(existential)} more than the existential deposit`);

    unsub();
  }
);
```

**Returns:** *[QueryableStorageMulti](../modules/_types_storage_.md#queryablestoragemulti)‹"rxjs"›*

___

###  rpc

• **get rpc**(): *[DecoratedRpc](../modules/_types_rpc_.md#decoratedrpc)‹"rxjs", [RpcInterface](../interfaces/_augment_rpc_._rpc_core_types_.rpcinterface.md)›*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[rpc](_promise_api_.apipromise.md#rpc)*

*Defined in [api/src/base/index.ts:186](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L186)*

**`description`** Contains all the raw rpc sections and their subsequent methods in the API as defined by the jsonrpc interface definitions. Unlike the dynamic `api.query` and `api.tx` sections, these methods are fixed (although extensible with node upgrades) and not determined by the runtime.

RPC endpoints available here allow for the query of chain, node and system information, in addition to providing interfaces for the raw queries of state (using known keys) and the submission of transactions.

**`example`** 
<BR>

```javascript
api.rpc.chain.subscribeNewHeads((header) => {
  console.log('new header', header);
});
```

**Returns:** *[DecoratedRpc](../modules/_types_rpc_.md#decoratedrpc)‹"rxjs", [RpcInterface](../interfaces/_augment_rpc_._rpc_core_types_.rpcinterface.md)›*

___

###  runtimeMetadata

• **get runtimeMetadata**(): *Metadata*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[runtimeMetadata](_promise_api_.apipromise.md#runtimemetadata)*

*Defined in [api/src/base/index.ts:193](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L193)*

**`description`** Yields the current attached runtime metadata. Generally this is only used to construct extrinsics & storage, but is useful for current runtime inspection.

**Returns:** *Metadata*

___

###  runtimeVersion

• **get runtimeVersion**(): *RuntimeVersion*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[runtimeVersion](_promise_api_.apipromise.md#runtimeversion)*

*Defined in [api/src/base/index.ts:200](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L200)*

**`description`** Contains the version information for the current runtime.

**Returns:** *RuntimeVersion*

___

###  rx

• **get rx**(): *Pick‹ApiInterfaceRx, "tx" | "rpc"›*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[rx](_promise_api_.apipromise.md#rx)*

*Defined in [api/src/base/index.ts:207](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L207)*

**`description`** The underlying Rx API interface

**Returns:** *Pick‹ApiInterfaceRx, "tx" | "rpc"›*

___

###  tx

• **get tx**(): *[SubmittableExtrinsics](../interfaces/_augment_tx_._api_types_submittable_.submittableextrinsics.md)‹"rxjs"›*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[tx](_promise_api_.apipromise.md#tx)*

*Defined in [api/src/base/index.ts:232](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L232)*

**`description`** Contains all the extrinsic modules and their subsequent methods in the API. It allows for the construction of transactions and the submission thereof. These are attached dynamically from the runtime metadata.

**`example`** 
<BR>

```javascript
api.tx.balances
  .transfer(<recipientId>, <balance>)
  .signAndSend(<keyPair>, ({status}) => {
    console.log('tx status', status.asFinalized.toHex());
  });
```

**Returns:** *[SubmittableExtrinsics](../interfaces/_augment_tx_._api_types_submittable_.submittableextrinsics.md)‹"rxjs"›*

___

###  type

• **get type**(): *[ApiTypes](../modules/_types_base_.md#apitypes)*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[type](_promise_api_.apipromise.md#type)*

*Defined in [api/src/base/index.ts:214](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L214)*

**`description`** The type of this API instance, either 'rxjs' or 'promise'

**Returns:** *[ApiTypes](../modules/_types_base_.md#apitypes)*

## Methods

###  clone

▸ **clone**(): *[ApiRx](_rx_api_.apirx.md)*

*Defined in [api/src/rx/Api.ts:193](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/rx/Api.ts#L193)*

**`description`** Returns a clone of this ApiRx instance (new underlying provider connection)

**Returns:** *[ApiRx](_rx_api_.apirx.md)*

___

###  createType

▸ **createType**‹**K**›(`type`: K, ...`params`: any[]): *InterfaceTypes[K]*

*Inherited from [Decorate](_base_decorate_.decorate.md).[createType](_base_decorate_.decorate.md#createtype)*

*Defined in [api/src/base/Decorate.ts:148](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/Decorate.ts#L148)*

**`description`** Creates an instance of a type as registered

**Type parameters:**

▪ **K**: *keyof InterfaceTypes*

**Parameters:**

Name | Type |
------ | ------ |
`type` | K |
`...params` | any[] |

**Returns:** *InterfaceTypes[K]*

___

###  disconnect

▸ **disconnect**(): *void*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[disconnect](_promise_api_.apipromise.md#disconnect)*

*Defined in [api/src/base/index.ts:239](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L239)*

**`description`** Disconnect from the underlying provider, halting all network traffic

**Returns:** *void*

___

###  findCall

▸ **findCall**(`callIndex`: Uint8Array | string): *CallFunction*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[findCall](_promise_api_.apipromise.md#findcall)*

*Defined in [api/src/base/index.ts:246](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L246)*

**`description`** Finds the definition for a specific [[CallFunction]] based on the index supplied

**Parameters:**

Name | Type |
------ | ------ |
`callIndex` | Uint8Array &#124; string |

**Returns:** *CallFunction*

___

###  findError

▸ **findError**(`errorIndex`: Uint8Array | string): *RegistryError*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[findError](_promise_api_.apipromise.md#finderror)*

*Defined in [api/src/base/index.ts:253](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L253)*

**`description`** Finds the definition for a specific [[RegistryError]] based on the index supplied

**Parameters:**

Name | Type |
------ | ------ |
`errorIndex` | Uint8Array &#124; string |

**Returns:** *RegistryError*

___

###  injectMetadata

▸ **injectMetadata**(`metadata`: Metadata, `fromEmpty?`: undefined | false | true): *void*

*Inherited from [Decorate](_base_decorate_.decorate.md).[injectMetadata](_base_decorate_.decorate.md#injectmetadata)*

*Defined in [api/src/base/Decorate.ts:166](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/Decorate.ts#L166)*

**Parameters:**

Name | Type |
------ | ------ |
`metadata` | Metadata |
`fromEmpty?` | undefined &#124; false &#124; true |

**Returns:** *void*

___

###  off

▸ **off**(`type`: ApiInterfaceEvents, `handler`: function): *this*

*Inherited from [Events](_base_events_.events.md).[off](_base_events_.events.md#off)*

*Defined in [api/src/base/Events.ts:62](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/Events.ts#L62)*

**`description`** Remove the given eventemitter handler

**`example`** 
<BR>

```javascript
const handler = (): void => {
 console.log('Connected !);
};

// Start listening
api.on('connected', handler);

// Stop listening
api.off('connected', handler);
```

**Parameters:**

▪ **type**: *ApiInterfaceEvents*

The type of event the callback was attached to. Available events are `connected`, `disconnected`, `ready` and `error`

▪ **handler**: *function*

The callback to unregister.

▸ (...`args`: any[]): *any*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  on

▸ **on**(`type`: ApiInterfaceEvents, `handler`: function): *this*

*Inherited from [Events](_base_events_.events.md).[on](_base_events_.events.md#on)*

*Defined in [api/src/base/Events.ts:35](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/Events.ts#L35)*

**`description`** Attach an eventemitter handler to listen to a specific event

**`example`** 
<BR>

```javascript
api.on('connected', (): void => {
  console.log('API has been connected to the endpoint');
});

api.on('disconnected', (): void => {
  console.log('API has been disconnected from the endpoint');
});
```

**Parameters:**

▪ **type**: *ApiInterfaceEvents*

The type of event to listen to. Available events are `connected`, `disconnected`, `ready` and `error`

▪ **handler**: *function*

The callback to be called when the event fires. Depending on the event type, it could fire with additional arguments.

▸ (...`args`: any[]): *any*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  once

▸ **once**(`type`: ApiInterfaceEvents, `handler`: function): *this*

*Inherited from [Events](_base_events_.events.md).[once](_base_events_.events.md#once)*

*Defined in [api/src/base/Events.ts:87](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/Events.ts#L87)*

**`description`** Attach an one-time eventemitter handler to listen to a specific event

**`example`** 
<BR>

```javascript
api.once('connected', (): void => {
  console.log('API has been connected to the endpoint');
});

api.once('disconnected', (): void => {
  console.log('API has been disconnected from the endpoint');
});
```

**Parameters:**

▪ **type**: *ApiInterfaceEvents*

The type of event to listen to. Available events are `connected`, `disconnected`, `ready` and `error`

▪ **handler**: *function*

The callback to be called when the event fires. Depending on the event type, it could fire with additional arguments.

▸ (...`args`: any[]): *any*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  registerTypes

▸ **registerTypes**(`types?`: RegistryTypes): *void*

*Inherited from [Decorate](_base_decorate_.decorate.md).[registerTypes](_base_decorate_.decorate.md#registertypes)*

*Defined in [api/src/base/Decorate.ts:155](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/Decorate.ts#L155)*

**`description`** Register additional user-defined of chain-specific types in the type registry

**Parameters:**

Name | Type |
------ | ------ |
`types?` | RegistryTypes |

**Returns:** *void*

___

###  setSigner

▸ **setSigner**(`signer`: Signer): *void*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[setSigner](_promise_api_.apipromise.md#setsigner)*

*Defined in [api/src/base/index.ts:260](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L260)*

**`description`** Set an external signer which will be used to sign extrinsic when account passed in is not KeyringPair

**Parameters:**

Name | Type |
------ | ------ |
`signer` | Signer |

**Returns:** *void*

___

###  sign

▸ **sign**(`address`: KeyringSigner | string, `data`: SignerPayloadRawBase, `__namedParameters`: object): *Promise‹string›*

*Inherited from [ApiPromise](_promise_api_.apipromise.md).[sign](_promise_api_.apipromise.md#sign)*

*Defined in [api/src/base/index.ts:267](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/base/index.ts#L267)*

**`description`** Signs a raw signer payload, string or Uint8Array

**Parameters:**

▪ **address**: *KeyringSigner | string*

▪ **data**: *SignerPayloadRawBase*

▪`Default value`  **__namedParameters**: *object*= {}

Name | Type |
------ | ------ |
`signer` | undefined &#124; Signer |

**Returns:** *Promise‹string›*

___

### `Static` create

▸ **create**(`options?`: ApiOptions): *Observable‹[ApiRx](_rx_api_.apirx.md)›*

*Defined in [api/src/rx/Api.ts:139](https://github.com/polkadot-js/api/blob/ad6b8280a2/packages/api/src/rx/Api.ts#L139)*

**`description`** Creates an ApiRx instance using the supplied provider. Returns an Observable containing the actual Api instance.

**`example`** 
<BR>

```javascript
import { switchMap } from 'rxjs/operators';
import Api from '@polkadot/api/rx';

Api.create()
  .pipe(
    switchMap((api) =>
      api.rpc.chain.subscribeNewHeads()
  ))
  .subscribe((header) => {
    console.log(`new block #${header.number.toNumber()}`);
  });
```

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options?` | ApiOptions | options that is passed to the class contructor. Can be either [[ApiOptions]] or [[WsProvider]] |

**Returns:** *Observable‹[ApiRx](_rx_api_.apirx.md)›*
