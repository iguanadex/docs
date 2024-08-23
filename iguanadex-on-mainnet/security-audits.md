---
description: >-
  IguanaDEX is a 'perfect' fork of PancakeSwap. See Security Audits from
  PancakeSwap directly.
---

# 🔎 Security Audits

### PancakeSwap history

The smart contracts powering IguanaDEX were created by the PancakeSwap team, mainly replicating the work of the Uniswap team for versions 2 and 3 of their flagship AMM Spot DEX.

The current PancakeSwap app contains 3 decentralized exchange versions.

* [v2](https://github.com/pancakeswap/pancake-smart-contracts): this is a perfect fork of Uniswap v2
* [v3](https://github.com/pancakeswap/pancake-v3-contracts): Uniswap v3's business license expired mid-2023 and PancakeSwap took the opportunity to upgrade their app by deploying a slightly tweaked version of the Uniswap v3 contracts
* v4: this version is not available on IguanaDEX and there are currently no plans to make this available in the future.



You can find the audits pertaining to those contracts here:

* v2: The Uniswap v2 audit itself is relevant here as PancakeSwap did not introduce any changes
  * [dapps.org](https://dapp.org.uk/reports/uniswapv2.html)
  * [SlowMist](https://github.com/slowmist/Knowledge-Base/blob/master/open-report/Smart%20Contract%20Security%20Audit%20Report%20%20-%20PancakeSwap.pdf)
* v3: Note that IguanaDEX does _not_ use MasterChefV3/LmPool so Phase 2 of SlowMist's audit is not relevant here
  * [PeckShield](https://github.com/peckshield/publications/blob/master/audit\_reports/PeckShield-Audit-Report-PancakeSwapV3-v1.0.pdf)
  * [SlowMist](https://github.com/slowmist/Knowledge-Base/blob/master/open-report-V2/smart-contract/SlowMist%20Audit%20Report%20-%20PancakeSwap\_v3\_en-us.pdf)
