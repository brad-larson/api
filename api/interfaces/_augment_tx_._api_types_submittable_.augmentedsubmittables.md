[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["augment/tx"](../modules/_augment_tx_.md) › ["api/types/submittable"](../modules/_augment_tx_._api_types_submittable_.md) › [AugmentedSubmittables](_augment_tx_._api_types_submittable_.augmentedsubmittables.md)

# Interface: AugmentedSubmittables ‹**ApiType**›

## Type parameters

▪ **ApiType**

## Hierarchy

* **AugmentedSubmittables**

  ↳ [SubmittableExtrinsics](_augment_tx_._api_types_submittable_.submittableextrinsics.md)

## Index

### Properties

* [authorship](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#authorship)
* [balances](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#balances)
* [contracts](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#contracts)
* [council](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#council)
* [democracy](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#democracy)
* [elections](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#elections)
* [finalityTracker](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#finalitytracker)
* [grandpa](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#grandpa)
* [identity](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#identity)
* [imOnline](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#imonline)
* [indices](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#indices)
* [multisig](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#multisig)
* [proxy](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#proxy)
* [recovery](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#recovery)
* [scheduler](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#scheduler)
* [session](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#session)
* [society](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#society)
* [staking](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#staking)
* [sudo](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#sudo)
* [system](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#system)
* [technicalCommittee](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#technicalcommittee)
* [technicalMembership](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#technicalmembership)
* [timestamp](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#timestamp)
* [treasury](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#treasury)
* [utility](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#utility)
* [vesting](_augment_tx_._api_types_submittable_.augmentedsubmittables.md#vesting)

## Properties

###  authorship

• **authorship**: *object*

*Defined in [api/src/augment/tx.ts:27](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L27)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **setUncles**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  balances

• **balances**: *object*

*Defined in [api/src/augment/tx.ts:34](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L34)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **forceTransfer**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setBalance**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **transfer**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **transferKeepAlive**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  contracts

• **contracts**: *object*

*Defined in [api/src/augment/tx.ts:111](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L111)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **call**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **claimSurcharge**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **instantiate**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **putCode**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **updateSchedule**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  council

• **council**: *object*

*Defined in [api/src/augment/tx.ts:156](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L156)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **close**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **disapproveProposal**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **execute**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **propose**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setMembers**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vote**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  democracy

• **democracy**: *object*

*Defined in [api/src/augment/tx.ts:291](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L291)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **cancelQueued**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **cancelReferendum**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **clearPublicProposals**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **delegate**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **emergencyCancel**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **enactProposal**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **externalPropose**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **externalProposeDefault**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **externalProposeMajority**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **fastTrack**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **noteImminentPreimage**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **noteImminentPreimageOperational**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **notePreimage**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **notePreimageOperational**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **propose**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **reapPreimage**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **removeOtherVote**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **removeVote**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **second**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **undelegate**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **unlock**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vetoExternal**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vote**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  elections

• **elections**: *object*

*Defined in [api/src/augment/tx.ts:698](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L698)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **removeMember**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **removeVoter**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **renounceCandidacy**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **reportDefunctVoter**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **submitCandidacy**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vote**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  finalityTracker

• **finalityTracker**: *object*

*Defined in [api/src/augment/tx.ts:861](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L861)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **finalHint**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  grandpa

• **grandpa**: *object*

*Defined in [api/src/augment/tx.ts:869](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L869)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **reportEquivocation**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  identity

• **identity**: *object*

*Defined in [api/src/augment/tx.ts:883](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L883)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **addRegistrar**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **cancelRequest**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **clearIdentity**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **killIdentity**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **provideJudgement**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **requestJudgement**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setAccountId**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setFee**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setFields**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setIdentity**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setSubs**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  imOnline

• **imOnline**: *object*

*Defined in [api/src/augment/tx.ts:1107](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L1107)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **heartbeat**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  indices

• **indices**: *object*

*Defined in [api/src/augment/tx.ts:1123](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L1123)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **claim**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **forceTransfer**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **free**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **freeze**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **transfer**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  multisig

• **multisig**: *object*

*Defined in [api/src/augment/tx.ts:1240](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L1240)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **approveAsMulti**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **asMulti**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **cancelAsMulti**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  proxy

• **proxy**: *object*

*Defined in [api/src/augment/tx.ts:1368](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L1368)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **addProxy**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **anonymous**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **killAnonymous**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **proxy**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **removeProxies**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **removeProxy**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  recovery

• **recovery**: *object*

*Defined in [api/src/augment/tx.ts:1487](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L1487)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **asRecovered**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **cancelRecovered**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **claimRecovery**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **closeRecovery**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **createRecovery**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **initiateRecovery**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **removeRecovery**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setRecovered**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vouchRecovery**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  scheduler

• **scheduler**: *object*

*Defined in [api/src/augment/tx.ts:1689](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L1689)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **cancel**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **cancelNamed**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **schedule**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **scheduleNamed**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  session

• **session**: *object*

*Defined in [api/src/augment/tx.ts:1744](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L1744)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **purgeKeys**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setKeys**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  society

• **society**: *object*

*Defined in [api/src/augment/tx.ts:1779](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L1779)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **bid**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **defenderVote**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **found**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **judgeSuspendedCandidate**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **judgeSuspendedMember**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **payout**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setMaxMembers**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **unbid**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **unfound**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **unvouch**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vote**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vouch**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  staking

• **staking**: *object*

*Defined in [api/src/augment/tx.ts:2099](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L2099)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **bond**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **bondExtra**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **cancelDeferredSlash**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **chill**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **forceNewEra**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **forceNewEraAlways**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **forceNoEras**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **forceUnstake**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **nominate**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **payoutStakers**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **reapStash**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **rebond**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setController**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setHistoryDepth**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setInvulnerables**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setPayee**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setValidatorCount**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **submitElectionSolution**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **submitElectionSolutionUnsigned**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **unbond**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **validate**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **withdrawUnbonded**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  sudo

• **sudo**: *object*

*Defined in [api/src/augment/tx.ts:2559](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L2559)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **setKey**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **sudo**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **sudoAs**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **sudoUncheckedWeight**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  system

• **system**: *object*

*Defined in [api/src/augment/tx.ts:2614](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L2614)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **fillBlock**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **killPrefix**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **killStorage**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **remark**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setChangesTrieConfig**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setCode**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setCodeWithoutChecks**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setHeapPages**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setStorage**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **suicide**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  technicalCommittee

• **technicalCommittee**: *object*

*Defined in [api/src/augment/tx.ts:2728](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L2728)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **close**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **disapproveProposal**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **execute**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **propose**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setMembers**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vote**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  technicalMembership

• **technicalMembership**: *object*

*Defined in [api/src/augment/tx.ts:2863](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L2863)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **addMember**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **changeKey**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **clearPrime**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **removeMember**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **resetMembers**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **setPrime**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **swapMember**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  timestamp

• **timestamp**: *object*

*Defined in [api/src/augment/tx.ts:2909](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L2909)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **set**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  treasury

• **treasury**: *object*

*Defined in [api/src/augment/tx.ts:2933](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L2933)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **approveProposal**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **closeTip**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **proposeSpend**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **rejectProposal**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **reportAwesome**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **retractTip**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **tip**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **tipNew**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  utility

• **utility**: *object*

*Defined in [api/src/augment/tx.ts:3086](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L3086)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **asLimitedSub**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **asSub**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **batch**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

___

###  vesting

• **vesting**: *object*

*Defined in [api/src/augment/tx.ts:3145](https://github.com/polkadot-js/api/blob/503c2b3c63/packages/api/src/augment/tx.ts#L3145)*

#### Type declaration:

* \[ **index**: *string*\]: [SubmittableExtrinsicFunction](_types_submittable_.submittableextrinsicfunction.md)‹ApiType›

* **vest**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vestOther**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*

* **vestedTransfer**: *[AugmentedSubmittable](../modules/_types_submittable_.md#augmentedsubmittable)‹function›*
