# Choosing a chain

The chain decides three things you will live with: what your buyers pay per
transaction, which wallets and exchanges they already use, and how much your
launch costs you up front. Everything else is preference.

## The short version

| If you want… | Consider |
| --- | --- |
| The cheapest, fastest launch with a large retail audience | **Solana** |
| The deepest liquidity and the most credibility with serious buyers | **Ethereum** |
| Ethereum compatibility at a fraction of the gas | **Base**, **Arbitrum** |
| A big established retail market outside the ETH world | **BNB Chain** |
| Very low fees on an EVM chain | **Polygon** |
| A specific ecosystem you are already part of | Whichever one that is |

## What actually differs

**Transaction cost for your holders.** Every transfer, swap and approval costs
gas. On Solana and the cheaper EVM chains that is a rounding error; on Ethereum
mainnet it can exceed the value of a small trade, which quietly filters out
exactly the buyers a new token needs.

**Where the buyers already are.** A token lives or dies by the wallets that can
reach it without effort. Launching on a chain your audience does not use means
asking every one of them to bridge funds first — a step most will not take.

**Tooling and standards.** Solana tokens are SPL or Token-2022; EVM chains use
ERC-20 (BEP-20 on BNB Chain is the same idea). Explorers, charting sites and
bots differ in coverage per chain, and thin tooling makes a token look
abandoned even when it is not.

**Finality and reliability.** Confirmation times vary from sub-second to tens
of seconds. It rarely matters for holding, and it matters a great deal during
the first hour of trading.

## Cost at the moment of launch

Tool fees are quoted in the chain's own coin, so the comparison depends on
coin prices on the day. As a rough ordering, launching on Solana or an ETH L2
is the cheapest path, Ethereum mainnet the most expensive once gas is counted.
The exact numbers are in [Fees and costs](fees-and-costs.md) and, live, in the
builder at
[unilaunch.online/create-token](https://unilaunch.online/create-token?utm_source=github&utm_medium=docs&utm_campaign=handbook).

## Things that are not reasons

- **"This chain is trending."** Attention moves faster than a token launch
  does, and you cannot migrate holders afterwards.
- **"Gas is free here."** No chain is free; some are cheap. A chain with almost
  no fees also has almost no barrier to spam, which is its own problem.
- **"I can launch on all of them."** You can, and each one splits your
  liquidity and your community. Pick one for the launch; bridge later if there
  is demand.

## Available today

Live: Solana, Ethereum, Base, Arbitrum, Blast, Robinhood Chain, BNB Chain,
Polygon, Avalanche. Being integrated: Monad, Tempo.

A token created on one chain stays on that chain. If you are unsure, pick the
chain whose native coin you already hold and whose wallet you already use —
that is usually the honest answer to "where is my audience".
