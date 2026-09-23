# Tokenomics basics

The numbers you choose in the builder are permanent on most chains, and they
imply things about your token whether you meant them or not.

## Supply

There is no correct total supply. 1,000,000 and 1,000,000,000 are equally
arbitrary; the only thing supply changes by itself is the number of zeros in
the price. What matters is the relationship between supply, the liquidity you
pair against it, and how much of it you keep.

Two habits worth avoiding:

- **Copying a famous token's supply** in the hope of copying its chart.
- **Picking an enormous supply for the cheap-looking unit price.** Buyers of
  new tokens read market capitalisation, not unit price.

## Decimals

How finely the token divides. 9 is the Solana convention, 18 the EVM default,
6 common for stable-value tokens. It changes nothing economically — it is a
display and precision decision — but it is permanent, and an unusual value
makes integrations and charts look wrong.

## Distribution

Who holds what at the first block. This is the number a serious buyer checks
first, ahead of the whitepaper.

- **Concentration is the signal.** One wallet holding most of the supply means
  one wallet can end the price. Split allocations across clearly labelled
  wallets and say what each is for.
- **Say what is locked, and prove it.** An unlocked team allocation is
  effectively circulating supply, whatever the roadmap says.
- **Multi-wallet distribution at creation** — supported in the builder — is
  cleaner than a flurry of manual transfers afterwards, which look like
  insider movement on the explorer.

## Burn on transfer

A percentage of each transfer is destroyed, reducing supply over time. It makes
every transfer more expensive for holders, and it makes the token a
"tax-on-transfer" token, which some routers, bridges and exchanges refuse or
mishandle. Test a real swap before you rely on it.

## Holder reflections

A percentage of each transfer is redistributed to existing holders. It rewards
holding without a staking contract, at the cost of the same compatibility
problems as burn on transfer — and of buyers who arrive expecting yield rather
than a product.

Both features are optional extras in step 2 of
[the builder](https://unilaunch.online/create-token?utm_source=github&utm_medium=docs&utm_campaign=handbook). Switch them on because
the design needs them, not because they are available.

## Authorities are part of tokenomics

A fixed supply claim means nothing while the mint authority is still held. If
your supply story matters, revoke it and let buyers verify — see
[Token authorities](token-authorities.md).

## A sanity test

Write down, in one sentence each: what the token is for, why the supply is that
number, who holds it at launch, and what stops you from printing more. If any
of those is hard to answer, the launch settings are not the problem yet.
