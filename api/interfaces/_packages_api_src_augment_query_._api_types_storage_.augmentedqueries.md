[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["packages/api/src/augment/query"](../modules/_packages_api_src_augment_query_.md) › ["api/types/storage"](../modules/_packages_api_src_augment_query_._api_types_storage_.md) › [AugmentedQueries](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md)

# Interface: AugmentedQueries ‹**ApiType**›

## Type parameters

▪ **ApiType**

## Hierarchy

* **AugmentedQueries**

## Index

### Properties

* [authorship](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#authorship)
* [babe](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#babe)
* [balances](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#balances)
* [contracts](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#contracts)
* [council](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#council)
* [democracy](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#democracy)
* [elections](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#elections)
* [grandpa](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#grandpa)
* [identity](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#identity)
* [imOnline](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#imonline)
* [indices](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#indices)
* [multisig](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#multisig)
* [offences](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#offences)
* [proxy](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#proxy)
* [randomnessCollectiveFlip](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#randomnesscollectiveflip)
* [recovery](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#recovery)
* [scheduler](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#scheduler)
* [session](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#session)
* [society](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#society)
* [staking](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#staking)
* [sudo](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#sudo)
* [system](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#system)
* [technicalCommittee](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#technicalcommittee)
* [technicalMembership](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#technicalmembership)
* [timestamp](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#timestamp)
* [transactionPayment](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#transactionpayment)
* [treasury](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#treasury)
* [vesting](_packages_api_src_augment_query_._api_types_storage_.augmentedqueries.md#vesting)

## Properties

###  authorship

• **authorship**: *object*

*Defined in [packages/api/src/augment/query.ts:34](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L34)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **author**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **didSetUncles**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **uncles**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  babe

• **babe**: *object*

*Defined in [packages/api/src/augment/query.ts:49](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L49)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **authorities**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **currentSlot**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **epochIndex**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **genesisSlot**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **initialized**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **lateness**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **nextEpochConfig**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **nextRandomness**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **randomness**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **segmentIndex**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **underConstruction**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  balances

• **balances**: *object*

*Defined in [packages/api/src/augment/query.ts:119](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L119)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **account**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **locks**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **storageVersion**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **totalIssuance**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  contracts

• **contracts**: *object*

*Defined in [packages/api/src/augment/query.ts:143](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L143)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **accountCounter**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **codeStorage**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **contractInfoOf**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **currentSchedule**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **pristineCode**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  council

• **council**: *object*

*Defined in [packages/api/src/augment/query.ts:168](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L168)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **members**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **prime**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **proposalCount**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **proposalOf**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **proposals**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **voting**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  democracy

• **democracy**: *object*

*Defined in [packages/api/src/augment/query.ts:196](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L196)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **blacklist**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **cancellations**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **depositOf**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **lastTabledWasExternal**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **locks**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **lowestUnbaked**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **nextExternal**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **preimages**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **publicPropCount**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **publicProps**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **referendumCount**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **referendumInfoOf**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **storageVersion**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **votingOf**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  elections

• **elections**: *object*

*Defined in [packages/api/src/augment/query.ts:274](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L274)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **candidates**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **electionRounds**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **members**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **runnersUp**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **voting**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  grandpa

• **grandpa**: *object*

*Defined in [packages/api/src/augment/query.ts:300](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L300)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **currentSetId**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **nextForced**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **pendingChange**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **setIdSession**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **stalled**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **state**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  identity

• **identity**: *object*

*Defined in [packages/api/src/augment/query.ts:331](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L331)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **identityOf**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **registrars**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **subsOf**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **superOf**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  imOnline

• **imOnline**: *object*

*Defined in [packages/api/src/augment/query.ts:360](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L360)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **authoredBlocks**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **heartbeatAfter**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **keys**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **receivedHeartbeats**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  indices

• **indices**: *object*

*Defined in [packages/api/src/augment/query.ts:386](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L386)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **accounts**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  multisig

• **multisig**: *object*

*Defined in [packages/api/src/augment/query.ts:393](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L393)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **calls**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **multisigs**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  offences

• **offences**: *object*

*Defined in [packages/api/src/augment/query.ts:401](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L401)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **concurrentReportsIndex**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **deferredOffences**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **reports**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **reportsByKindIndex**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  proxy

• **proxy**: *object*

*Defined in [packages/api/src/augment/query.ts:426](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L426)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **proxies**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  randomnessCollectiveFlip

• **randomnessCollectiveFlip**: *object*

*Defined in [packages/api/src/augment/query.ts:434](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L434)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **randomMaterial**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  recovery

• **recovery**: *object*

*Defined in [packages/api/src/augment/query.ts:443](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L443)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **activeRecoveries**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **proxy**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **recoverable**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  scheduler

• **scheduler**: *object*

*Defined in [packages/api/src/augment/query.ts:463](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L463)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **agenda**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **lookup**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  session

• **session**: *object*

*Defined in [packages/api/src/augment/query.ts:474](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L474)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **currentIndex**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **disabledValidators**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **keyOwner**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **nextKeys**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **queuedChanged**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **queuedKeys**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **validators**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  society

• **society**: *object*

*Defined in [packages/api/src/augment/query.ts:509](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L509)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **bids**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **candidates**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **defender**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **defenderVotes**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **founder**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **head**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **maxMembers**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **members**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **payouts**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **pot**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **rules**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **strikes**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **suspendedCandidates**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **suspendedMembers**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **votes**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **vouching**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  staking

• **staking**: *object*

*Defined in [packages/api/src/augment/query.ts:577](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L577)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **activeEra**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **bonded**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **bondedEras**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **canceledSlashPayout**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **currentEra**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **earliestUnappliedSlash**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **eraElectionStatus**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **erasRewardPoints**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **erasStakers**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **erasStakersClipped**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **erasStartSessionIndex**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **erasTotalStake**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **erasValidatorPrefs**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **erasValidatorReward**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **forceEra**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **historyDepth**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **invulnerables**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **isCurrentSessionFinal**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **ledger**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **minimumValidatorCount**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **nominatorSlashInEra**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **nominators**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **payee**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **queuedElected**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **queuedScore**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **slashRewardFraction**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **slashingSpans**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **snapshotNominators**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **snapshotValidators**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **spanSlash**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **storageVersion**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **unappliedSlashes**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **validatorCount**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **validatorSlashInEra**: *[AugmentedQueryDoubleMap](../modules/_packages_api_src_types_storage_.md#augmentedquerydoublemap)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **validators**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  sudo

• **sudo**: *object*

*Defined in [packages/api/src/augment/query.ts:774](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L774)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **key**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  system

• **system**: *object*

*Defined in [packages/api/src/augment/query.ts:781](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L781)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **account**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **allExtrinsicsLen**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **blockHash**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **blockWeight**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **digest**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **eventCount**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **eventTopics**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **events**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **executionPhase**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **extrinsicCount**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **extrinsicData**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **extrinsicsRoot**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **lastRuntimeUpgrade**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **number**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **parentHash**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  technicalCommittee

• **technicalCommittee**: *object*

*Defined in [packages/api/src/augment/query.ts:853](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L853)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **members**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **prime**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **proposalCount**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **proposalOf**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **proposals**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **voting**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  technicalMembership

• **technicalMembership**: *object*

*Defined in [packages/api/src/augment/query.ts:881](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L881)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **members**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **prime**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  timestamp

• **timestamp**: *object*

*Defined in [packages/api/src/augment/query.ts:892](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L892)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **didUpdate**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **now**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  transactionPayment

• **transactionPayment**: *object*

*Defined in [packages/api/src/augment/query.ts:903](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L903)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **nextFeeMultiplier**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **storageVersion**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  treasury

• **treasury**: *object*

*Defined in [packages/api/src/augment/query.ts:908](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L908)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **approvals**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **proposalCount**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **proposals**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **reasons**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

* **tips**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*

___

###  vesting

• **vesting**: *object*

*Defined in [packages/api/src/augment/query.ts:934](https://github.com/polkadot-js/api/blob/b26c7f9f0a/packages/api/src/augment/query.ts#L934)*

#### Type declaration:

* \[ **index**: *string*\]: [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›

* **vesting**: *[AugmentedQuery](../modules/_packages_api_src_types_storage_.md#augmentedquery)‹ApiType, function› & [QueryableStorageEntry](../modules/_packages_api_src_types_storage_.md#queryablestorageentry)‹ApiType›*
