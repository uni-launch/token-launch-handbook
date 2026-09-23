# Fees and costs

Three different things take money out of your wallet during a launch. They are
paid to three different parties, and only one of them is under a tool's
control.

## 1. The tool fee

What the platform charges for building and submitting the transaction. On
[Unilaunch](https://unilaunch.online/create-token?utm_source=github&utm_medium=docs&utm_campaign=handbook) it is quoted in the native
coin of the chain you picked, and it is made of a base fee plus a small amount
for each optional feature you switch on.

| Coin (chains that settle in it) | Base | Each optional feature |
| --- | --- | --- |
| SOL (Solana) | 0.3 | 0.1 |
| ETH (Ethereum, Base, Arbitrum, Blast, Robinhood Chain) | 0.02 | 0.01 |
| BNB (BNB Chain) | 0.1 | 0.025 |
| POL (Polygon) | 500 | 250 |
| AVAX (Avalanche) | 5 | 3 |

The optional features priced this way are social links, creator info,
multi-wallet supply distribution, burn on transfer, holder reflections, and
authority settings. **Creating a liquidity pool and configuring a transfer fee
add no tool fee.**

Figures can change. The builder shows the live total before you commit to
anything, and that total is the authoritative one.

## 2. The network fee

Gas, paid to the validators of the chain — never to the platform, and never
waivable. It depends on how busy the network is at the moment you sign, which
is why the final amount in your wallet's confirmation screen can differ from
the estimate you saw a minute earlier.

Two practical consequences:

- **Keep a margin.** Funding the wallet with exactly the quoted amount is how
  launches fail halfway.
- **Time it.** On Ethereum mainnet, the same transaction can cost several times
  more during peak hours than overnight.

## 3. The liquidity

If you open a pool, you deposit both sides of a pair: your tokens, and an
amount of the chain's coin. This is not a fee — it stays yours, in the pool's
smart contract, and you can withdraw it. What you are risking is price
movement, not a charge. See [Liquidity pools](liquidity-pools.md), and
[impermanent loss](glossary.md#impermanent-loss) in particular.

## Putting it together

A realistic Solana launch with two paid extras and a pool looks like:

```
tool fee      0.3 SOL base + 0.2 SOL for two extras   = 0.5 SOL
network fee   a fraction of a cent, twice             ≈ 0.00001 SOL
liquidity     whatever you choose to pair             = yours, at risk
```

The same launch on Ethereum mainnet swaps a trivial network fee for a
significant one, which is the single biggest reason people pick an L2.

## What is not refundable

Blockchain transactions are irreversible once confirmed, so tool fees are
generally non-refundable — there is no mechanism to claw back a transaction
that succeeded. The exception a serious operator will make is a verified defect
in their own software; on Unilaunch that runs through
[a support ticket](https://unilaunch.online/open-ticket?utm_source=github&utm_medium=docs&utm_campaign=handbook), and the
[FAQ](https://unilaunch.online/faq?utm_source=github&utm_medium=docs&utm_campaign=handbook) states the policy.

Before you pay anything, run the [pre-launch checklist](launch-checklist.md) —
most wasted fees are wasted on a token whose name or supply was wrong.
