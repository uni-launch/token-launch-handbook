# Token Launch Handbook

**A practical, vendor-maintained guide to creating and managing your own token — on Solana, Ethereum, Base, BNB Chain and six more networks, without writing code.**

[![Guides](https://img.shields.io/badge/guides-9-ff0098)](#the-guides)
[![Chains covered](https://img.shields.io/badge/chains-9%20live%20%2B%202%20soon-151515)](#supported-networks)
[![Licence: CC BY 4.0](https://img.shields.io/badge/licence-CC%20BY%204.0-blue)](LICENSE)
[![Website](https://img.shields.io/badge/website-unilaunch.online-ff0098)](https://unilaunch.online?utm_source=github&utm_medium=readme&utm_campaign=handbook)

Launching a token is five minutes of clicking and a long list of decisions you
cannot undo afterwards: which chain, how many decimals, whether to keep the
mint authority, how much liquidity to pair. This handbook is about the
decisions. It is written for people launching their first token, and it is
deliberately short on hype.

> **Who maintains this.** The handbook is written and kept current by the team
> behind [Unilaunch](https://unilaunch.online?utm_source=github&utm_medium=readme&utm_campaign=handbook), a no-code token creation and
> liquidity tool. The guides are written to be useful whatever tool you end up
> using; where Unilaunch is the example, it says so.

---

## Start here

| If you… | Read this |
| --- | --- |
| have never touched a wallet | [Wallets and keys](docs/wallet-setup.md) |
| are choosing a blockchain | [Choosing a chain](docs/choose-a-chain.md) |
| want to know the real cost | [Fees and costs](docs/fees-and-costs.md) |
| are about to launch | [Pre-launch checklist](docs/launch-checklist.md) |
| are setting up a pool | [Liquidity pools](docs/liquidity-pools.md) |
| want people to trust the token | [Token authorities](docs/token-authorities.md) |
| keep meeting unfamiliar words | [Glossary](docs/glossary.md) |
| just want the short answers | [Short FAQ](docs/faq.md) |

Or launch one now: **[unilaunch.online/create-token](https://unilaunch.online/create-token?utm_source=github&utm_medium=readme&utm_campaign=handbook)**.

## The guides

- **[Wallets and keys](docs/wallet-setup.md)** — self-custody in plain terms, which wallet works on which chain, and the habits that keep funds safe.
- **[Choosing a chain](docs/choose-a-chain.md)** — what actually differs between Solana, the Ethereum family, BNB Chain, Polygon and Avalanche when you are the one paying the fees.
- **[Fees and costs](docs/fees-and-costs.md)** — the three separate things you pay for, and why a quoted tool fee is never the final number.
- **[Pre-launch checklist](docs/launch-checklist.md)** — everything to decide, verify and prepare before you sign the creation transaction.
- **[Token authorities](docs/token-authorities.md)** — mint, freeze and update authority on Solana, the mintable/burnable/pausable equivalents on EVM chains, and what revoking them signals.
- **[Liquidity pools](docs/liquidity-pools.md)** — what a pool is, what the opening price is made of, slippage, and how adding and removing liquidity works.
- **[Tokenomics basics](docs/tokenomics-basics.md)** — supply, decimals, distribution, and the two extras (burn on transfer, holder reflections) worth understanding before switching them on.
- **[Avoiding scams](docs/avoid-scams.md)** — how rug pulls and honeypots work, what to check before buying, and why nobody legitimate ever asks for a seed phrase.
- **[Glossary](docs/glossary.md)** — the vocabulary, defined once, in one place.

## Supported networks

Nine networks are live today; two more are being integrated.

| Network | Native coin | Token standard | Status |
| --- | --- | --- | --- |
| Solana | SOL | SPL, Token-2022 | Live |
| Ethereum | ETH | ERC-20 | Live |
| Base | ETH | ERC-20 | Live |
| Arbitrum | ETH | ERC-20 | Live |
| Blast | ETH | ERC-20 | Live |
| Robinhood Chain | ETH | ERC-20 | Live |
| BNB Chain | BNB | BEP-20 | Live |
| Polygon | POL | ERC-20 | Live |
| Avalanche | AVAX | ERC-20 | Live |
| Monad | — | — | Coming soon |
| Tempo | — | — | Coming soon |

## What a launch costs

Three separate costs, and only the first one is set by the tool:

1. **Tool fee** — charged by Unilaunch, quoted in the chain's native coin. A base fee for the token, plus a small amount per optional feature you switch on.
2. **Network fee** — gas or priority fee paid to the network's validators. Nobody can waive it.
3. **Liquidity** — the coins and tokens you choose to put into a pool. Not a fee: it stays yours, at risk of price movement.

Base tool fees, by the coin the chain settles in:

| Coin | Base fee | Each optional feature |
| --- | --- | --- |
| SOL | 0.3 | 0.1 |
| ETH (Ethereum, Base, Arbitrum, Blast, Robinhood) | 0.02 | 0.01 |
| BNB | 0.1 | 0.025 |
| POL | 500 | 250 |
| AVAX | 5 | 3 |

Creating a liquidity pool and setting a transfer fee are included at no extra
tool fee. Prices can change — the live figures are always the ones shown in
the builder at [unilaunch.online/create-token](https://unilaunch.online/create-token?utm_source=github&utm_medium=readme&utm_campaign=handbook),
and [Fees and costs](docs/fees-and-costs.md) explains how the total is assembled.

## How a launch works

1. **Connect a wallet you control.** Phantom or Solflare for Solana; MetaMask or Trust Wallet for the EVM chains.
2. **Describe the token.** Network, name, symbol, decimals, supply, description, image. These cannot be changed later on most chains — see [the checklist](docs/launch-checklist.md).
3. **Configure the extras.** Social links, creator info, multi-wallet distribution, burn on transfer, holder reflections, authority revocation, and a liquidity pool if you want one.
4. **Pay and sign.** The fee is quoted before you commit; the transaction is signed in your own wallet and broadcast from there.
5. **Manage it afterwards.** Positions, adding and removing liquidity, and history live in [My Portfolio](https://unilaunch.online/liquidity-pool?utm_source=github&utm_medium=readme&utm_campaign=handbook).

Nothing in that flow is custodial: the platform never holds keys, tokens or
liquidity, and it never asks for a seed phrase. If any site ever does, close
it — see [Avoiding scams](docs/avoid-scams.md).

## Read it in your language

The main site is published in 11 languages:
[English](https://unilaunch.online/en?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[Español](https://unilaunch.online/es?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[Deutsch](https://unilaunch.online/de?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[Français](https://unilaunch.online/fr?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[Português](https://unilaunch.online/pt?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[Italiano](https://unilaunch.online/it?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[Türkçe](https://unilaunch.online/tr?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[العربية](https://unilaunch.online/ar?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[हिन्दी](https://unilaunch.online/hi?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[বাংলা](https://unilaunch.online/bn?utm_source=github&utm_medium=readme&utm_campaign=handbook) ·
[中文](https://unilaunch.online/zh?utm_source=github&utm_medium=readme&utm_campaign=handbook)

## Useful links

| | |
| --- | --- |
| Create a token | <https://unilaunch.online/create-token> |
| Liquidity pool and portfolio | <https://unilaunch.online/liquidity-pool> |
| Knowledge base | <https://unilaunch.online/knowledge-base> |
| Getting started guide | <https://unilaunch.online/getting-started> |
| Crypto basics | <https://unilaunch.online/crypto-basics> |
| FAQ | <https://unilaunch.online/faq> |
| Articles and tutorials | <https://unilaunch.wiki> |
| Support | <https://unilaunch.online/open-ticket> |

## Contributing

Corrections and additions are welcome — a wrong number in a guide is worse
than a missing one. Open an issue, or send a pull request; see
[CONTRIBUTING.md](CONTRIBUTING.md). Questions about your own launch are better
asked through [support](https://unilaunch.online/open-ticket?utm_source=github&utm_medium=readme&utm_campaign=handbook), where the team
can see your wallet and transaction.

If a guide here saved you a mistake, a star helps other people find it.

## Licence

Text and guides: [CC BY 4.0](LICENSE) — use them anywhere, with attribution.

---

*Nothing here is financial, legal or tax advice. Launching a token carries
risk, and blockchain transactions cannot be reversed. Decide for yourself, and
where the stakes are high, take professional advice.*
