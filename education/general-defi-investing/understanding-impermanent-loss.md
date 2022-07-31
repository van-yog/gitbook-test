---
cover: ../../.gitbook/assets/Cover (4).png
coverY: 0
---

# Understanding Impermanent Loss

Impermanent loss is a unique feature that arises when providing liquidity to automated market makers (AMMs). It is a real risk that yield farmers come up against, which is why we’ll give you a clear understanding of what it is in this quick explainer.

### The background — AMMs and Liquidity Pools

Automated Market Makers, popularized by UniSwap, SushiSwap, PancakeSwap, and Ref Finance, are the mechanism by which decentralized exchanges (DEXes) can function. The main feature of DEXes is that they allow you to swap tokens without any intermediaries or the traditional order book technique that matches buyers and sellers.

So how does this work? Successful swaps using AMMs rely on two things, liquidity pools, and smart contracts. Smart contracts automatically execute any swaps that occur on the exchange, and liquidity pools hold the required funds needed to make the transaction — no counterparty is needed.

Liquidity pools are funded by users, who then receive a percentage of transaction fees and other rewards for lending out their coins; this is where yield farming comes from.

### So where does impermanent loss factor in?

Impermanent loss is due to the automatic rebalancing of funds that occurs when the price ratio in a liquidity pool changes relative to the price you deposited at. Unless you’re farming stablecoins, the impermanent loss is a common occurrence.

Impermanent loss is not always disastrous, and doesn’t always mean a loss in dollar terms, which is why it is sometimes referred to as an opportunity cost — impermanent loss means you would have done better simply holding the two coins rather than depositing them in a liquidity pool.

### How impermanent loss works

As part of AMMs, liquidity pools work when the total value of each asset in the pool is equal.

For example, with NEAR worth $5 and USDT worth $1, there must always be 5 times as many USDT as NEAR in the pool, creating a 50:50 ratio. If NEAR goes to $6, there must be 6 times as many USDT to keep the balance.&#x20;

_Let’s imagine you put have 100 NEAR ($500) and 500 USDT (total $1000), which you deposit into a liquidity pool._

NEAR surges 10% to $5.50 meaning your 100 NEAR is now worth $550. This is good for you, but not for the liquidity pool, as there is no longer a 50:50 balance.

* To keep ratios equal, some of your NEAR will be exchanged to USDT, giving you 524.4 USDT and 95.35 NEAR.
* The total in dollar terms of your tokens is now $1,048.81, which is great, you’ve made some profit! But if you simply held your tokens without depositing, your holdings would come to $1,050. This means your impermanent loss is $1.19, or 0.11%.

![](<../../.gitbook/assets/TW\_10.2 (2).png>)

While this doesn’t sound so dramatic, it’s important to note that this was a fairly conservative example. Impermanent loss can be much greater when farming two volatile assets (or less when farming two stable assets).

### Impermanent loss — things to note

* Impermanent loss can occur irrespective of whether token prices go down or up. It is to do with the different value ratios between the two coins you are farming.
* Impermanent loss can be offset by yield farming rewards — if you’re getting a 140% APY return, a small impermanent loss is unlikely to worry you.
* Impermanent loss is not permanent — further shifts in token prices can cause the pool to rebalance in your favor.
* Leveraged yield farming adds an extra layer of risk because you can be liquidated before rebalancing occurs, leaving you with impermanent loss, and a fall in the value of your position which is also subject to protocol fees.
* Impermanent loss is most dangerous when: \
  \- One token drastically increases in price. \
  \- One token drastically decreases in price. \
  \- One token increases, while the other one decreases.

To get more of an understanding of how impermanent loss works and look at some examples, we encourage you to look at these impermanent loss calculators:

[Daily DeFi impermanent loss calculator](https://dailydefi.org/tools/impermanent-loss-calculator/) - a simple calculator based on UniSwap’s algorithm. [WhiteboardCrypto impermanent loss calculator](https://whiteboardcrypto.com/impermanent-loss-calculator/) - three calculators with varying degrees of explanation behind the calculation of your impermanent loss.
