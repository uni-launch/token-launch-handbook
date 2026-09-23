# Avoiding scams

Most crypto losses are not sophisticated. They are a person typing twelve words
into a page that asked for them, or buying a token that was never sellable.

## The four that account for nearly everything

**The seed phrase page.** A site, DM or "support agent" asks you to "validate",
"sync", "restore" or "migrate" your wallet by entering your recovery phrase.
There is no legitimate version of this request. No tool needs your phrase to
do anything — creating a token, opening a pool, claiming an airdrop — because
signing happens inside your wallet.

**The impersonated support agent.** You post a problem publicly; within minutes
somebody friendly and well-branded messages you first. Real support does not
reach out in DMs. On Unilaunch, support exists only inside
[tickets you open yourself](https://unilaunch.online/open-ticket?utm_source=github&utm_medium=docs&utm_campaign=handbook) after
connecting your wallet.

**The rug pull.** A token attracts buyers, then the people who created it
remove the liquidity, and the price goes to zero because there is nothing left
to sell into. Check who holds the LP position and whether it is locked before
you buy — see [Liquidity pools](liquidity-pools.md).

**The honeypot.** A token you can buy and cannot sell, by design: the contract
blocks transfers from anyone but the deployer, or sets a sell tax of effectively
100%. The chart looks perfect, because nobody is able to sell.

## Before you buy anything

- **Get the contract address from the project's own channel**, not from a
  reply, a screenshot or a search result. Fake tokens with the right name
  appear within minutes of any launch that gets attention.
- **Open it in the chain's explorer.** Look at holder concentration, the age of
  the token, and the number of real transactions.
- **Run it through a token scanner.** Mintable, pausable, transfer tax and
  honeypot behaviour are all detectable automatically.
- **Try selling a small amount early.** A token that cannot be sold is cheaper
  to discover with $5 than with $500.
- **Distrust urgency.** "Presale closes in 10 minutes" exists to stop you
  checking the four things above.

## If you are the one launching

You inherit the burden of proof:

- Publish the contract address on the channels you control, and pin it.
- Revoke the authorities you do not need, and say which you kept and why —
  see [Token authorities](token-authorities.md).
- Be explicit about supply held by the team, and about anything locked.
- Expect impersonators. Someone will copy your name and ticker on day one;
  having one canonical, verifiable place for the real address is the only
  defence that works.

## If something has already gone wrong

A confirmed transaction cannot be reversed, cancelled or refunded by anyone —
that is a property of the chain, not a policy. Move any remaining funds to a
new wallet created from a fresh seed phrase, revoke outstanding approvals, and
assume the old wallet is compromised permanently.

Then keep the evidence: wallet address, transaction signature, timestamps. If
the problem involves a tool you used, that is exactly what its support will
ask for — for Unilaunch, through
[a ticket](https://unilaunch.online/open-ticket?utm_source=github&utm_medium=docs&utm_campaign=handbook).

Further reading, written for beginners:
[unilaunch.online/crypto-basics](https://unilaunch.online/crypto-basics?utm_source=github&utm_medium=docs&utm_campaign=handbook).
