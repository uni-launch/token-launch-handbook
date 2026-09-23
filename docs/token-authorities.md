# Token authorities

An authority is permission, recorded on-chain, to do something to a token after
it exists. Buyers read these before they buy, because they decide what you can
still do to them.

## On Solana

A new SPL token is created with three of them:

| Authority | What the holder can do | Revoking it means |
| --- | --- | --- |
| **Mint** | Create more tokens, any time, any amount | The supply is fixed forever |
| **Freeze** | Freeze any holder's balance in place | Nobody's tokens can ever be frozen |
| **Update** | Change the name, symbol and image (metadata) | The identity is fixed forever |

Revoking is one-way. There is no mechanism to restore an authority once it has
been given up — which is exactly why revoking is credible.

## On EVM chains

There is no equivalent flag on the standard itself; the same questions are
answered by what the contract can do:

| Capability | What it means | Why a buyer cares |
| --- | --- | --- |
| **Mintable** | New tokens can be created after launch | Their share can be diluted |
| **Burnable** | Tokens can be destroyed | Supply can shrink, deliberately |
| **Pausable** | Transfers can be halted | Someone can stop them selling |

A token that is mintable and pausable is, in practice, one where the deployer
can dilute and immobilise holders at will. That is not automatically wrong —
it is sometimes required — but it must be disclosed, because anyone competent
will check.

## Choosing

**Revoke the mint authority** if your promise is a fixed supply. It is the
single strongest, cheapest signal of good faith available to a new token, and
scanners display it prominently.

**Keep the mint authority** only if your plan genuinely needs future issuance —
staking rewards, scheduled emissions — and say so publicly, before launch,
rather than being asked.

**Revoke the freeze authority** in almost every case. Very few legitimate token
designs need the power to freeze individual holders, and its presence reads as
a rug-pull mechanism.

**The update authority** is the one worth thinking twice about. Keeping it lets
you fix a typo or replace a broken image URL; revoking it guarantees nobody can
quietly change what your token claims to be. If you keep it, expect to explain
why.

## How to check anyone's token

- Open the mint or contract address in the chain's explorer and read the
  authorities directly, rather than trusting a screenshot.
- Run it through a token scanner; most flag mintable, pausable and
  transfer-fee behaviour automatically.
- Check who holds the supply. Revoked authorities mean little if one wallet
  holds 90% of the tokens and can sell into your pool.

On Unilaunch these settings are made while configuring the token — see step 2
of [the builder](https://unilaunch.online/create-token?utm_source=github&utm_medium=docs&utm_campaign=handbook) — and the
[FAQ](https://unilaunch.online/faq?utm_source=github&utm_medium=docs&utm_campaign=handbook) explains what each one does at the moment
you choose it.
