# Pre-launch checklist

Work down this list before you sign anything. Items marked **permanent** cannot
be changed after the creation transaction confirms.

## The token itself

- [ ] **Name** — spelled and capitalised exactly as you want it to appear forever. **Permanent**
- [ ] **Symbol** — short, unique enough to search for, not already used by a well-known token. **Permanent**
- [ ] **Decimals** — 9 is the Solana convention, 18 the EVM one; 6 suits a stable-value token. Match your audience's expectations. **Permanent**
- [ ] **Total supply** — decided together with your price story, not after it. **Permanent** unless you keep the mint authority.
- [ ] **Description** — what the token is for, in language a stranger understands.
- [ ] **Image** — square, readable at 32 px, hosted at a permanent URL. Wallets and explorers cache it; a broken image looks like an abandoned project.

## The wallet

- [ ] The launch wallet is one **you control**, with the seed phrase written down offline.
- [ ] It holds the chain's native coin, with a **margin above** the quoted total — see [Fees and costs](fees-and-costs.md).
- [ ] You are on the **right network** in the wallet before connecting.
- [ ] If any supply goes to other wallets, every destination address is **checked character by character**. A wrong address is an irreversible donation.

## The configuration

- [ ] You know which optional features you actually need, and what each one costs.
- [ ] If using **burn on transfer** or **holder reflections**, you understand that some exchanges and bridges handle transfer-taxed tokens badly — test before you promote.
- [ ] You have decided about **authorities**: keeping the mint authority means you can issue more later and buyers can see that; revoking it is a one-way promise. See [Token authorities](token-authorities.md).
- [ ] If opening a pool at creation: you know how many tokens go in, how much coin goes in, and therefore what the **opening price** is. See [Liquidity pools](liquidity-pools.md).

## The rehearsal

- [ ] Read the fee total on the confirmation screen and compare it with what you expected.
- [ ] Read the wallet's own confirmation — amount, destination, network — rather than clicking through it.
- [ ] Nobody is rushing you. Every "you must act in the next 10 minutes" in crypto is either a scam or a bad decision.

## After it confirms

- [ ] Save the **mint or contract address** somewhere permanent, and check it on the chain's explorer.
- [ ] Verify the token shows correctly in a wallet other than the one that created it.
- [ ] If you created a pool, check the position appears in [My Portfolio](https://unilaunch.online/liquidity-pool?utm_source=github&utm_medium=docs&utm_campaign=handbook).
- [ ] Publish the contract address yourself, in a place people can verify — impersonator tokens appear within minutes of any launch that gets attention.
- [ ] Keep the transaction signature; it is what support will ask for first.

## What no checklist can fix

A token is a container. It does not create demand, and launching one is the
easy part of whatever you are actually trying to build. Spend the planning
time on why anyone would want it — the settings above only decide how well the
container works.
