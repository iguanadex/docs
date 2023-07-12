---
description: The iguana-treasury wallet on Arbitrum
---

# Multisig

## Overview

**The multisig does not have decision making power**, as its role is to simply enact on-chain the decisions $IGN holders make via off-chain voting.

The iguana-treasury wallet was deployed using [Gnosis Safe](https://gnosis-safe.io/), the most battle-tested multisig contract on BNB Chain and the overall EVM ecosystem.

The iguana-treasury wallet is a "3 out of 5" multisig wallet, meaning that signatures from 3 signers are required every time the wallet interacts with the chain. There are 5 possible signers in total.&#x20;

The 5 signers are a diverse set of community members. IguanaDEX contracts allow for some tweaking of core protocol parameters.

The multisig address can for instance set the level of protocol fees. As a placeholder for a future on-chain DAO, limited admin powers have been initially granted to the iguana-treasury wallet.

## Multisig Powers

IguanaDEX smart contracts grant specific powers to the iguana-treasury wallet address.

These powers are:

* grant roles in the Authorizer
* set the level of protocol swap fees (maximum 50% of total swap fees collected)
* set the overall swap fee in the DMI Pool and the IGN/BUSD Pool
* set the leverage trading fee
* set a flash loan fee
* extract collected protocol fees and/or excess balances (e.g. airdrops), from the Vault to any destination
* set the address of the oracle implementation
* pause/resume swaps on all pools
* set relayer addresses: relayers are (user opt-in, audited) contracts that can make calls to the vault (with the transaction “sender” being any arbitrary address) and use the sender’s ERC20 vault allowance, internal balance or BPTs on their behalf



## Future Signer Short-List

Beyond the current signers, the community shall keep a short, ordered list of potential signers in order to make any eventual signer substitution as smooth and timely as possible.

## Multisig signers

{% tabs %}
{% tab title="Arbitrum" %}
### Address

[0xE6ae1e6B67ad5D92F9a16B4CcaB45210DA43c8Da](https://bscscan.com/address/0xe6ae1e6b67ad5d92f9a16b4ccab45210da43c8da)

### Signers

* [Styliann](https://twitter.com/Styliann\_) (IguanaDEX)
* [Mut.eth](https://twitter.com/Mut\_eth) (Dewhales)
* [Nal X](https://twitter.com/0xNalX) (Wonderland)
* [Weierstrass](https://twitter.com/weierstrass42)
* [Wayne More](https://twitter.com/ThisIsWayneMore)
{% endtab %}
{% endtabs %}

## Context

Since its inception, the long-term vision for IguanaDEX is to be fully governed by IGN token holders, while token ownership is aimed to be widely spread across the Balancer community.

But getting to that ideal, long-term vision of a truly decentralized and effective governance is no easy task. Protocol governance is a highly complex and rapidly evolving topic. The whole crypto ecosystem is still in the very early days of trying to figure out:

* which mechanisms and processes work best
* the necessary infrastructure, tooling, and user interfaces
* the risks and concerns associated with each approach

Experimentation has been running wild in all directions:

* vote delegation
* minimum quorum
* specialized committees
* continuous voting
* augmented voting power via token lock
* off-chain voting for signaling / polling
* on-chain actions from off-chain voting by way of oracles
* upgradeable smart contracts
* time delays on sensitive actions
* emergency actions via Multisig (e.g. pause, shutdown)
* legal entities (e.g. foundation) providing support for the DAO
* tools for DAO treasury management
* token issuance to cover protocol expenses
* incentivized voting
* incentivized off-chain engagement (e.g. forum participation)
* and so on…

While also actively experimenting with governance-related initiatives, the Balancer community has leaned towards the more cautious and thoughtful approach of not trying to rush the path to full decentralization, so each step towards a mature on-chain governance will be taken with due care, having learned from others’ experiences.

## Signer Duties

All signers are expected to create a transaction on Arbitrum ratifying each decision made by IGN holders through Snapshot votes. This signature is expected to be done within the two weeks after the snapshot vote was concluded. Even after quorum is reached (by n signers), the remaining signers are also expected to sign before a multisig action is executed. This procedure aims to regularly confirm each signers’ conformity to the off-chain votes and also to serve as recent proof of their ability to sign.

A signer shall lose his/her role (by action of the remaining multisig signers excluding him/her) in case he/she:

* acts against IGN token holders’ off-chain voting;
* goes through 3 months or 2 votes (whichever takes longer) without performing any of their signer duties.

## Relevant Votes

The below Snapshot votes are instances of multisig or shortlist signers

* [Vote #1](https://snapshot.org/#/balancer.eth/proposal/0xadd41023d90e4e66bc1af834f7a3951b7c6171388d24f3779afed4ca9ad75a9e)
* [Vote #2](https://snapshot.org/#/balancer.eth/proposal/0xbd025f8f5a0b1d748a8ad034f5a2b6fd50cc8ff7257cbee6b8344b2a70e9e2ed)
* [Vote #3](https://snapshot.org/#/balancer.eth/proposal/0x9614c890099947b96d36cee4f6d64e649fe41bdd66331d1d93b39ed952c4ffcd)
