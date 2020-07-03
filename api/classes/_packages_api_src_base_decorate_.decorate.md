[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/api/src/base/Decorate"](../modules/_packages_api_src_base_decorate_.md) › [Decorate](_packages_api_src_base_decorate_.decorate.md)

# Class: Decorate ‹**ApiType**›

## Type parameters

▪ **ApiType**: *[ApiTypes](../modules/_packages_api_src_types_base_.md#apitypes)*

## Hierarchy

* [Events](_packages_api_src_base_events_.events.md)

  ↳ **Decorate**

  ↳ [Init](_packages_api_src_base_init_.init.md)

## Index

### Constructors

* [constructor](_packages_api_src_base_decorate_.decorate.md#constructor)

### Properties

* [registry](_packages_api_src_base_decorate_.decorate.md#readonly-registry)

### Accessors

* [hasSubscriptions](_packages_api_src_base_decorate_.decorate.md#hassubscriptions)

### Methods

* [createType](_packages_api_src_base_decorate_.decorate.md#createtype)
* [injectMetadata](_packages_api_src_base_decorate_.decorate.md#injectmetadata)
* [off](_packages_api_src_base_decorate_.decorate.md#off)
* [on](_packages_api_src_base_decorate_.decorate.md#on)
* [once](_packages_api_src_base_decorate_.decorate.md#once)
* [registerTypes](_packages_api_src_base_decorate_.decorate.md#registertypes)

## Constructors

###  constructor

\+ **new Decorate**(`options`: ApiOptions, `type`: [ApiTypes](../modules/_packages_api_src_types_base_.md#apitypes), `decorateMethod`: [DecorateMethod](../modules/_packages_api_src_types_base_.md#decoratemethod)‹ApiType›): *[Decorate](_packages_api_src_base_decorate_.decorate.md)*

*Defined in [packages/api/src/base/Decorate.ts:107](https://github.com/polkadot-js/api/blob/63096cc238/packages/api/src/base/Decorate.ts#L107)*

**`description`** Create an instance of the class

**`example`** 
<BR>

```javascript
import Api from '@polkadot/api/promise';

const api = new Api().isReady();

api.rpc.subscribeNewHeads((header) => {
  console.log(`new block #${header.number.toNumber()}`);
});
```

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options` | ApiOptions | Options object to create API instance or a Provider instance  |
`type` | [ApiTypes](../modules/_packages_api_src_types_base_.md#apitypes) | - |
`decorateMethod` | [DecorateMethod](../modules/_packages_api_src_types_base_.md#decoratemethod)‹ApiType› | - |

**Returns:** *[Decorate](_packages_api_src_base_decorate_.decorate.md)*

## Properties

### `Readonly` registry

• **registry**: *Registry*

*Defined in [packages/api/src/base/Decorate.ts:48](https://github.com/polkadot-js/api/blob/63096cc238/packages/api/src/base/Decorate.ts#L48)*

## Accessors

###  hasSubscriptions

• **get hasSubscriptions**(): *boolean*

*Defined in [packages/api/src/base/Decorate.ts:162](https://github.com/polkadot-js/api/blob/63096cc238/packages/api/src/base/Decorate.ts#L162)*

**Returns:** *boolean*

`true` if the API operates with subscriptions

## Methods

###  createType

▸ **createType**‹**K**›(`type`: K, ...`params`: unknown[]): *InterfaceTypes[K]*

*Defined in [packages/api/src/base/Decorate.ts:148](https://github.com/polkadot-js/api/blob/63096cc238/packages/api/src/base/Decorate.ts#L148)*

**`description`** Creates an instance of a type as registered

**Type parameters:**

▪ **K**: *keyof InterfaceTypes*

**Parameters:**

Name | Type |
------ | ------ |
`type` | K |
`...params` | unknown[] |

**Returns:** *InterfaceTypes[K]*

___

###  injectMetadata

▸ **injectMetadata**(`metadata`: Metadata, `fromEmpty?`: undefined | false | true): *void*

*Defined in [packages/api/src/base/Decorate.ts:166](https://github.com/polkadot-js/api/blob/63096cc238/packages/api/src/base/Decorate.ts#L166)*

**Parameters:**

Name | Type |
------ | ------ |
`metadata` | Metadata |
`fromEmpty?` | undefined &#124; false &#124; true |

**Returns:** *void*

___

###  off

▸ **off**(`type`: ApiInterfaceEvents, `handler`: function): *this*

*Inherited from [Events](_packages_api_src_base_events_.events.md).[off](_packages_api_src_base_events_.events.md#off)*

*Defined in [packages/api/src/base/Events.ts:62](https://github.com/polkadot-js/api/blob/63096cc238/packages/api/src/base/Events.ts#L62)*

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

*Inherited from [Events](_packages_api_src_base_events_.events.md).[on](_packages_api_src_base_events_.events.md#on)*

*Defined in [packages/api/src/base/Events.ts:35](https://github.com/polkadot-js/api/blob/63096cc238/packages/api/src/base/Events.ts#L35)*

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

*Inherited from [Events](_packages_api_src_base_events_.events.md).[once](_packages_api_src_base_events_.events.md#once)*

*Defined in [packages/api/src/base/Events.ts:87](https://github.com/polkadot-js/api/blob/63096cc238/packages/api/src/base/Events.ts#L87)*

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

*Defined in [packages/api/src/base/Decorate.ts:155](https://github.com/polkadot-js/api/blob/63096cc238/packages/api/src/base/Decorate.ts#L155)*

**`description`** Register additional user-defined of chain-specific types in the type registry

**Parameters:**

Name | Type |
------ | ------ |
`types?` | RegistryTypes |

**Returns:** *void*
