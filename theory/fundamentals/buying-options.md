---
description: >-
  An explanation of buying binary options and what takes place at the protocol
  level.
---

# Buying Options

Binary options are speculative financial instruments that derive their value from some other asset or quantity. Eventually, all binary options are either completely worthless or become worth a specific calculable amount in the future.

This section on buying options was taken from the detailed explanation provided on Medium [here](https://munair.medium.com/what-are-binary-options-e18fcf59dd01). To skip the theory and dive straight into trading, check out the [instruction manuals](https://munair.gitbook.io/biopset/practice/guides).

## Price Speculation

BIOPset was created to facilitate price speculation. The whole purpose of buying binary options is to take a position on the direction of movement in prices.

{% hint style="info" %}
 Binary options are essentially all or nothing financial derivatives. Traders either win or they lose. There’s no in-between \(or other possible outcomes\).
{% endhint %}

They are called derivatives because their value is derived from something else after a certain period of time. After that period of time, the options are said to have **expired**. That _something else_ from which binary options derive their value is called the **underlying** \(or **underlying asset**\).

## What's New?

In BIOPset V3, the underlying asset is ether \(or **ETH**\). However, the underlying needn’t be a financial asset or cryptocurrency. It could be the quality of the weather \(like a rainy day\) or something else that will have an attribute that changes in the future. \[1\]

Binary options are speculative instruments. Those that purchase them \(**options buyers** or **options holders**\) usually have a strong opinion about the future state of some phenomenon. In BIOPset V3, traders that buy binary options typically have a serious opinion about the future price of ETH.

More precisely, traders are actively engaged in forecasting the direction of the movements in the price of ETH. They are not passively buying options because they want to _save_ money. **WARNING: never use your savings**.

Traders use the platform to _make_ money based on what \(they think\) they know about the future.

{% tabs %}
{% tab title="Options Buyers" %}
Options buyers hold an opinion about the direction of movement in the price of ETH. There are only two directions: up or down. They choose one.

_For example, Alice believes that ETH prices are going up. She feels very strongly that this will come to pass. Alice is willing to commit 10 ETH on that opinion and takes "**up**" the position against a pool of option sellers on BIOPset._
{% endtab %}

{% tab title="Options Sellers" %}
Options sellers **must** hold the opposing view about the future price of ETH. By definition, the option seller is the counterparty and takes the opposition positi

{% hint style="info" %}
In BIOPset, no individual seller holds the opposing view alone. The sellers as a group hold the opposing view in proportion to the funds committed to the pool \(or house\).
{% endhint %}

_Considering Alice's strong opinion, the pool is obliged to take the opposing view and commits 10 ETH to prices going "**down**"._
{% endtab %}
{% endtabs %}

## Calls And Puts <a id="8949"></a>

Traders that want to make money on an appreciation in the price of ETH purchase **calls**. Those prognosticating a price decrease purchase **puts**.

Only price direction matters.

It never matters how much the price increases or decreases. In BIOPset, call holders win whether the price of ETH increases by one dollar or one thousand dollars. Similarly, put holders win whether the price of ETH decreases by one dollar or one thousand dollars.

## Strike Price <a id="effd"></a>

On BIOPset, call holders can exercise their options anytime the price of ETH exceeds the **strike price**. Put holders can exercise their options anytime the strike price exceeds the price of ETH.

The strike price of a binary option on BIOPset is simply determined. It is the price of ETH at the moment the option was purchased according to the [Chainlink Oracle](https://www.gemini.com/cryptopedia/what-is-chainlink-and-how-does-it-work#:~:text=Summary,when%20certain%20conditions%20are%20met.). It is always listed on the BIOPset UI. 

## Expiration <a id="15d9"></a>

At expiration, binary options are always worthless \(or possess **zero intrinsic value**\). The intrinsic value that they possessed has **decayed**. At that point, the right to exercise them no longer exists.

In BIOPset V3, the future is always only one hour away. Options always expire after 60 minutes. Consider it a fancy way of stating that your options are worthless after an hour.

Thanks to smart contract design, BIOPset options cannot completely expire on their own. Expiration requires intervention. Human intervention is incentivized by offering a 5_% expiration fee_.

Consequently, the call or put holder can _expire_ the option themselves and collect that 5% fee. In such cases, the payout of the option is 100%.

Otherwise, any arbitrary platform participant can expire the option if it is in their financial interest and collect the 5% fee. In such cases, the payout of the option drops to 95% \(as 5% is paid to the person/bot that expires the option\).

