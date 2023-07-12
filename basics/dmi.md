---
cover: ../.gitbook/assets/yellow.png
coverY: 0
---

# 📈 Digital Market Index

## ✳️ A broad benchmark of the digital asset space

The Digital Market Index is _**composed of 10 of the largest digital assets**_.

The index is denominated in [Euros](https://en.wikipedia.org/wiki/Euro) (€ - the currency of the [Eurozone](https://en.wikipedia.org/wiki/Eurozone) within the [European Union](https://en.wikipedia.org/wiki/European\_Union)).

The aim of the Digital Market Index is to provide investors with a transparent benchmark of the crypto space, one that can be tracked easily by investment funds and derivative products - more on that in the [Digital Market Fund \[DMF\] section](../summary-of-each-tab/pool/).

## ✳️ Index calculation

The universe of digital assets considered for inclusion in the index is comprised of the top 100 digital assets by [Real Volume](#user-content-fn-1)[^1] as reported by [Messari](https://messari.io/). The index is rebalanced on the first business day of each quarter.

1\) Filter out any digital asset that represents a [stablecoin](https://en.wikipedia.org/wiki/Stablecoin) (USDC, EURS...), a [wrapped token](https://www.ledger.com/academy/what-is-wrapped-crypto) (e.g. WBTC) or a [receipt token](https://www.pcmag.com/encyclopedia/term/defi-receipt-token) (e.g. stETH).

2\) Rank the remaining digital assets considered by Real Volume - in descending order, highest volume is #1.

3\) Calculate the average of the Real Volumes of the digital assets in positions #11-to-#20 in that list

4\) Now rank the digital assets by [Y+10 Marketcap](#user-content-fn-2)[^2] as reported by [Messari](https://messari.io/).

5\) Filter out the digital assets with Real Volume < average Real Volume calculated in step 3.

6\) If at this point the top 10 digital assets in our ranked list are the same ones as the ones currently included in the index we can proceed. However, if one or more of the digital assets are potential new additions, we apply the following rule:

\=> a new digital asset can only be added if it made the top 10 after stage 5 for 2 continuous quarterly calculations. If so, then the digital asset gets added.

Correspondingly, one of the digital assets currently in the index will be dropped: the one with the lowest Y+10 Marketcap at today's prices.

7\) At this point we now have a list of 10 digital assets along with their Y+10 Marketcaps in Euros. In order to calculate the weights, we use the square root of each of the Y+10 Marketcaps of the coins:

$$
W_i = \frac{\sqrt M_i}{\sum_n  \sqrt M_i} \forall i \in \{ 1, 2, ..., 10 \}
$$



## ✳️ Current information

The composition of the index is summarized in a table on the Home tab.

There you can see which digital assets are currently in the index and their respective weights.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2023-01-19 at 01.10.12.png" alt=""><figcaption></figcaption></figure>

## ✳️ Time Machine

The first table shows a historical (simulated) view of the index composition, every single month since January 2018.

[^1]: Real Volume is trading volume of the asset over the selected timeframe from the exchanges Messari includes in its Real Volume methodology.Reported Volume is the trading volume of the asset over the selected timeframe from all exchanges covered by Messari.

[^2]: The Y+10 Marketcap is the marketcap of the asset accounting for known issuance 10 years into the future. It is calculated by multiplying the current Price USD of the asset by its Y+10 Supply.
