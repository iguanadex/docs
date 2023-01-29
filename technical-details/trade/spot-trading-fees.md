# Spot Trading fees

## Overview

DMI token holders (i.e. Liquidity Providers) collect swap fees as users trade with the DMI pool.

## Swap Fees

Traders pay swap fees when they trade with the pool. The fees can be customized with a minimum value of 0.0001% and a maximum value of 10%.

80% of swap fees go to DMI token holders (i.e. Liquidity Providers) in exchange for them putting their tokens in the pool to facilitate trades. Trade fees are collected when a swap occurs, and they are deposited directly into the pool, growing the pool's balance in the process.

For a trade with a given $$inputToken$$ and $$outputToken$$, the amount collected by the pool as a fee is $$Amount_{fee} = Amount_{inputToken} * swapFee$$.

As the pool collects fees, **DMI tokens automatically collect fees** since they represent a **proportional share of the pool.**

#### Example:

Let's say Alice, Bob, Chuck and Diana provide a combined $100 of liquidity in the DMI Pool initially.

After some time, the pool has collected fees from various trades and is now worth $200. The pool itself grows while the Liquidity Providers' proportional shares stay the same.

| Person | Proportional Share | Initial Value | Value After Trading |
| ------ | ------------------ | ------------- | ------------------- |
| Alice  | 50.0%              | $50           | $100                |
| Bob    | 25.0%              | $25           | $50                 |
| Chuck  | 12.5%              | $12.50        | $25                 |
| Diana  | 12.5%              | $12.50        | $25                 |

![](<../../.gitbook/assets/Screen Shot 2021-08-12 at 10.10.06 AM.png>)

### Dynamic Fees

The [iguana-treasury multi-sig](https://app.safe.global/bnb:0xE6ae1e6B67ad5D92F9a16B4CcaB45210DA43c8Da/home) can change the level of fees in the DMI Pool. This has to be decided in a Governance vote by the DAO.

### Protocol Swap Fees

The Protocol collects 20% of swap fees.

Example: Chao sells $100 of ETH in exchange for BUSD to the pool. The fee on that pair is 0.05% so Chao will pay 5 cents in fees.

Out of those 5 cents, 4 cents will go to $DMI holders and 1 cent will go to the Protocol.
