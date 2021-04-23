---
description: >-
  An explanation of selling binary options and what takes place at the protocol
  level.
---

# Selling Options

In BIOPset, options sellers are market makers \(or **liquidity providers**\). Sellers \(officially called **writers**\) pool their funds together to take an opposing position to any option buyer \(or **trader**\) that wants to express an opinion on the direction of prices.

Writers are always passive counterparties to active traders on the BIOPset platform.

{% hint style="info" %}
Counterparties take the opposing side of a binary options contract. It is impossible to buy binary options without a counterparty.
{% endhint %}

Whenever a writer makes a contribution to the pool, they are issued **pETH** \(or **poolETH**\) in proportion to their stake in the pool. For this reason, providing funds to the pool is ofter called staking.

## Staking Ether

BIOPset V4 offers traders the ability to speculate on the direction of Chainlink \(or **LINK**\) prices. The pooled ETH pool makes this possible. Option sellers deposit their contributions directly to this pool and receive pETH in return.

{% hint style="info" %}
The amount of pETH a writer receives is a representation of their relative contribution to the entire quantity of ETH in the pool.

**pETH is a risky asset.** Its value in ETH changes over time depending on the performance of the pool. The value may increase tremendously if the writer pool performs well. pETH could also become worthless if traders perform well.
{% endhint %}

pETH is issued one-to-one for ETH, but its redemption is less trivial.

## Redemption Value

pETH is redeemable for ETH. However, its redemption value changes every time binary options expire worthless \(or **out-of-the-money** or **OTM**\) or are valuable \(or **in-the-money** or **ITM**\) and exercised.

[Shalaquiana](https://twitter.com/shalaquiana) expresses this most eloquently with the following scenario:

> Suppose BIOPset just launched and Brock the Bull has 1 ETH at his disposal. He decides to sell binary options for the pure fun of it. It's discretionary wealth for him and he has a lot of wealth to burn.
>
> Brock is the first writer to stake and received 1 pETH for contributing 1 ETH to the fledgling ETH pool. Brock's 1 pETH represents 100% of the ETH pool.
>
> Furthermore, suppose Tahlia the Tigress comes along and contributes 2 ETH. She receives 2 pETH. At this point, Brock's 1 pETH represents 33% of the ETH pool. Tahlia's 2 pETH represents the remaining 66% of the ETH pool.
>
> Finally, suppose Jose the Jackrabbit holds the opinion that LINK prices are going down and purchases a 2 ETH worth of binary put option on the price of LINK via BIOPset. The oracle update is received and the options expire worthlessly OTM. Jose was wrong and lost 2 ETH.
>
> Jose's loss is the pool's benefit. At the expiration of Jose's binary option, the pool has a total of 5 ETH in it. If Brock were to withdraw his portion of the pool, his 33% stake is worth 1.66 ETH. He receives 33% of 5 ETH.

Shalaquiana's explanation is clearly understood, but it's an oversimplification. It left out one important part of market making on BIOPset: Liquidity Locks.

## Liquidity Locking

There are two types of liquidity locks in BIOPset:

1. Collateral Locks
2. Deposit Locks

Traders trigger collateral locks. Writers commit to a deposit lock every time they contribute liquidity.

### Collateral Locks

A collateral lock occurs whenever an option is purchased. The lock on pool funds remains until the option expires or the option is exercised ITM. A collateral lock contains both pool funds and trader funds.

During this period of time \(called the **lockup period**\) writers may only withdraw their respective share of the unlocked liquidity in the ETH pool.

Again, [Shalaquiana](https://twitter.com/shalaquiana) explains it best:

> **Withdrawal only entitles liquidity providers to their share of the unlocked liquidity.** For example, supposed there is 6 ETH in the pool and your share of the pool is 50% \(meaning that you possess 3 pETH of the total 6 pETH issued\) but a trader suddenly purchases 2 ETH worth of binary call options banking on LINK's price appreciation. That purchase would result in a collateral lock that reduces the unlocked liquidity from 6 ETH to 4 ETH.
>
> If you wanted to withdraw your liquidity during the collateral lock, you could only withdraw up to 2 ETH \(50% of the unlocked 4 ETH\). If you wait for the collateral lock to be removed through expiration, you could withdraw your entire stake of 3 ETH \(50% of the unlocked 6 ETH\). If the trader's binary option is ITM when settled then the funds in that collateral lock all go to the trader.

### Deposit Locks

Writers deposit ETH into the pool for minimum period of time. This is the second type of lockup period. The lockup period on a deposit lock resets every time a writer contributes new funds to the pool. It is set on the deposit of funds and cannot be reduced.

The lockup period of BIOPset V3 is 14 days. During that 14 day period, any withdrawal of funds contributed to the pool is taxed an early withdrawal fee\(1%\). After the lockup period funds may be withdrawn and occur no fees.

{% hint style="info" %}
The 14-day lockup period may change depending on governance decisions.
{% endhint %}

#### Early Withdraw Fees

There is a 1% early withdrawal fee. During the deposit lockup period, writers are only entitled to their stake in the unlocked pool liquidity.

{% hint style="info" %}
The early withdrawal fee does not apply after the 14-day lockup period expires and the percentage may change depending on governance decisions.
{% endhint %}

