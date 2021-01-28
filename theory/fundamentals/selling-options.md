---
description: >-
  An explanation of selling binary options and what takes place at the protocol
  level.
---

# Selling Options

In BIOPset, options sellers \(or **writers**\) pool their funds together to take an opposing position to any option buyer \(or **trader**\) that wants to express an opinion on the direction of prices.

Writers are always passive counterparties to active traders on the BIOPset platform.

{% hint style="info" %}
Counterparties take the opposing side of a binary options contract. It is impossible to buy binary options without a counterparty.
{% endhint %}

Whenever a writer makes a contribution to the pool, they are issued **pETH** \(or **poolETH**\) in proportion to their stake in the pool. For this reason, providing funds to the pool is ofter called staking.

## Staking Ether

BIOPset V3 will offer traders the ability to speculate on the direction of ether \(or **ETH**\) prices. An ETH pool will be created to make this happen. Option sellers deposit their contributions directly to this pool and receive pETH in return.

{% hint style="info" %}
The amount of pETH a writer receives is a representation of their relative contribution to the entire quantity of ETH in the pool.

**pETH is a risky asset.** Its value in ETH changes over time depending on the performance of the pool. The value may increase tremendously if the writer pool performs well. pETH could also become worthless if traders perform well.
{% endhint %}

pETH is issued one-to-one for ETH, but its redemption is less trivial.

## Redemption Value

pETH is redeemable for ETH. However, its redemption value changes every time binary options expire worthless \(or **out-of-the-money** or **OTM**\) or are valuable \(or **in-the-money** or **ITM**\) and exercised.

Shalaquinha expresses this most eloquently with the following scenario:

> Suppose BIOPset just launched and Brock the Bull has 1 ETH at his disposal. He decides to sell binary options for the pure fun of it. It's discretionary wealth for him and he has a lot of wealth to burn. 
>
> Brock is the first writer to stake and received 1 pETH for contributing 1 ETH to the fledgling ETH pool. Brock's 1 pETH represents 100% of the ETH pool.

> Furthermore, suppose Tahlia the Tigress comes along and contributes 2 ETH. She receives 2 pETH. At this point, Brock's 1 pETH represents 33% of the ETH pool. Tahlia's 2 pETH represents the remaining 66% of the ETH pool. 
>
> Finally, suppose Jose the Jackrabbit holds the opinion that ETH prices are going down and purchases a 2 ETH binary put option on BIOPset. An hour passes and the options expire worthlessly OTM. Jose was wrong and lost 2 ETH.
>
> Jose's loss is the pool's benefit. At the expiration of Jose's binary option, the pool has a total of 5 ETH in it. If Brock were to withdraw his portion of the pool, his 33% stake is worth 1.66 ETH. He receives 33% of 5 ETH.

### Early Withdraw Fees

There is a 1% early withdrawal fee. 

When you lock ETH in the pool there is a lockup period. This is set at the time of staking and can't be changed later on for your stake. It is reset every time you make a new stake.

### Liquidity is locked when an option is opened

Whenever you withdraw you only receive your % of non locked liquidity. This means if there's 6 ETH in the pool and you have 3 pETH, but 2 ETH is currently locked in open options then you will only receive 2 ETH, not the 3 ETH you would get by waiting for those options to expire.

