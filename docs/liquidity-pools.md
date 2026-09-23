# Liquidity pools

A token with no pool cannot be bought. A pool is what turns a balance in your
wallet into something with a price.

## What a pool is

Two assets held together in a smart contract: your token, and something people
already own — the chain's native coin, usually. Anyone can swap one for the
other against the pool, and the ratio between the two sides *is* the price. Buy
pressure removes tokens and adds coin, and the price rises; selling does the
reverse.

Nobody sets the price. You set the opening ratio, and the market moves it from
there.

## The opening price

If you deposit 1,000,000 tokens and 10 SOL, the pool opens at 0.00001 SOL per
token. That is the only pricing decision you make directly, and two things
follow from it:

- **Deep pool, small moves.** More coin on the other side means each trade
  moves the price less. A thin pool looks dramatic on a chart and is trivially
  manipulated.
- **You are the first liquidity provider.** Your deposit is the money the first
  buyers trade against.

## Adding and removing

On Unilaunch the pool is created as part of the token, in step 2 of
[the builder](https://unilaunch.online/create-token?utm_source=github&utm_medium=docs&utm_campaign=handbook), rather than as a separate
job afterwards. Every position — including a token launched without a pool,
which starts at zero — then appears in
[My Portfolio](https://unilaunch.online/liquidity-pool?utm_source=github&utm_medium=docs&utm_campaign=handbook), where **Add Liquidity**
tops a position up and **Remove Liquidity** takes part or all of it back out.

The liquidity itself sits in the liquidity protocol's contract, not with the
platform. That is the difference between a tool that helps you build a
transaction and a custodian: the contract holds the funds, and your wallet
holds the claim.

## What can go wrong

**Impermanent loss.** When the price moves, the pool rebalances between the two
sides, and withdrawing later can be worth less than simply holding both assets
would have been. The bigger the move, the bigger the gap.

**Slippage.** The price you get is the price after your own trade moves the
pool, so a large trade against a small pool executes worse than the quote
suggested. Thin pools punish exactly the enthusiastic early buyer you want.

**Removing it all at once.** Withdrawing the whole pool leaves holders with a
token they cannot sell. Done deliberately after attracting buyers, that is the
textbook rug pull — and it is why anyone serious watches the LP position, not
the marketing.

**Transfer-taxed tokens.** If you enabled burn on transfer or reflections, test
a swap before promoting: some pools and routers handle tax-on-transfer tokens
badly, and the failure looks to a buyer like a broken token.

## Reasonable practice

- Open with enough depth that a normal-sized buy does not move the price
  double digits.
- Add liquidity in steps as volume grows, rather than all at once at launch.
- If you intend to lock or burn LP tokens as a trust signal, do it visibly and
  say where.
- Treat your own withdrawals as public events, because they are.

Definitions of the terms used here are in the [glossary](glossary.md).
