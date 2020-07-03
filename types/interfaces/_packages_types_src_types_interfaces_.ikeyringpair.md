[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/types/src/types/interfaces"](../modules/_packages_types_src_types_interfaces_.md) › [IKeyringPair](_packages_types_src_types_interfaces_.ikeyringpair.md)

# Interface: IKeyringPair

## Hierarchy

* **IKeyringPair**

## Index

### Properties

* [address](_packages_types_src_types_interfaces_.ikeyringpair.md#address)
* [publicKey](_packages_types_src_types_interfaces_.ikeyringpair.md#publickey)
* [sign](_packages_types_src_types_interfaces_.ikeyringpair.md#sign)

## Properties

###  address

• **address**: *string*

*Defined in [packages/types/src/types/interfaces.ts:18](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/types/interfaces.ts#L18)*

___

###  publicKey

• **publicKey**: *[Uint8Array](../classes/_packages_types_src_codec_raw_.raw.md#static-uint8array)*

*Defined in [packages/types/src/types/interfaces.ts:19](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/types/interfaces.ts#L19)*

___

###  sign

• **sign**: *function*

*Defined in [packages/types/src/types/interfaces.ts:20](https://github.com/polkadot-js/api/blob/66884febea/packages/types/src/types/interfaces.ts#L20)*

#### Type declaration:

▸ (`data`: [Uint8Array](../classes/_packages_types_src_codec_raw_.raw.md#static-uint8array), `options?`: SignOptions): *[Uint8Array](../classes/_packages_types_src_codec_raw_.raw.md#static-uint8array)*

**Parameters:**

Name | Type |
------ | ------ |
`data` | [Uint8Array](../classes/_packages_types_src_codec_raw_.raw.md#static-uint8array) |
`options?` | SignOptions |
