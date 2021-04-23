---
description: >-
  An explanation of buying binary options and what takes place at the protocol
  level.
---

# Buying Options

Binary options are speculative financial instruments that derive their value from some other asset or quantity. Eventually, all binary options are either completely worthless or become worth a specific calculable amount in the future.

This section on buying options was taken from the detailed explanation provided on [Medium](https://munair.medium.com/what-are-binary-options-e18fcf59dd01). To skip the theory and dive straight into trading, check out the [instruction manuals](https://munair.gitbook.io/biopset/practice/guides).

## Price Speculation

BIOPset facilitates price speculation. The whole purpose of buying binary options is to take a position on the direction of movement in prices.

{% hint style="info" %}
Binary options are essentially all or nothing financial derivatives. Traders either win or they lose. There’s no in-between \(or other possible outcomes\).
{% endhint %}

They are called derivatives because their value is derived from something else after a certain period of time. After that period of time, the options are said to have **expired**. That _something else_ from which binary options derive their value is called the **underlying** \(or **underlying asset**\).

In BIOPset V4, the utilized information feeds are provided by [Chainlink](https://docs.chain.link/docs/reference-contracts). However, the underlying needn’t be a financial asset or cryptocurrency. It could be the quality of the weather \(like a rainy day\) or something else that will have an attribute that changes in the future. \[1\]

Binary options are speculative instruments. Those that purchase them \(**options buyers** or **options holders**\) usually have a strong opinion about the future state of some phenomenon. In BIOPset V4, traders that buy binary options typically have a serious opinion about the future price of their chosen price trading pair \(i.e. BTC/USD\).

More precisely, traders are actively engaged in forecasting the direction of the movements in the price of the underlying asset. They are not passively buying options because they want to _save_ money. **WARNING: never use your savings**.

Traders use the platform to _make_ money based on what \(they think\) they know about the future.

{% tabs %}
{% tab title="Options Buyers" %}
Options buyers hold an opinion about the direction of movement in the price of BTC/USD. There are only two directions: up or down. They choose one.

_For example, Alice believes that BTC/USD prices are going up. She feels very strongly that this will come to pass. Alice is willing to commit 10 ETH on that opinion and takes "**up**" the position against a pool of option sellers on BIOPset._
{% endtab %}

{% tab title="Options Sellers" %}
Options sellers **must** hold the opposing view about the future price of BTC/USD. By definition, the option seller is the counterparty and takes the opposition positi

{% hint style="info" %}
In BIOPset, no individual seller holds the opposing view alone. The sellers as a group hold the opposing view in proportion to the funds committed to the pool \(or house\).
{% endhint %}

_Considering Alice's strong opinion, the pool is obliged to take the opposing view and commits 10 BTC to prices going "**down**"._
{% endtab %}
{% endtabs %}

## Calls And Puts <a id="8949"></a>

Traders that want to make money on an appreciation in the price of BTC purchase **calls**. Those prognosticating a price decrease purchase **puts**.

Only price direction matters.

It never matters how much the price increases or decreases. In BIOPset, call holders win whether the price of BTC increases by one dollar or one thousand dollars. Similarly, put holders win whether the price of BTC decreases by one dollar or one thousand dollars.

## Strike Price <a id="effd"></a>

The price of BTC at the moment the binary option is purchased is called the **strike price**. It is always displayed on the BIOPset UI.

To be precise, it is the price of BTC at the moment the option was purchased according to the [Chainlink Oracle](https://www.gemini.com/cryptopedia/what-is-chainlink-and-how-does-it-work#:~:text=Summary,when%20certain%20conditions%20are%20met.). This is important to note because the value of the option changes based on this strike price.

Put holders can settle their options if the strike price exceeds the price of LINK when the first update from the oracle is received. Call holders can settle their options if the price of BTC when the first update from the oracle exceeds the strike price.

## Expiration <a id="15d9"></a>

At expiration, traditional binary options are always worthless \(or possess **zero intrinsic value**\). The intrinsic value that they possessed has **expired**. At that point, the right to exercise them no longer exists.

The concept of expiration does not exist with BIOPset. Expiration is set to infinity. That's because the value of the option is determined by the oracle update received.

## Settlement

Any person or bot may also settle the option and receive the 0.2_%_ **settlement fee** after the oracle update is received.

Consequently, the call or put holder can **settle** the option themselves and collect that 0.2% fee. In such cases, the payout of the option is 99% \(BIOPset charges 1% transaction fee\).

Otherwise, any arbitrary platform participant can settle the option if it is in their financial interest and collect the 0.2% fee. In such cases, the payout of the option drops to 98.8% \(as 0.2% is paid to the person/bot that settles the option\).

The settlement role transactions are always risk free. The exact payoff is viewable before this action is taken.

