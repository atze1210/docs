---
title: Constants
---

The following sections contain the module constants, also known as parameter types. These can only be changed as part of a runtime upgrade. On the api, these are exposed via `api.consts.<module>.<method>`. 

(NOTE: These were generated from a static/snapshot view of a recent default Substrate runtime. Some items may not be available in older nodes, or in any customized implementations.)

- **[alliance](#alliance)**

- **[allianceMotion](#alliancemotion)**

- **[assetConversion](#assetconversion)**

- **[assetRewards](#assetrewards)**

- **[assets](#assets)**

- **[babe](#babe)**

- **[balances](#balances)**

- **[beefy](#beefy)**

- **[bounties](#bounties)**

- **[broker](#broker)**

- **[childBounties](#childbounties)**

- **[contracts](#contracts)**

- **[convictionVoting](#convictionvoting)**

- **[coreFellowship](#corefellowship)**

- **[council](#council)**

- **[delegatedStaking](#delegatedstaking)**

- **[democracy](#democracy)**

- **[electionProviderMultiPhase](#electionprovidermultiphase)**

- **[elections](#elections)**

- **[fastUnstake](#fastunstake)**

- **[grandpa](#grandpa)**

- **[identity](#identity)**

- **[imOnline](#imonline)**

- **[indices](#indices)**

- **[lottery](#lottery)**

- **[messageQueue](#messagequeue)**

- **[mixnet](#mixnet)**

- **[multiBlockMigrations](#multiblockmigrations)**

- **[multisig](#multisig)**

- **[nftFractionalization](#nftfractionalization)**

- **[nfts](#nfts)**

- **[nis](#nis)**

- **[nominationPools](#nominationpools)**

- **[poolAssets](#poolassets)**

- **[proxy](#proxy)**

- **[rankedPolls](#rankedpolls)**

- **[recovery](#recovery)**

- **[referenda](#referenda)**

- **[revive](#revive)**

- **[safeMode](#safemode)**

- **[salary](#salary)**

- **[scheduler](#scheduler)**

- **[society](#society)**

- **[staking](#staking)**

- **[statement](#statement)**

- **[stateTrieMigration](#statetriemigration)**

- **[system](#system)**

- **[technicalCommittee](#technicalcommittee)**

- **[timestamp](#timestamp)**

- **[tips](#tips)**

- **[transactionPayment](#transactionpayment)**

- **[treasury](#treasury)**

- **[txPause](#txpause)**

- **[uniques](#uniques)**

- **[utility](#utility)**

- **[vesting](#vesting)**

- **[voterList](#voterlist)**


___


## alliance
 
### allyDeposit: `u128`
- **interface**: `api.consts.alliance.allyDeposit`
- **summary**:    The deposit required for submitting candidacy. 
 
### maxAnnouncementsCount: `u32`
- **interface**: `api.consts.alliance.maxAnnouncementsCount`
- **summary**:    The maximum number of announcements. 
 
### maxMembersCount: `u32`
- **interface**: `api.consts.alliance.maxMembersCount`
- **summary**:    The maximum number of members per member role. 
 
### maxUnscrupulousItems: `u32`
- **interface**: `api.consts.alliance.maxUnscrupulousItems`
- **summary**:    The maximum number of the unscrupulous items supported by the pallet. 
 
### maxWebsiteUrlLength: `u32`
- **interface**: `api.consts.alliance.maxWebsiteUrlLength`
- **summary**:    The maximum length of a website URL. 

___


## allianceMotion
 
### maxProposalWeight: `SpWeightsWeightV2Weight`
- **interface**: `api.consts.allianceMotion.maxProposalWeight`
- **summary**:    The maximum weight of a dispatch call that can be proposed and executed. 

___


## assetConversion
 
### liquidityWithdrawalFee: `Permill`
- **interface**: `api.consts.assetConversion.liquidityWithdrawalFee`
- **summary**:    A fee to withdraw the liquidity. 
 
### lpFee: `u32`
- **interface**: `api.consts.assetConversion.lpFee`
- **summary**:    A % the liquidity providers will take of every swap. Represents 10ths of a percent. 
 
### maxSwapPathLength: `u32`
- **interface**: `api.consts.assetConversion.maxSwapPathLength`
- **summary**:    The max number of hops in a swap. 
 
### mintMinLiquidity: `u128`
- **interface**: `api.consts.assetConversion.mintMinLiquidity`
- **summary**:    The minimum LP token amount that could be minted. Ameliorates rounding errors. 
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.assetConversion.palletId`
- **summary**:    The pallet's id, used for deriving its sovereign account ID. 
 
### poolSetupFee: `u128`
- **interface**: `api.consts.assetConversion.poolSetupFee`
- **summary**:    A one-time fee to setup the pool. 
 
### poolSetupFeeAsset: `FrameSupportTokensFungibleUnionOfNativeOrWithId`
- **interface**: `api.consts.assetConversion.poolSetupFeeAsset`
- **summary**:    Asset class from [`Config::Assets`] used to pay the [`Config::PoolSetupFee`]. 

___


## assetRewards
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.assetRewards.palletId`
- **summary**:    The pallet's unique identifier, used to derive the pool's account ID. 

   The account ID is derived once during pool creation and stored in the storage. 

___


## assets
 
### approvalDeposit: `u128`
- **interface**: `api.consts.assets.approvalDeposit`
- **summary**:    The amount of funds that must be reserved when creating a new approval. 
 
### assetAccountDeposit: `u128`
- **interface**: `api.consts.assets.assetAccountDeposit`
- **summary**:    The amount of funds that must be reserved for a non-provider asset account to be  maintained. 
 
### assetDeposit: `u128`
- **interface**: `api.consts.assets.assetDeposit`
- **summary**:    The basic amount of funds that must be reserved for an asset. 
 
### metadataDepositBase: `u128`
- **interface**: `api.consts.assets.metadataDepositBase`
- **summary**:    The basic amount of funds that must be reserved when adding metadata to your asset. 
 
### metadataDepositPerByte: `u128`
- **interface**: `api.consts.assets.metadataDepositPerByte`
- **summary**:    The additional funds that must be reserved for the number of bytes you store in your  metadata. 
 
### removeItemsLimit: `u32`
- **interface**: `api.consts.assets.removeItemsLimit`
- **summary**:    Max number of items to destroy per `destroy_accounts` and `destroy_approvals` call. 

   Must be configured to result in a weight that makes each call fit in a block. 
 
### stringLimit: `u32`
- **interface**: `api.consts.assets.stringLimit`
- **summary**:    The maximum length of a name or symbol stored on-chain. 

___


## babe
 
### epochDuration: `u64`
- **interface**: `api.consts.babe.epochDuration`
- **summary**:    The amount of time, in slots, that each epoch should last.  NOTE: Currently it is not possible to change the epoch duration after  the chain has started. Attempting to do so will brick block production. 
 
### expectedBlockTime: `u64`
- **interface**: `api.consts.babe.expectedBlockTime`
- **summary**:    The expected average block time at which BABE should be creating  blocks. Since BABE is probabilistic it is not trivial to figure out  what the expected average block time should be based on the slot  duration and the security parameter `c` (where `1 - c` represents  the probability of a slot being empty). 
 
### maxAuthorities: `u32`
- **interface**: `api.consts.babe.maxAuthorities`
- **summary**:    Max number of authorities allowed 
 
### maxNominators: `u32`
- **interface**: `api.consts.babe.maxNominators`
- **summary**:    The maximum number of nominators for each validator. 

___


## balances
 
### existentialDeposit: `u128`
- **interface**: `api.consts.balances.existentialDeposit`
- **summary**:    The minimum amount required to keep an account open. MUST BE GREATER THAN ZERO! 

   If you *really* need it to be zero, you can enable the feature `insecure_zero_ed` for  this pallet. However, you do so at your own risk: this will open up a major DoS vector.  In case you have multiple sources of provider references, you may also get unexpected  behaviour if you set this to zero. 

   Bottom line: Do yourself a favour and make it at least one! 
 
### maxFreezes: `u32`
- **interface**: `api.consts.balances.maxFreezes`
- **summary**:    The maximum number of individual freeze locks that can exist on an account at any time. 
 
### maxLocks: `u32`
- **interface**: `api.consts.balances.maxLocks`
- **summary**:    The maximum number of locks that should exist on an account.  Not strictly enforced, but used for weight estimation. 

   Use of locks is deprecated in favour of freezes. See `https://github.com/paritytech/substrate/pull/12951/` 
 
### maxReserves: `u32`
- **interface**: `api.consts.balances.maxReserves`
- **summary**:    The maximum number of named reserves that can exist on an account. 

   Use of reserves is deprecated in favour of holds. See `https://github.com/paritytech/substrate/pull/12951/` 

___


## beefy
 
### maxAuthorities: `u32`
- **interface**: `api.consts.beefy.maxAuthorities`
- **summary**:    The maximum number of authorities that can be added. 
 
### maxNominators: `u32`
- **interface**: `api.consts.beefy.maxNominators`
- **summary**:    The maximum number of nominators for each validator. 
 
### maxSetIdSessionEntries: `u64`
- **interface**: `api.consts.beefy.maxSetIdSessionEntries`
- **summary**:    The maximum number of entries to keep in the set id to session index mapping. 

   Since the `SetIdSession` map is only used for validating equivocations this  value should relate to the bonding duration of whatever staking system is  being used (if any). If equivocation handling is not enabled then this value  can be zero. 

___


## bounties
 
### bountyDepositBase: `u128`
- **interface**: `api.consts.bounties.bountyDepositBase`
- **summary**:    The amount held on deposit for placing a bounty proposal. 
 
### bountyDepositPayoutDelay: `u32`
- **interface**: `api.consts.bounties.bountyDepositPayoutDelay`
- **summary**:    The delay period for which a bounty beneficiary need to wait before claim the payout. 
 
### bountyUpdatePeriod: `u32`
- **interface**: `api.consts.bounties.bountyUpdatePeriod`
- **summary**:    The time limit for a curator to act before a bounty expires. 

   The period that starts when a curator is approved, during which they must execute or  update the bounty via `extend_bounty_expiry`. If missed, the bounty expires, and the  curator may be slashed. If `BlockNumberFor::MAX`, bounties stay active indefinitely,  removing the need for `extend_bounty_expiry`. 
 
### bountyValueMinimum: `u128`
- **interface**: `api.consts.bounties.bountyValueMinimum`
- **summary**:    Minimum value for a bounty. 
 
### curatorDepositMax: `Option<u128>`
- **interface**: `api.consts.bounties.curatorDepositMax`
- **summary**:    Maximum amount of funds that should be placed in a deposit for making a proposal. 
 
### curatorDepositMin: `Option<u128>`
- **interface**: `api.consts.bounties.curatorDepositMin`
- **summary**:    Minimum amount of funds that should be placed in a deposit for making a proposal. 
 
### curatorDepositMultiplier: `Permill`
- **interface**: `api.consts.bounties.curatorDepositMultiplier`
- **summary**:    The curator deposit is calculated as a percentage of the curator fee. 

   This deposit has optional upper and lower bounds with `CuratorDepositMax` and  `CuratorDepositMin`. 
 
### dataDepositPerByte: `u128`
- **interface**: `api.consts.bounties.dataDepositPerByte`
- **summary**:    The amount held on deposit per byte within the tip report reason or bounty description. 
 
### maximumReasonLength: `u32`
- **interface**: `api.consts.bounties.maximumReasonLength`
- **summary**:    Maximum acceptable reason length. 

   Benchmarks depend on this value, be sure to update weights file when changing this value 

___


## broker
 
### maxAutoRenewals: `u32`
- **interface**: `api.consts.broker.maxAutoRenewals`
- **summary**:    Given that we are performing all auto-renewals in a single block, it has to be limited. 
 
### maxLeasedCores: `u32`
- **interface**: `api.consts.broker.maxLeasedCores`
- **summary**:    Maximum number of legacy leases. 
 
### maxReservedCores: `u32`
- **interface**: `api.consts.broker.maxReservedCores`
- **summary**:    Maximum number of system cores. 
 
### minimumCreditPurchase: `u128`
- **interface**: `api.consts.broker.minimumCreditPurchase`
- **summary**:    The smallest amount of credits a user can purchase. 

   Needed to prevent spam attacks. 
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.broker.palletId`
- **summary**:    Identifier from which the internal Pot is generated. 
 
### timeslicePeriod: `u32`
- **interface**: `api.consts.broker.timeslicePeriod`
- **summary**:    Number of Relay-chain blocks per timeslice. 

___


## childBounties
 
### childBountyValueMinimum: `u128`
- **interface**: `api.consts.childBounties.childBountyValueMinimum`
- **summary**:    Minimum value for a child-bounty. 
 
### maxActiveChildBountyCount: `u32`
- **interface**: `api.consts.childBounties.maxActiveChildBountyCount`
- **summary**:    Maximum number of child bounties that can be added to a parent bounty. 

___


## contracts
 
### apiVersion: `u16`
- **interface**: `api.consts.contracts.apiVersion`
- **summary**:    The version of the HostFn APIs that are available in the runtime. 

   Only valid value is `()`. 
 
### codeHashLockupDepositPercent: `Perbill`
- **interface**: `api.consts.contracts.codeHashLockupDepositPercent`
- **summary**:    The percentage of the storage deposit that should be held for using a code hash.  Instantiating a contract, or calling [`chain_extension::Ext::lock_delegate_dependency`]  protects the code from being removed. In order to prevent abuse these actions are  protected with a percentage of the code deposit. 
 
### defaultDepositLimit: `u128`
- **interface**: `api.consts.contracts.defaultDepositLimit`
- **summary**:    Fallback value to limit the storage deposit if it's not being set by the caller. 
 
### depositPerByte: `u128`
- **interface**: `api.consts.contracts.depositPerByte`
- **summary**:    The amount of balance a caller has to pay for each byte of storage. 

   #### Note 

   Changing this value for an existing chain might need a storage migration. 
 
### depositPerItem: `u128`
- **interface**: `api.consts.contracts.depositPerItem`
- **summary**:    The amount of balance a caller has to pay for each storage item. 

   #### Note 

   Changing this value for an existing chain might need a storage migration. 
 
### environment: `PalletContractsEnvironment`
- **interface**: `api.consts.contracts.environment`
- **summary**:    Type that bundles together all the runtime configurable interface types. 

   This is not a real config. We just mention the type here as constant so that  its type appears in the metadata. Only valid value is `()`. 
 
### maxCodeLen: `u32`
- **interface**: `api.consts.contracts.maxCodeLen`
- **summary**:    The maximum length of a contract code in bytes. 

   The value should be chosen carefully taking into the account the overall memory limit  your runtime has, as well as the [maximum allowed callstack  depth](#associatedtype.CallStack). Look into the `integrity_test()` for some insights. 
 
### maxDebugBufferLen: `u32`
- **interface**: `api.consts.contracts.maxDebugBufferLen`
- **summary**:    The maximum length of the debug buffer in bytes. 
 
### maxDelegateDependencies: `u32`
- **interface**: `api.consts.contracts.maxDelegateDependencies`
- **summary**:    The maximum number of delegate_dependencies that a contract can lock with  [`chain_extension::Ext::lock_delegate_dependency`]. 
 
### maxStorageKeyLen: `u32`
- **interface**: `api.consts.contracts.maxStorageKeyLen`
- **summary**:    The maximum allowable length in bytes for storage keys. 
 
### maxTransientStorageSize: `u32`
- **interface**: `api.consts.contracts.maxTransientStorageSize`
- **summary**:    The maximum size of the transient storage in bytes.  This includes keys, values, and previous entries used for storage rollback. 
 
### schedule: `PalletContractsSchedule`
- **interface**: `api.consts.contracts.schedule`
- **summary**:    Cost schedule and limits. 
 
### unsafeUnstableInterface: `bool`
- **interface**: `api.consts.contracts.unsafeUnstableInterface`
- **summary**:    Make contract callable functions marked as `#[unstable]` available. 

   Contracts that use `#[unstable]` functions won't be able to be uploaded unless  this is set to `true`. This is only meant for testnets and dev nodes in order to  experiment with new features. 

   #### Warning 

   Do **not** set to `true` on productions chains. 

___


## convictionVoting
 
### maxVotes: `u32`
- **interface**: `api.consts.convictionVoting.maxVotes`
- **summary**:    The maximum number of concurrent votes an account may have. 

   Also used to compute weight, an overly large value can lead to extrinsics with large  weight estimation: see `delegate` for instance. 
 
### voteLockingPeriod: `u32`
- **interface**: `api.consts.convictionVoting.voteLockingPeriod`
- **summary**:    The minimum period of vote locking. 

   It should be no shorter than enactment period to ensure that in the case of an approval,  those successful voters are locked into the consequences that their votes entail. 

___


## coreFellowship
 
### evidenceSize: `u32`
- **interface**: `api.consts.coreFellowship.evidenceSize`
- **summary**:    The maximum size in bytes submitted evidence is allowed to be. 
 
### maxRank: `u32`
- **interface**: `api.consts.coreFellowship.maxRank`
- **summary**:    Represents the highest possible rank in this pallet. 

   Increasing this value is supported, but decreasing it may lead to a broken state. 

___


## council
 
### maxProposalWeight: `SpWeightsWeightV2Weight`
- **interface**: `api.consts.council.maxProposalWeight`
- **summary**:    The maximum weight of a dispatch call that can be proposed and executed. 

___


## delegatedStaking
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.delegatedStaking.palletId`
- **summary**:    Injected identifier for the pallet. 
 
### slashRewardFraction: `Perbill`
- **interface**: `api.consts.delegatedStaking.slashRewardFraction`
- **summary**:    Fraction of the slash that is rewarded to the caller of pending slash to the agent. 

___


## democracy
 
### cooloffPeriod: `u32`
- **interface**: `api.consts.democracy.cooloffPeriod`
- **summary**:    Period in blocks where an external proposal may not be re-submitted after being vetoed. 
 
### enactmentPeriod: `u32`
- **interface**: `api.consts.democracy.enactmentPeriod`
- **summary**:    The period between a proposal being approved and enacted. 

   It should generally be a little more than the unstake period to ensure that  voting stakers have an opportunity to remove themselves from the system in the case  where they are on the losing side of a vote. 
 
### fastTrackVotingPeriod: `u32`
- **interface**: `api.consts.democracy.fastTrackVotingPeriod`
- **summary**:    Minimum voting period allowed for a fast-track referendum. 
 
### instantAllowed: `bool`
- **interface**: `api.consts.democracy.instantAllowed`
- **summary**:    Indicator for whether an emergency origin is even allowed to happen. Some chains may  want to set this permanently to `false`, others may want to condition it on things such  as an upgrade having happened recently. 
 
### launchPeriod: `u32`
- **interface**: `api.consts.democracy.launchPeriod`
- **summary**:    How often (in blocks) new public referenda are launched. 
 
### maxBlacklisted: `u32`
- **interface**: `api.consts.democracy.maxBlacklisted`
- **summary**:    The maximum number of items which can be blacklisted. 
 
### maxDeposits: `u32`
- **interface**: `api.consts.democracy.maxDeposits`
- **summary**:    The maximum number of deposits a public proposal may have at any time. 
 
### maxProposals: `u32`
- **interface**: `api.consts.democracy.maxProposals`
- **summary**:    The maximum number of public proposals that can exist at any time. 
 
### maxVotes: `u32`
- **interface**: `api.consts.democracy.maxVotes`
- **summary**:    The maximum number of votes for an account. 

   Also used to compute weight, an overly big value can  lead to extrinsic with very big weight: see `delegate` for instance. 
 
### minimumDeposit: `u128`
- **interface**: `api.consts.democracy.minimumDeposit`
- **summary**:    The minimum amount to be used as a deposit for a public referendum proposal. 
 
### voteLockingPeriod: `u32`
- **interface**: `api.consts.democracy.voteLockingPeriod`
- **summary**:    The minimum period of vote locking. 

   It should be no shorter than enactment period to ensure that in the case of an approval,  those successful voters are locked into the consequences that their votes entail. 
 
### votingPeriod: `u32`
- **interface**: `api.consts.democracy.votingPeriod`
- **summary**:    How often (in blocks) to check for new votes. 

___


## electionProviderMultiPhase
 
### betterSignedThreshold: `Perbill`
- **interface**: `api.consts.electionProviderMultiPhase.betterSignedThreshold`
- **summary**:    The minimum amount of improvement to the solution score that defines a solution as  "better" in the Signed phase. 
 
### maxWinners: `u32`
- **interface**: `api.consts.electionProviderMultiPhase.maxWinners`
- **summary**:    The maximum number of winners that can be elected by this `ElectionProvider`  implementation. 

   Note: This must always be greater or equal to `T::DataProvider::desired_targets()`. 
 
### minerMaxLength: `u32`
- **interface**: `api.consts.electionProviderMultiPhase.minerMaxLength`
 
### minerMaxVotesPerVoter: `u32`
- **interface**: `api.consts.electionProviderMultiPhase.minerMaxVotesPerVoter`
 
### minerMaxWeight: `SpWeightsWeightV2Weight`
- **interface**: `api.consts.electionProviderMultiPhase.minerMaxWeight`
 
### minerMaxWinners: `u32`
- **interface**: `api.consts.electionProviderMultiPhase.minerMaxWinners`
 
### minerTxPriority: `u64`
- **interface**: `api.consts.electionProviderMultiPhase.minerTxPriority`
- **summary**:    The priority of the unsigned transaction submitted in the unsigned-phase 
 
### offchainRepeat: `u32`
- **interface**: `api.consts.electionProviderMultiPhase.offchainRepeat`
- **summary**:    The repeat threshold of the offchain worker. 

   For example, if it is 5, that means that at least 5 blocks will elapse between attempts  to submit the worker's solution. 
 
### signedDepositByte: `u128`
- **interface**: `api.consts.electionProviderMultiPhase.signedDepositByte`
- **summary**:    Per-byte deposit for a signed solution. 
 
### signedDepositWeight: `u128`
- **interface**: `api.consts.electionProviderMultiPhase.signedDepositWeight`
- **summary**:    Per-weight deposit for a signed solution. 
 
### signedMaxRefunds: `u32`
- **interface**: `api.consts.electionProviderMultiPhase.signedMaxRefunds`
- **summary**:    The maximum amount of unchecked solutions to refund the call fee for. 
 
### signedMaxSubmissions: `u32`
- **interface**: `api.consts.electionProviderMultiPhase.signedMaxSubmissions`
- **summary**:    Maximum number of signed submissions that can be queued. 

   It is best to avoid adjusting this during an election, as it impacts downstream data  structures. In particular, `SignedSubmissionIndices<T>` is bounded on this value. If you  update this value during an election, you _must_ ensure that  `SignedSubmissionIndices.len()` is less than or equal to the new value. Otherwise,  attempts to submit new solutions may cause a runtime panic. 
 
### signedMaxWeight: `SpWeightsWeightV2Weight`
- **interface**: `api.consts.electionProviderMultiPhase.signedMaxWeight`
- **summary**:    Maximum weight of a signed solution. 

   If [`Config::MinerConfig`] is being implemented to submit signed solutions (outside of  this pallet), then [`MinerConfig::solution_weight`] is used to compare against  this value. 
 
### signedRewardBase: `u128`
- **interface**: `api.consts.electionProviderMultiPhase.signedRewardBase`
- **summary**:    Base reward for a signed solution 

___


## elections
 
### candidacyBond: `u128`
- **interface**: `api.consts.elections.candidacyBond`
- **summary**:    How much should be locked up in order to submit one's candidacy. 
 
### desiredMembers: `u32`
- **interface**: `api.consts.elections.desiredMembers`
- **summary**:    Number of members to elect. 
 
### desiredRunnersUp: `u32`
- **interface**: `api.consts.elections.desiredRunnersUp`
- **summary**:    Number of runners_up to keep. 
 
### maxCandidates: `u32`
- **interface**: `api.consts.elections.maxCandidates`
- **summary**:    The maximum number of candidates in a phragmen election. 

   Warning: This impacts the size of the election which is run onchain. Chose wisely, and  consider how it will impact `T::WeightInfo::election_phragmen`. 

   When this limit is reached no more candidates are accepted in the election. 
 
### maxVoters: `u32`
- **interface**: `api.consts.elections.maxVoters`
- **summary**:    The maximum number of voters to allow in a phragmen election. 

   Warning: This impacts the size of the election which is run onchain. Chose wisely, and  consider how it will impact `T::WeightInfo::election_phragmen`. 

   When the limit is reached the new voters are ignored. 
 
### maxVotesPerVoter: `u32`
- **interface**: `api.consts.elections.maxVotesPerVoter`
- **summary**:    Maximum numbers of votes per voter. 

   Warning: This impacts the size of the election which is run onchain. Chose wisely, and  consider how it will impact `T::WeightInfo::election_phragmen`. 
 
### palletId: `[u8;8]`
- **interface**: `api.consts.elections.palletId`
- **summary**:    Identifier for the elections-phragmen pallet's lock 
 
### termDuration: `u32`
- **interface**: `api.consts.elections.termDuration`
- **summary**:    How long each seat is kept. This defines the next block number at which an election  round will happen. If set to zero, no elections are ever triggered and the module will  be in passive mode. 
 
### votingBondBase: `u128`
- **interface**: `api.consts.elections.votingBondBase`
- **summary**:    Base deposit associated with voting. 

   This should be sensibly high to economically ensure the pallet cannot be attacked by  creating a gigantic number of votes. 
 
### votingBondFactor: `u128`
- **interface**: `api.consts.elections.votingBondFactor`
- **summary**:    The amount of bond that need to be locked for each vote (32 bytes). 

___


## fastUnstake
 
### deposit: `u128`
- **interface**: `api.consts.fastUnstake.deposit`
- **summary**:    Deposit to take for unstaking, to make sure we're able to slash the it in order to cover  the costs of resources on unsuccessful unstake. 

___


## grandpa
 
### maxAuthorities: `u32`
- **interface**: `api.consts.grandpa.maxAuthorities`
- **summary**:    Max Authorities in use 
 
### maxNominators: `u32`
- **interface**: `api.consts.grandpa.maxNominators`
- **summary**:    The maximum number of nominators for each validator. 
 
### maxSetIdSessionEntries: `u64`
- **interface**: `api.consts.grandpa.maxSetIdSessionEntries`
- **summary**:    The maximum number of entries to keep in the set id to session index mapping. 

   Since the `SetIdSession` map is only used for validating equivocations this  value should relate to the bonding duration of whatever staking system is  being used (if any). If equivocation handling is not enabled then this value  can be zero. 

___


## identity
 
### basicDeposit: `u128`
- **interface**: `api.consts.identity.basicDeposit`
- **summary**:    The amount held on deposit for a registered identity. 
 
### byteDeposit: `u128`
- **interface**: `api.consts.identity.byteDeposit`
- **summary**:    The amount held on deposit per encoded byte for a registered identity. 
 
### maxRegistrars: `u32`
- **interface**: `api.consts.identity.maxRegistrars`
- **summary**:    Maximum number of registrars allowed in the system. Needed to bound the complexity  of, e.g., updating judgements. 
 
### maxSubAccounts: `u32`
- **interface**: `api.consts.identity.maxSubAccounts`
- **summary**:    The maximum number of sub-accounts allowed per identified account. 
 
### maxSuffixLength: `u32`
- **interface**: `api.consts.identity.maxSuffixLength`
- **summary**:    The maximum length of a suffix. 
 
### maxUsernameLength: `u32`
- **interface**: `api.consts.identity.maxUsernameLength`
- **summary**:    The maximum length of a username, including its suffix and any system-added delimiters. 
 
### pendingUsernameExpiration: `u32`
- **interface**: `api.consts.identity.pendingUsernameExpiration`
- **summary**:    The number of blocks within which a username grant must be accepted. 
 
### subAccountDeposit: `u128`
- **interface**: `api.consts.identity.subAccountDeposit`
- **summary**:    The amount held on deposit for a registered subaccount. This should account for the fact  that one storage item's value will increase by the size of an account ID, and there will  be another trie item whose value is the size of an account ID plus 32 bytes. 
 
### usernameDeposit: `u128`
- **interface**: `api.consts.identity.usernameDeposit`
- **summary**:    The amount held on deposit per registered username. This value should change only in  runtime upgrades with proper migration of existing deposits. 
 
### usernameGracePeriod: `u32`
- **interface**: `api.consts.identity.usernameGracePeriod`
- **summary**:    The number of blocks that must pass to enable the permanent deletion of a username by  its respective authority. 

___


## imOnline
 
### unsignedPriority: `u64`
- **interface**: `api.consts.imOnline.unsignedPriority`
- **summary**:    A configuration for base priority of unsigned transactions. 

   This is exposed so that it can be tuned for particular runtime, when  multiple pallets send unsigned transactions. 

___


## indices
 
### deposit: `u128`
- **interface**: `api.consts.indices.deposit`
- **summary**:    The deposit needed for reserving an index. 

___


## lottery
 
### maxCalls: `u32`
- **interface**: `api.consts.lottery.maxCalls`
- **summary**:    The max number of calls available in a single lottery. 
 
### maxGenerateRandom: `u32`
- **interface**: `api.consts.lottery.maxGenerateRandom`
- **summary**:    Number of time we should try to generate a random number that has no modulo bias.  The larger this number, the more potential computation is used for picking the winner,  but also the more likely that the chosen winner is done fairly. 
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.lottery.palletId`
- **summary**:    The Lottery's pallet id 

___


## messageQueue
 
### heapSize: `u32`
- **interface**: `api.consts.messageQueue.heapSize`
- **summary**:    The size of the page; this implies the maximum message size which can be sent. 

   A good value depends on the expected message sizes, their weights, the weight that is  available for processing them and the maximal needed message size. The maximal message  size is slightly lower than this as defined by [`MaxMessageLenOf`]. 
 
### idleMaxServiceWeight: `Option<SpWeightsWeightV2Weight>`
- **interface**: `api.consts.messageQueue.idleMaxServiceWeight`
- **summary**:    The maximum amount of weight (if any) to be used from remaining weight `on_idle` which  should be provided to the message queue for servicing enqueued items `on_idle`.  Useful for parachains to process messages at the same block they are received. 

   If `None`, it will not call `ServiceQueues::service_queues` in `on_idle`. 
 
### maxStale: `u32`
- **interface**: `api.consts.messageQueue.maxStale`
- **summary**:    The maximum number of stale pages (i.e. of overweight messages) allowed before culling  can happen. Once there are more stale pages than this, then historical pages may be  dropped, even if they contain unprocessed overweight messages. 
 
### serviceWeight: `Option<SpWeightsWeightV2Weight>`
- **interface**: `api.consts.messageQueue.serviceWeight`
- **summary**:    The amount of weight (if any) which should be provided to the message queue for  servicing enqueued items `on_initialize`. 

   This may be legitimately `None` in the case that you will call  `ServiceQueues::service_queues` manually or set [`Self::IdleMaxServiceWeight`] to have  it run in `on_idle`. 

___


## mixnet
 
### maxAuthorities: `u32`
- **interface**: `api.consts.mixnet.maxAuthorities`
- **summary**:    The maximum number of authorities per session. 
 
### maxExternalAddressesPerMixnode: `u32`
- **interface**: `api.consts.mixnet.maxExternalAddressesPerMixnode`
- **summary**:    The maximum number of external addresses for a mixnode. 
 
### maxExternalAddressSize: `u32`
- **interface**: `api.consts.mixnet.maxExternalAddressSize`
- **summary**:    The maximum size of one of a mixnode's external addresses. 
 
### minMixnodes: `u32`
- **interface**: `api.consts.mixnet.minMixnodes`
- **summary**:    Minimum number of mixnodes. If there are fewer than this many mixnodes registered for a  session, the mixnet will not be active during the session. 
 
### numCoverToCurrentBlocks: `u32`
- **interface**: `api.consts.mixnet.numCoverToCurrentBlocks`
- **summary**:    Length of the first phase of each session (`CoverToCurrent`), in blocks. 
 
### numCoverToPrevBlocks: `u32`
- **interface**: `api.consts.mixnet.numCoverToPrevBlocks`
- **summary**:    Length of the third phase of each session (`CoverToPrev`), in blocks. 
 
### numRegisterEndSlackBlocks: `u32`
- **interface**: `api.consts.mixnet.numRegisterEndSlackBlocks`
- **summary**:    The number of "slack" blocks at the end of each session.  [`maybe_register`](Pallet::maybe_register) will try to register before this slack  period, but may post registration transactions during the slack period as a last  resort. 
 
### numRegisterStartSlackBlocks: `u32`
- **interface**: `api.consts.mixnet.numRegisterStartSlackBlocks`
- **summary**:    The number of "slack" blocks at the start of each session, during which  [`maybe_register`](Pallet::maybe_register) will not attempt to post registration  transactions. 
 
### numRequestsToCurrentBlocks: `u32`
- **interface**: `api.consts.mixnet.numRequestsToCurrentBlocks`
- **summary**:    Length of the second phase of each session (`RequestsToCurrent`), in blocks. 
 
### registrationPriority: `u64`
- **interface**: `api.consts.mixnet.registrationPriority`
- **summary**:    Priority of unsigned transactions used to register mixnodes. 

___


## multiBlockMigrations
 
### cursorMaxLen: `u32`
- **interface**: `api.consts.multiBlockMigrations.cursorMaxLen`
- **summary**:    The maximal length of an encoded cursor. 

   A good default needs to selected such that no migration will ever have a cursor with MEL  above this limit. This is statically checked in `integrity_test`. 
 
### identifierMaxLen: `u32`
- **interface**: `api.consts.multiBlockMigrations.identifierMaxLen`
- **summary**:    The maximal length of an encoded identifier. 

   A good default needs to selected such that no migration will ever have an identifier  with MEL above this limit. This is statically checked in `integrity_test`. 

___


## multisig
 
### depositBase: `u128`
- **interface**: `api.consts.multisig.depositBase`
- **summary**:    The base amount of currency needed to reserve for creating a multisig execution or to  store a dispatch call for later. 

   This is held for an additional storage item whose value size is  `4 + sizeof((BlockNumber, Balance, AccountId))` bytes and whose key size is  `32 + sizeof(AccountId)` bytes. 
 
### depositFactor: `u128`
- **interface**: `api.consts.multisig.depositFactor`
- **summary**:    The amount of currency needed per unit threshold when creating a multisig execution. 

   This is held for adding 32 bytes more into a pre-existing storage value. 
 
### maxSignatories: `u32`
- **interface**: `api.consts.multisig.maxSignatories`
- **summary**:    The maximum amount of signatories allowed in the multisig. 

___


## nftFractionalization
 
### deposit: `u128`
- **interface**: `api.consts.nftFractionalization.deposit`
- **summary**:    The deposit paid by the user locking an NFT. The deposit is returned to the original NFT  owner when the asset is unified and the NFT is unlocked. 
 
### newAssetName: `Bytes`
- **interface**: `api.consts.nftFractionalization.newAssetName`
- **summary**:    The newly created asset's name. 
 
### newAssetSymbol: `Bytes`
- **interface**: `api.consts.nftFractionalization.newAssetSymbol`
- **summary**:    The newly created asset's symbol. 
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.nftFractionalization.palletId`
- **summary**:    The pallet's id, used for deriving its sovereign account ID. 
 
### stringLimit: `u32`
- **interface**: `api.consts.nftFractionalization.stringLimit`
- **summary**:    The maximum length of a name or symbol stored on-chain. 

___


## nfts
 
### approvalsLimit: `u32`
- **interface**: `api.consts.nfts.approvalsLimit`
- **summary**:    The maximum approvals an item could have. 
 
### attributeDepositBase: `u128`
- **interface**: `api.consts.nfts.attributeDepositBase`
- **summary**:    The basic amount of funds that must be reserved when adding an attribute to an item. 
 
### collectionDeposit: `u128`
- **interface**: `api.consts.nfts.collectionDeposit`
- **summary**:    The basic amount of funds that must be reserved for collection. 
 
### depositPerByte: `u128`
- **interface**: `api.consts.nfts.depositPerByte`
- **summary**:    The additional funds that must be reserved for the number of bytes store in metadata,  either "normal" metadata or attribute metadata. 
 
### features: `u64`
- **interface**: `api.consts.nfts.features`
- **summary**:    Disables some of pallet's features. 
 
### itemAttributesApprovalsLimit: `u32`
- **interface**: `api.consts.nfts.itemAttributesApprovalsLimit`
- **summary**:    The maximum attributes approvals an item could have. 
 
### itemDeposit: `u128`
- **interface**: `api.consts.nfts.itemDeposit`
- **summary**:    The basic amount of funds that must be reserved for an item. 
 
### keyLimit: `u32`
- **interface**: `api.consts.nfts.keyLimit`
- **summary**:    The maximum length of an attribute key. 
 
### maxAttributesPerCall: `u32`
- **interface**: `api.consts.nfts.maxAttributesPerCall`
- **summary**:    The max number of attributes a user could set per call. 
 
### maxDeadlineDuration: `u32`
- **interface**: `api.consts.nfts.maxDeadlineDuration`
- **summary**:    The max duration in blocks for deadlines. 
 
### maxTips: `u32`
- **interface**: `api.consts.nfts.maxTips`
- **summary**:    The max number of tips a user could send. 
 
### metadataDepositBase: `u128`
- **interface**: `api.consts.nfts.metadataDepositBase`
- **summary**:    The basic amount of funds that must be reserved when adding metadata to your item. 
 
### stringLimit: `u32`
- **interface**: `api.consts.nfts.stringLimit`
- **summary**:    The maximum length of data stored on-chain. 
 
### valueLimit: `u32`
- **interface**: `api.consts.nfts.valueLimit`
- **summary**:    The maximum length of an attribute value. 

___


## nis
 
### basePeriod: `u32`
- **interface**: `api.consts.nis.basePeriod`
- **summary**:    The base period for the duration queues. This is the common multiple across all  supported freezing durations that can be bid upon. 
 
### fifoQueueLen: `u32`
- **interface**: `api.consts.nis.fifoQueueLen`
- **summary**:    Portion of the queue which is free from ordering and just a FIFO. 

   Must be no greater than `MaxQueueLen`. 
 
### intakePeriod: `u32`
- **interface**: `api.consts.nis.intakePeriod`
- **summary**:    The number of blocks between consecutive attempts to dequeue bids and create receipts. 

   A larger value results in fewer storage hits each block, but a slower period to get to  the target. 
 
### maxIntakeWeight: `SpWeightsWeightV2Weight`
- **interface**: `api.consts.nis.maxIntakeWeight`
- **summary**:    The maximum amount of bids that can consolidated into receipts in a single intake. A  larger value here means less of the block available for transactions should there be a  glut of bids. 
 
### maxQueueLen: `u32`
- **interface**: `api.consts.nis.maxQueueLen`
- **summary**:    Maximum number of items that may be in each duration queue. 

   Must be larger than zero. 
 
### minBid: `u128`
- **interface**: `api.consts.nis.minBid`
- **summary**:    The minimum amount of funds that may be placed in a bid. Note that this  does not actually limit the amount which may be represented in a receipt since bids may  be split up by the system. 

   It should be at least big enough to ensure that there is no possible storage spam attack  or queue-filling attack. 
 
### minReceipt: `Perquintill`
- **interface**: `api.consts.nis.minReceipt`
- **summary**:    The minimum amount of funds which may intentionally be left remaining under a single  receipt. 
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.nis.palletId`
- **summary**:    The treasury's pallet id, used for deriving its sovereign account ID. 
 
### queueCount: `u32`
- **interface**: `api.consts.nis.queueCount`
- **summary**:    Number of duration queues in total. This sets the maximum duration supported, which is  this value multiplied by `Period`. 
 
### thawThrottle: `(Perquintill,u32)`
- **interface**: `api.consts.nis.thawThrottle`
- **summary**:    The maximum proportion which may be thawed and the period over which it is reset. 

___


## nominationPools
 
### maxPointsToBalance: `u8`
- **interface**: `api.consts.nominationPools.maxPointsToBalance`
- **summary**:    The maximum pool points-to-balance ratio that an `open` pool can have. 

   This is important in the event slashing takes place and the pool's points-to-balance  ratio becomes disproportional. 

   Moreover, this relates to the `RewardCounter` type as well, as the arithmetic operations  are a function of number of points, and by setting this value to e.g. 10, you ensure  that the total number of points in the system are at most 10 times the total_issuance of  the chain, in the absolute worse case. 

   For a value of 10, the threshold would be a pool points-to-balance ratio of 10:1.  Such a scenario would also be the equivalent of the pool being 90% slashed. 
 
### maxUnbonding: `u32`
- **interface**: `api.consts.nominationPools.maxUnbonding`
- **summary**:    The maximum number of simultaneous unbonding chunks that can exist per member. 
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.nominationPools.palletId`
- **summary**:    The nomination pool's pallet id. 

___


## poolAssets
 
### approvalDeposit: `u128`
- **interface**: `api.consts.poolAssets.approvalDeposit`
- **summary**:    The amount of funds that must be reserved when creating a new approval. 
 
### assetAccountDeposit: `u128`
- **interface**: `api.consts.poolAssets.assetAccountDeposit`
- **summary**:    The amount of funds that must be reserved for a non-provider asset account to be  maintained. 
 
### assetDeposit: `u128`
- **interface**: `api.consts.poolAssets.assetDeposit`
- **summary**:    The basic amount of funds that must be reserved for an asset. 
 
### metadataDepositBase: `u128`
- **interface**: `api.consts.poolAssets.metadataDepositBase`
- **summary**:    The basic amount of funds that must be reserved when adding metadata to your asset. 
 
### metadataDepositPerByte: `u128`
- **interface**: `api.consts.poolAssets.metadataDepositPerByte`
- **summary**:    The additional funds that must be reserved for the number of bytes you store in your  metadata. 
 
### removeItemsLimit: `u32`
- **interface**: `api.consts.poolAssets.removeItemsLimit`
- **summary**:    Max number of items to destroy per `destroy_accounts` and `destroy_approvals` call. 

   Must be configured to result in a weight that makes each call fit in a block. 
 
### stringLimit: `u32`
- **interface**: `api.consts.poolAssets.stringLimit`
- **summary**:    The maximum length of a name or symbol stored on-chain. 

___


## proxy
 
### announcementDepositBase: `u128`
- **interface**: `api.consts.proxy.announcementDepositBase`
- **summary**:    The base amount of currency needed to reserve for creating an announcement. 

   This is held when a new storage item holding a `Balance` is created (typically 16  bytes). 
 
### announcementDepositFactor: `u128`
- **interface**: `api.consts.proxy.announcementDepositFactor`
- **summary**:    The amount of currency needed per announcement made. 

   This is held for adding an `AccountId`, `Hash` and `BlockNumber` (typically 68 bytes)  into a pre-existing storage value. 
 
### maxPending: `u32`
- **interface**: `api.consts.proxy.maxPending`
- **summary**:    The maximum amount of time-delayed announcements that are allowed to be pending. 
 
### maxProxies: `u32`
- **interface**: `api.consts.proxy.maxProxies`
- **summary**:    The maximum amount of proxies allowed for a single account. 
 
### proxyDepositBase: `u128`
- **interface**: `api.consts.proxy.proxyDepositBase`
- **summary**:    The base amount of currency needed to reserve for creating a proxy. 

   This is held for an additional storage item whose value size is  `sizeof(Balance)` bytes and whose key size is `sizeof(AccountId)` bytes. 
 
### proxyDepositFactor: `u128`
- **interface**: `api.consts.proxy.proxyDepositFactor`
- **summary**:    The amount of currency needed per proxy added. 

   This is held for adding 32 bytes plus an instance of `ProxyType` more into a  pre-existing storage value. Thus, when configuring `ProxyDepositFactor` one should take  into account `32 + proxy_type.encode().len()` bytes of data. 

___


## rankedPolls
 
### alarmInterval: `u32`
- **interface**: `api.consts.rankedPolls.alarmInterval`
- **summary**:    Quantization level for the referendum wakeup scheduler. A higher number will result in  fewer storage reads/writes needed for smaller voters, but also result in delays to the  automatic referendum status changes. Explicit servicing instructions are unaffected. 
 
### maxQueued: `u32`
- **interface**: `api.consts.rankedPolls.maxQueued`
- **summary**:    Maximum size of the referendum queue for a single track. 
 
### submissionDeposit: `u128`
- **interface**: `api.consts.rankedPolls.submissionDeposit`
- **summary**:    The minimum amount to be used as a deposit for a public referendum proposal. 
 
### tracks: `Vec<(u16,PalletReferendaTrackDetails)>`
- **interface**: `api.consts.rankedPolls.tracks`
- **summary**:    A list of tracks. 

   Note: if the tracks are dynamic, the value in the static metadata might be inaccurate. 
 
### undecidingTimeout: `u32`
- **interface**: `api.consts.rankedPolls.undecidingTimeout`
- **summary**:    The number of blocks after submission that a referendum must begin being decided by.  Once this passes, then anyone may cancel the referendum. 

___


## recovery
 
### configDepositBase: `u128`
- **interface**: `api.consts.recovery.configDepositBase`
- **summary**:    The base amount of currency needed to reserve for creating a recovery configuration. 

   This is held for an additional storage item whose value size is  `2 + sizeof(BlockNumber, Balance)` bytes. 
 
### friendDepositFactor: `u128`
- **interface**: `api.consts.recovery.friendDepositFactor`
- **summary**:    The amount of currency needed per additional user when creating a recovery  configuration. 

   This is held for adding `sizeof(AccountId)` bytes more into a pre-existing storage  value. 
 
### maxFriends: `u32`
- **interface**: `api.consts.recovery.maxFriends`
- **summary**:    The maximum amount of friends allowed in a recovery configuration. 

   NOTE: The threshold programmed in this Pallet uses u16, so it does  not really make sense to have a limit here greater than u16::MAX.  But also, that is a lot more than you should probably set this value  to anyway... 
 
### recoveryDeposit: `u128`
- **interface**: `api.consts.recovery.recoveryDeposit`
- **summary**:    The base amount of currency needed to reserve for starting a recovery. 

   This is primarily held for deterring malicious recovery attempts, and should  have a value large enough that a bad actor would choose not to place this  deposit. It also acts to fund additional storage item whose value size is  `sizeof(BlockNumber, Balance + T * AccountId)` bytes. Where T is a configurable  threshold. 

___


## referenda
 
### alarmInterval: `u32`
- **interface**: `api.consts.referenda.alarmInterval`
- **summary**:    Quantization level for the referendum wakeup scheduler. A higher number will result in  fewer storage reads/writes needed for smaller voters, but also result in delays to the  automatic referendum status changes. Explicit servicing instructions are unaffected. 
 
### maxQueued: `u32`
- **interface**: `api.consts.referenda.maxQueued`
- **summary**:    Maximum size of the referendum queue for a single track. 
 
### submissionDeposit: `u128`
- **interface**: `api.consts.referenda.submissionDeposit`
- **summary**:    The minimum amount to be used as a deposit for a public referendum proposal. 
 
### tracks: `Vec<(u16,PalletReferendaTrackDetails)>`
- **interface**: `api.consts.referenda.tracks`
- **summary**:    A list of tracks. 

   Note: if the tracks are dynamic, the value in the static metadata might be inaccurate. 
 
### undecidingTimeout: `u32`
- **interface**: `api.consts.referenda.undecidingTimeout`
- **summary**:    The number of blocks after submission that a referendum must begin being decided by.  Once this passes, then anyone may cancel the referendum. 

___


## revive
 
### chainId: `u64`
- **interface**: `api.consts.revive.chainId`
- **summary**:    The [EIP-155](https://eips.ethereum.org/EIPS/eip-155) chain ID. 

   This is a unique identifier assigned to each blockchain network,  preventing replay attacks. 
 
### codeHashLockupDepositPercent: `Perbill`
- **interface**: `api.consts.revive.codeHashLockupDepositPercent`
- **summary**:    The percentage of the storage deposit that should be held for using a code hash.  Instantiating a contract, protects the code from being removed. In order to prevent  abuse these actions are protected with a percentage of the code deposit. 
 
### depositPerByte: `u128`
- **interface**: `api.consts.revive.depositPerByte`
- **summary**:    The amount of balance a caller has to pay for each byte of storage. 

   #### Note 

   It is safe to change this value on a live chain as all refunds are pro rata. 
 
### depositPerItem: `u128`
- **interface**: `api.consts.revive.depositPerItem`
- **summary**:    The amount of balance a caller has to pay for each storage item. 

   #### Note 

   It is safe to change this value on a live chain as all refunds are pro rata. 
 
### nativeToEthRatio: `u32`
- **interface**: `api.consts.revive.nativeToEthRatio`
- **summary**:    The ratio between the decimal representation of the native token and the ETH token. 
 
### unsafeUnstableInterface: `bool`
- **interface**: `api.consts.revive.unsafeUnstableInterface`
- **summary**:    Make contract callable functions marked as `#[unstable]` available. 

   Contracts that use `#[unstable]` functions won't be able to be uploaded unless  this is set to `true`. This is only meant for testnets and dev nodes in order to  experiment with new features. 

   #### Warning 

   Do **not** set to `true` on productions chains. 

___


## safeMode
 
### enterDepositAmount: `Option<u128>`
- **interface**: `api.consts.safeMode.enterDepositAmount`
- **summary**:    The amount that will be reserved upon calling [`Pallet::enter`]. 

   `None` disallows permissionlessly enabling the safe-mode and is a sane default. 
 
### enterDuration: `u32`
- **interface**: `api.consts.safeMode.enterDuration`
- **summary**:    For how many blocks the safe-mode will be entered by [`Pallet::enter`]. 
 
### extendDepositAmount: `Option<u128>`
- **interface**: `api.consts.safeMode.extendDepositAmount`
- **summary**:    The amount that will be reserved upon calling [`Pallet::extend`]. 

   `None` disallows permissionlessly extending the safe-mode and is a sane default. 
 
### extendDuration: `u32`
- **interface**: `api.consts.safeMode.extendDuration`
- **summary**:    For how many blocks the safe-mode can be extended by each [`Pallet::extend`] call. 

   This does not impose a hard limit as the safe-mode can be extended multiple times. 
 
### releaseDelay: `Option<u32>`
- **interface**: `api.consts.safeMode.releaseDelay`
- **summary**:    The minimal duration a deposit will remain reserved after safe-mode is entered or  extended, unless [`Pallet::force_release_deposit`] is successfully called sooner. 

   Every deposit is tied to a specific activation or extension, thus each deposit can be  released independently after the delay for it has passed. 

   `None` disallows permissionlessly releasing the safe-mode deposits and is a sane  default. 

___


## salary
 
### budget: `u128`
- **interface**: `api.consts.salary.budget`
- **summary**:    The total budget per cycle. 

   This may change over the course of a cycle without any problem. 
 
### payoutPeriod: `u32`
- **interface**: `api.consts.salary.payoutPeriod`
- **summary**:    The number of blocks within a cycle which accounts have to claim the payout. 

   The number of blocks between sequential payout cycles is the sum of this and  `RegistrationPeriod`. 
 
### registrationPeriod: `u32`
- **interface**: `api.consts.salary.registrationPeriod`
- **summary**:    The number of blocks within a cycle which accounts have to register their intent to  claim. 

   The number of blocks between sequential payout cycles is the sum of this and  `PayoutPeriod`. 

___


## scheduler
 
### maximumWeight: `SpWeightsWeightV2Weight`
- **interface**: `api.consts.scheduler.maximumWeight`
- **summary**:    The maximum weight that may be scheduled per block for any dispatchables. 
 
### maxScheduledPerBlock: `u32`
- **interface**: `api.consts.scheduler.maxScheduledPerBlock`
- **summary**:    The maximum number of scheduled calls in the queue for a single block. 

   NOTE:  + Dependent pallets' benchmarks might require a higher limit for the setting. Set a  higher limit under `runtime-benchmarks` feature. 

___


## society
 
### challengePeriod: `u32`
- **interface**: `api.consts.society.challengePeriod`
- **summary**:    The number of blocks between membership challenges. 
 
### claimPeriod: `u32`
- **interface**: `api.consts.society.claimPeriod`
- **summary**:    The number of blocks on which new candidates can claim their membership and be the  named head. 
 
### graceStrikes: `u32`
- **interface**: `api.consts.society.graceStrikes`
- **summary**:    The maximum number of strikes before a member gets funds slashed. 
 
### maxBids: `u32`
- **interface**: `api.consts.society.maxBids`
- **summary**:    The maximum number of bids at once. 
 
### maxLockDuration: `u32`
- **interface**: `api.consts.society.maxLockDuration`
- **summary**:    The maximum duration of the payout lock. 
 
### maxPayouts: `u32`
- **interface**: `api.consts.society.maxPayouts`
- **summary**:    The maximum number of payouts a member may have waiting unclaimed. 
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.society.palletId`
- **summary**:    The societies's pallet id 
 
### periodSpend: `u128`
- **interface**: `api.consts.society.periodSpend`
- **summary**:    The amount of incentive paid within each period. Doesn't include VoterTip. 
 
### votingPeriod: `u32`
- **interface**: `api.consts.society.votingPeriod`
- **summary**:    The number of blocks on which new candidates should be voted on. Together with  `ClaimPeriod`, this sums to the number of blocks between candidate intake periods. 

___


## staking
 
### bondingDuration: `u32`
- **interface**: `api.consts.staking.bondingDuration`
- **summary**:    Number of eras that staked funds must remain bonded for. 
 
### historyDepth: `u32`
- **interface**: `api.consts.staking.historyDepth`
- **summary**:    Number of eras to keep in history. 

   Following information is kept for eras in `[current_era -  HistoryDepth, current_era]`: `ErasStakers`, `ErasStakersClipped`,  `ErasValidatorPrefs`, `ErasValidatorReward`, `ErasRewardPoints`,  `ErasTotalStake`, `ErasStartSessionIndex`, `ClaimedRewards`, `ErasStakersPaged`,  `ErasStakersOverview`. 

   Must be more than the number of eras delayed by session.  I.e. active era must always be in history. I.e. `active_era >  current_era - history_depth` must be guaranteed. 

   If migrating an existing pallet from storage value to config value,  this should be set to same value or greater as in storage. 

   Note: `HistoryDepth` is used as the upper bound for the `BoundedVec`  item `StakingLedger.legacy_claimed_rewards`. Setting this value lower than  the existing value can lead to inconsistencies in the  `StakingLedger` and will need to be handled properly in a migration.  The test `reducing_history_depth_abrupt` shows this effect. 
 
### maxExposurePageSize: `u32`
- **interface**: `api.consts.staking.maxExposurePageSize`
- **summary**:    The maximum size of each `T::ExposurePage`. 

   An `ExposurePage` is weakly bounded to a maximum of `MaxExposurePageSize`  nominators. 

   For older non-paged exposure, a reward payout was restricted to the top  `MaxExposurePageSize` nominators. This is to limit the i/o cost for the  nominator payout. 

   Note: `MaxExposurePageSize` is used to bound `ClaimedRewards` and is unsafe to reduce  without handling it in a migration. 
 
### maxUnlockingChunks: `u32`
- **interface**: `api.consts.staking.maxUnlockingChunks`
- **summary**:    The maximum number of `unlocking` chunks a [`StakingLedger`] can  have. Effectively determines how many unique eras a staker may be  unbonding in. 

   Note: `MaxUnlockingChunks` is used as the upper bound for the  `BoundedVec` item `StakingLedger.unlocking`. Setting this value  lower than the existing value can lead to inconsistencies in the  `StakingLedger` and will need to be handled properly in a runtime  migration. The test `reducing_max_unlocking_chunks_abrupt` shows  this effect. 
 
### sessionsPerEra: `u32`
- **interface**: `api.consts.staking.sessionsPerEra`
- **summary**:    Number of sessions per era. 
 
### slashDeferDuration: `u32`
- **interface**: `api.consts.staking.slashDeferDuration`
- **summary**:    Number of eras that slashes are deferred by, after computation. 

   This should be less than the bonding duration. Set to 0 if slashes  should be applied immediately, without opportunity for intervention. 

___


## statement
 
### byteCost: `u128`
- **interface**: `api.consts.statement.byteCost`
- **summary**:    Cost of data byte used for priority calculation. 
 
### maxAllowedBytes: `u32`
- **interface**: `api.consts.statement.maxAllowedBytes`
- **summary**:    Maximum data bytes allowed per account. 
 
### maxAllowedStatements: `u32`
- **interface**: `api.consts.statement.maxAllowedStatements`
- **summary**:    Maximum number of statements allowed per account. 
 
### minAllowedBytes: `u32`
- **interface**: `api.consts.statement.minAllowedBytes`
- **summary**:    Minimum data bytes allowed per account. 
 
### minAllowedStatements: `u32`
- **interface**: `api.consts.statement.minAllowedStatements`
- **summary**:    Minimum number of statements allowed per account. 
 
### statementCost: `u128`
- **interface**: `api.consts.statement.statementCost`
- **summary**:    Min balance for priority statements. 

___


## stateTrieMigration
 
### maxKeyLen: `u32`
- **interface**: `api.consts.stateTrieMigration.maxKeyLen`
- **summary**:    Maximal number of bytes that a key can have. 

   FRAME itself does not limit the key length.  The concrete value must therefore depend on your storage usage.  A [`frame_support::storage::StorageNMap`] for example can have an arbitrary number of  keys which are then hashed and concatenated, resulting in arbitrarily long keys. 

   Use the *state migration RPC* to retrieve the length of the longest key in your  storage: <https://github.com/paritytech/substrate/issues/11642> 

   The migration will halt with a `Halted` event if this value is too small.  Since there is no real penalty from over-estimating, it is advised to use a large  value. The default is 512 byte. 

   Some key lengths for reference: 

  - [`frame_support::storage::StorageValue`]: 32 byte

  - [`frame_support::storage::StorageMap`]: 64 byte

  - [`frame_support::storage::StorageDoubleMap`]: 96 byte

   For more info see  <https://www.shawntabrizi.com/blog/substrate/querying-substrate-storage-via-rpc/> 

___


## system
 
### blockHashCount: `u32`
- **interface**: `api.consts.system.blockHashCount`
- **summary**:    Maximum number of block number to block hash mappings to keep (oldest pruned first). 
 
### blockLength: `FrameSystemLimitsBlockLength`
- **interface**: `api.consts.system.blockLength`
- **summary**:    The maximum length of a block (in bytes). 
 
### blockWeights: `FrameSystemLimitsBlockWeights`
- **interface**: `api.consts.system.blockWeights`
- **summary**:    Block & extrinsics weights: base values and limits. 
 
### dbWeight: `SpWeightsRuntimeDbWeight`
- **interface**: `api.consts.system.dbWeight`
- **summary**:    The weight of runtime database operations the runtime can invoke. 
 
### ss58Prefix: `u16`
- **interface**: `api.consts.system.ss58Prefix`
- **summary**:    The designated SS58 prefix of this chain. 

   This replaces the "ss58Format" property declared in the chain spec. Reason is  that the runtime should know about the prefix in order to make use of it as  an identifier of the chain. 
 
### version: `SpVersionRuntimeVersion`
- **interface**: `api.consts.system.version`
- **summary**:    Get the chain's in-code version. 

___


## technicalCommittee
 
### maxProposalWeight: `SpWeightsWeightV2Weight`
- **interface**: `api.consts.technicalCommittee.maxProposalWeight`
- **summary**:    The maximum weight of a dispatch call that can be proposed and executed. 

___


## timestamp
 
### minimumPeriod: `u64`
- **interface**: `api.consts.timestamp.minimumPeriod`
- **summary**:    The minimum period between blocks. 

   Be aware that this is different to the *expected* period that the block production  apparatus provides. Your chosen consensus system will generally work with this to  determine a sensible block time. For example, in the Aura pallet it will be double this  period on default settings. 

___


## tips
 
### dataDepositPerByte: `u128`
- **interface**: `api.consts.tips.dataDepositPerByte`
- **summary**:    The amount held on deposit per byte within the tip report reason or bounty description. 
 
### maximumReasonLength: `u32`
- **interface**: `api.consts.tips.maximumReasonLength`
- **summary**:    Maximum acceptable reason length. 

   Benchmarks depend on this value, be sure to update weights file when changing this value 
 
### maxTipAmount: `u128`
- **interface**: `api.consts.tips.maxTipAmount`
- **summary**:    The maximum amount for a single tip. 
 
### tipCountdown: `u32`
- **interface**: `api.consts.tips.tipCountdown`
- **summary**:    The period for which a tip remains open after is has achieved threshold tippers. 
 
### tipFindersFee: `Percent`
- **interface**: `api.consts.tips.tipFindersFee`
- **summary**:    The percent of the final tip which goes to the original reporter of the tip. 
 
### tipReportDepositBase: `u128`
- **interface**: `api.consts.tips.tipReportDepositBase`
- **summary**:    The non-zero amount held on deposit for placing a tip report. 

___


## transactionPayment
 
### operationalFeeMultiplier: `u8`
- **interface**: `api.consts.transactionPayment.operationalFeeMultiplier`
- **summary**:    A fee multiplier for `Operational` extrinsics to compute "virtual tip" to boost their  `priority` 

   This value is multiplied by the `final_fee` to obtain a "virtual tip" that is later  added to a tip component in regular `priority` calculations.  It means that a `Normal` transaction can front-run a similarly-sized `Operational`  extrinsic (with no tip), by including a tip value greater than the virtual tip. 

   ```rust,ignore  // For `Normal`  let priority = priority_calc(tip); 

   // For `Operational`  let virtual_tip = (inclusion_fee + tip) * OperationalFeeMultiplier;  let priority = priority_calc(tip + virtual_tip);  ``` 

   Note that since we use `final_fee` the multiplier applies also to the regular `tip`  sent with the transaction. So, not only does the transaction get a priority bump based  on the `inclusion_fee`, but we also amplify the impact of tips applied to `Operational`  transactions. 

___


## treasury
 
### burn: `Permill`
- **interface**: `api.consts.treasury.burn`
- **summary**:    Percentage of spare funds (if any) that are burnt per spend period. 
 
### maxApprovals: `u32`
- **interface**: `api.consts.treasury.maxApprovals`
- **summary**:    DEPRECATED: associated with `spend_local` call and will be removed in May 2025.  Refer to <https://github.com/paritytech/polkadot-sdk/pull/5961> for migration to `spend`. 

   The maximum number of approvals that can wait in the spending queue. 

   NOTE: This parameter is also used within the Bounties Pallet extension if enabled. 
 
### palletId: `FrameSupportPalletId`
- **interface**: `api.consts.treasury.palletId`
- **summary**:    The treasury's pallet id, used for deriving its sovereign account ID. 
 
### payoutPeriod: `u32`
- **interface**: `api.consts.treasury.payoutPeriod`
- **summary**:    The period during which an approved treasury spend has to be claimed. 
 
### potAccount: `AccountId32`
- **interface**: `api.consts.treasury.potAccount`
- **summary**:    Gets this pallet's derived pot account. 
 
### spendPeriod: `u32`
- **interface**: `api.consts.treasury.spendPeriod`
- **summary**:    Period between successive spends. 

___


## txPause
 
### maxNameLen: `u32`
- **interface**: `api.consts.txPause.maxNameLen`
- **summary**:    Maximum length for pallet name and call name SCALE encoded string names. 

   TOO LONG NAMES WILL BE TREATED AS PAUSED. 

___


## uniques
 
### attributeDepositBase: `u128`
- **interface**: `api.consts.uniques.attributeDepositBase`
- **summary**:    The basic amount of funds that must be reserved when adding an attribute to an item. 
 
### collectionDeposit: `u128`
- **interface**: `api.consts.uniques.collectionDeposit`
- **summary**:    The basic amount of funds that must be reserved for collection. 
 
### depositPerByte: `u128`
- **interface**: `api.consts.uniques.depositPerByte`
- **summary**:    The additional funds that must be reserved for the number of bytes store in metadata,  either "normal" metadata or attribute metadata. 
 
### itemDeposit: `u128`
- **interface**: `api.consts.uniques.itemDeposit`
- **summary**:    The basic amount of funds that must be reserved for an item. 
 
### keyLimit: `u32`
- **interface**: `api.consts.uniques.keyLimit`
- **summary**:    The maximum length of an attribute key. 
 
### metadataDepositBase: `u128`
- **interface**: `api.consts.uniques.metadataDepositBase`
- **summary**:    The basic amount of funds that must be reserved when adding metadata to your item. 
 
### stringLimit: `u32`
- **interface**: `api.consts.uniques.stringLimit`
- **summary**:    The maximum length of data stored on-chain. 
 
### valueLimit: `u32`
- **interface**: `api.consts.uniques.valueLimit`
- **summary**:    The maximum length of an attribute value. 

___


## utility
 
### batchedCallsLimit: `u32`
- **interface**: `api.consts.utility.batchedCallsLimit`
- **summary**:    The limit on the number of batched calls. 

___


## vesting
 
### maxVestingSchedules: `u32`
- **interface**: `api.consts.vesting.maxVestingSchedules`
 
### minVestedTransfer: `u128`
- **interface**: `api.consts.vesting.minVestedTransfer`
- **summary**:    The minimum amount transferred to call `vested_transfer`. 

___


## voterList
 
### bagThresholds: `Vec<u64>`
- **interface**: `api.consts.voterList.bagThresholds`
- **summary**:    The list of thresholds separating the various bags. 

   Ids are separated into unsorted bags according to their score. This specifies the  thresholds separating the bags. An id's bag is the largest bag for which the id's score  is less than or equal to its upper threshold. 

   When ids are iterated, higher bags are iterated completely before lower bags. This means  that iteration is _semi-sorted_: ids of higher score tend to come before ids of lower  score, but peer ids within a particular bag are sorted in insertion order. 

   #### Expressing the constant 

   This constant must be sorted in strictly increasing order. Duplicate items are not  permitted. 

   There is an implied upper limit of `Score::MAX`; that value does not need to be  specified within the bag. For any two threshold lists, if one ends with  `Score::MAX`, the other one does not, and they are otherwise equal, the two  lists will behave identically. 

   #### Calculation 

   It is recommended to generate the set of thresholds in a geometric series, such that  there exists some constant ratio such that `threshold[k + 1] == (threshold[k] *  constant_ratio).max(threshold[k] + 1)` for all `k`. 

   The helpers in the `/utils/frame/generate-bags` module can simplify this calculation. 

   #### Examples 

   - If `BagThresholds::get().is_empty()`, then all ids are put into the same bag, and  iteration is strictly in insertion order. 

  - If `BagThresholds::get().len() == 64`, and the thresholds are determined according to the procedure given above, then the constant ratio is equal to 2. 

  - If `BagThresholds::get().len() == 200`, and the thresholds are determined according to the procedure given above, then the constant ratio is approximately equal to 1.248. 

  - If the threshold list begins `[1, 2, 3, ...]`, then an id with score 0 or 1 will fall into bag 0, an id with score 2 will fall into bag 1, etc. 

   #### Migration 

   In the event that this list ever changes, a copy of the old bags list must be retained.  With that `List::migrate` can be called, which will perform the appropriate migration. 
