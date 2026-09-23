# Wallets and keys

Everything you do with a token starts in a wallet. Get this part right and the
rest is reversible mistakes; get it wrong and nothing else matters.

## Self-custody, in one paragraph

A self-custodial wallet is one where the keys live on your device and nowhere
else. No company can move your funds, and no company can restore them for you.
An exchange account is the opposite: convenient, and not yours. Token creation
tools — including [Unilaunch](https://unilaunch.online?utm_source=github&utm_medium=docs&utm_campaign=handbook) — work with
self-custodial wallets, because creating a token means signing a transaction
with a key only you hold.

## The three things you will hear about

| Term | What it is | Who may see it |
| --- | --- | --- |
| Public address | Your account number on the chain | Anyone. Share freely. |
| Private key | The signature power over one account | Nobody, ever. |
| Seed phrase | 12 or 24 words that regenerate every private key in the wallet | Nobody, ever. |

A seed phrase is not a password. A password protects an account you could
recover another way; a seed phrase *is* the account. Anyone who reads it owns
everything in the wallet, immediately and irreversibly.

## Which wallet for which chain

| Chain | Wallets |
| --- | --- |
| Solana | Phantom, Solflare |
| Ethereum, Base, Arbitrum, Blast, Robinhood Chain, BNB Chain, Polygon, Avalanche | MetaMask, Trust Wallet |

Install from the wallet's own website or the official app store, never from a
link someone sent you. Extension stores carry convincing fakes; the usual tell
is a recently published extension with few users and a familiar logo.

## Setting up, properly

1. **Write the seed phrase on paper.** Not a screenshot, not a notes app, not a
   password manager you also use on a compromised machine. Two copies in two
   places is better than one.
2. **Verify the words.** The wallet will ask you to re-enter some of them. Do
   it honestly — this is the only time you will find out you wrote them down
   wrong while it is still cheap.
3. **Send a small amount first.** Fund the wallet with a little of the native
   coin and move it once, so you know the flow works before real money is
   involved.
4. **Keep a launch wallet separate.** A wallet that only ever pays fees and
   holds the tokens you create limits the blast radius if you ever approve
   something you should not have.

## Funding it

Every chain charges its own coin for gas, so the coin you need depends on where
you launch:

- Solana → **SOL**
- Ethereum, Base, Arbitrum, Blast, Robinhood Chain → **ETH**
- BNB Chain → **BNB**
- Polygon → **POL**
- Avalanche → **AVAX**

Keep a margin above the quoted cost. Gas moves with network demand, and a
transaction that runs out mid-flight still costs you what it burned. See
[Fees and costs](fees-and-costs.md).

## Signing safely

Read what the wallet is actually asking before you approve it:

- **A signature request** proves you hold the address. It costs nothing and
  moves nothing — this is how sites log you in.
- **A transaction** moves coins or changes state on-chain. It shows the
  amount, the destination and the fee. Check all three.
- **An approval** lets a contract spend a token on your behalf, sometimes
  without a limit. Grant it only to contracts you meant to use, and revoke old
  ones periodically.

If a request does not match what you were doing on screen, reject it. A
rejected transaction costs nothing.

## Red lines

- No legitimate site, team member or "support agent" will ever ask for your
  seed phrase or private key. There is no situation where they need it.
- Support that contacts *you* first — in DMs, by email, in a comment reply —
  is almost always an impersonator. On Unilaunch, support runs through
  [tickets you open yourself](https://unilaunch.online/open-ticket?utm_source=github&utm_medium=docs&utm_campaign=handbook).
- A "wallet validation", "sync" or "migration" page asking for your words is a
  theft page. There are no exceptions to this rule.

More on the wider pattern in [Avoiding scams](avoid-scams.md), and a longer
beginner walkthrough at
[unilaunch.online/crypto-basics](https://unilaunch.online/crypto-basics?utm_source=github&utm_medium=docs&utm_campaign=handbook).
