---
description: >-
  An explanation of selling binary options and what takes place at the protocol
  level.
---

# Selling Options

Traditionally, 

When you stake ETH into the binary options trading protocol you receive pETH. pETH is a representation of your % of the total ETH that has been staked in the pool.

**For Example:** if Brock the bull is the first to stake, and sends 1 ETH and gets 1 pETH then Brocks pETH represents 100% of the pool. Then if Tahlia the tiger comes along and stakes 2 ETH she will receive 2 pETH. At this point Brock's 1 pETH represents 33% of the pool. Tahlia's represents 66%. Next Jose the jackrabbit buys a 2 ETH binary put option, he thinks the price is going to go down. An hour goes by and Jose is wrong, his option expires OTM. Now the pool has a total of 5 ETH. If Brock wants to withdraw his stake now he will receive 33% of 5 ETH or 1.66 ETH.

### Early Withdraw Fees

There is a 1% early withdrawal fee. 

When you lock ETH in the pool there is a lockup period. This is set at the time of staking and can't be changed later on for your stake. It is reset every time you make a new stake.

### Liquidity is locked when an option is opened

Whenever you withdraw you only receive your % of non locked liquidity. This means if there's 6 ETH in the pool and you have 3 pETH, but 2 ETH is currently locked in open options then you will only receive 2 ETH, not the 3 ETH you would get by waiting for those options to expire.

