---
description: Transaction Mining on BIOPset
---

# Rewards

Incentivizing early adoption and transitioning to a successful decentralized governance system are the goals of BIOPset's utilization rewards initiative.

## Utilization Rewards In Brief

Every interaction with the BIOPset platform earns BIOP tokens. BIOP rewards may be sold or held or delegated for their voting power.

{% hint style="info" %}
In BIOP V2, utilization rewards were automatically issued. However, in BIOP V3, **utilization rewards must be claimed**.
{% endhint %}

Utilization rewards are quadrupled during the rewards period and are broken down in the table below:

| Action | Launch Rewards \(4x\) | Standard Rewards |
| :--- | :--- | :--- |
| Writing | 0.0016 BIOP | 0.0004 BIOP |
| Trading | 0.0008 BIOP | 0.0002 BIOP |
| Intervening | 0.0008 BIOP | 0.0002 BIOP |

{% hint style="info" %}
Capturing utilization rewards is also referred to as **transaction mining** in BIOPset documentation.
{% endhint %}

Intervening and trading rewards are issued per option. [Read more](https://docs.biopset.com/references/tokens/rewards#trading-utilization-rewards-in-detail).

Writing rewards are issued over time. [Read more](https://docs.biopset.com/references/tokens/rewards#writer-utilization-rewards-in-detail).

## Writer Utilization Rewards In Detail

Providing liquidity \(or **contributing** or **writing**\) to the pool is heavily incentivized. Writing utilization rewards are structured so that writers receive more BIOP over time depending on the amount of liquidity staked.

Writers earn rewards based on 3 factors: 

1. The size of their contribution to the pool. _For example, 10 ETH._
2. The length of time that contribution has been staked in the pool. _For example, 3 months._
3. The quantity of options written during the staking period. _For example, 400 1 ETH calls and 200 1 ETH puts._

These three types of rewards are called **contribution bonuses**, **period bonuses**, and **trading bonuses** respectively.

### Contribution Bonuses

Contribution bonuses are issued relative to the liquidity contributed to the pool.

| Contribution | Reward Multiplier |
| :--- | :--- |
| Any | 2X |
| More than 1% of the writer pool | 3X |
| More than 2% of the writer pool | 4X |
| More than 5% of the writer pool | 6X |
| More than 10% of the writer pool | 8X |
| More than 25% of the writer pool | 14X |
| More than 50% of the writer pool | 20X |

**Contributions are diluted over time as other writers contribute to the pool.** 

{% hint style="info" %}
Shalaquiana recommends claiming this bonus immediately after making a large contribution. Timing is essential because the contribution bonus is calculated at time of the writer makes the claim. 
{% endhint %}

### Period Bonuses

Period bonuses are issued every nine \(9\) days. _For example, contributing to the pool for 18 days results in 2X reward multiplier._

| Staking Period | Reward Multiplier |
| :--- | :--- |
| 9 Days | 1X |
| 18 Days | 2X |
| 27 Days | 3X |
| 81 Days | 9X |

There is no upper limit to the period bonus. As long as utilization rewards exist, writers are eligible to claim period bonuses. However, the bonus resets whenever there is a change in the funds contributed \(for example, on a withdrawal of funds from the pool\). The bonus also resets whenever rewards are claimed.

Every 9 days you remain staked your bonus will grow. For example at 18 days you get 2x, 27 days 3x, 81 days 9x. This bonus is uncapped. It resets anytime you claim rewards or withdraw from the pool.

### Trading Bonuses

A trading bonus is for every ETH written \(call or put\).

| Trade | Reward Multiplier |
| :--- | :--- |
| 1 ETH | 1X |
| 2 ETH | 2X |
| 10 ETH | 10X |

The trading bonus resets anytime rewards are claimed. It also resets whenever the contribution to the pool changes. _For example, funds are withdraw from the pool._

## Trading Utilization Rewards In Detail

Trading rewards are issued for each call or put purchased.

## Intervening Utilization Rewards in Detail

Intervening rewards are issued for each call or put expired or exercised.

