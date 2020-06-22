[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["util/decorate"](_util_decorate_.md)

# Module: "util/decorate"

## Index

### Type aliases

* [DeriveAllSections](_util_decorate_.md#deriveallsections)

### Functions

* [decorateSections](_util_decorate_.md#decoratesections)

## Type aliases

###  DeriveAllSections

Ƭ **DeriveAllSections**: *object*

*Defined in [api/src/util/decorate.ts:13](https://github.com/polkadot-js/api/blob/f1b6268784/packages/api/src/util/decorate.ts#L13)*

#### Type declaration:

## Functions

###  decorateSections

▸ **decorateSections**‹**ApiType**, **AllSections**›(`allSections`: AllSections, `decorateMethod`: [DecorateMethod](_types_base_.md#decoratemethod)‹ApiType›): *[DeriveAllSections](_util_decorate_.md#deriveallsections)‹ApiType, AllSections›*

*Defined in [api/src/util/decorate.ts:44](https://github.com/polkadot-js/api/blob/f1b6268784/packages/api/src/util/decorate.ts#L44)*

This is a section decorator which keeps all type information.

**Type parameters:**

▪ **ApiType**: *[ApiTypes](_types_base_.md#apitypes)*

▪ **AllSections**: *AnyDerive*

**Parameters:**

Name | Type |
------ | ------ |
`allSections` | AllSections |
`decorateMethod` | [DecorateMethod](_types_base_.md#decoratemethod)‹ApiType› |

**Returns:** *[DeriveAllSections](_util_decorate_.md#deriveallsections)‹ApiType, AllSections›*
