# Glossary

The words that appear in every launch, defined once.

### Airdrop
Distributing tokens to many wallets for free, usually to bootstrap a community.
Also the most common bait in phishing campaigns.

### Approval
Permission you grant a contract to spend a token from your wallet. Often
unlimited by default; worth revoking when you stop using a site.

### Authority
On-chain permission to change something about a token after creation — mint,
freeze or update on Solana. See [Token authorities](token-authorities.md).

### Base fee / tool fee
What a creation tool charges for building and submitting the transaction. Paid
to the tool, not the network. See [Fees and costs](fees-and-costs.md).

### Burn
Destroying tokens by sending them somewhere nobody can spend from, reducing
supply permanently.

### Contract address / mint address
The token's unique identifier on-chain. On EVM chains it is the contract
address; on Solana, the mint address. This is the only reliable way to identify
a token — names and symbols are not unique.

### Decimals
How many fractional places the token divides into. 9 is conventional on
Solana, 18 on EVM chains. Permanent.

### DEX
A decentralised exchange: swaps happen against liquidity pools in smart
contracts rather than an order book run by a company.

### ERC-20 / BEP-20 / SPL / Token-2022
Token standards. ERC-20 is the Ethereum standard, BEP-20 its BNB Chain
equivalent, SPL the Solana one, and Token-2022 the newer Solana standard with
extra built-in features.

### Gas
The fee paid to a network's validators for including your transaction. Varies
with demand; never waivable.

### Honeypot
A token engineered so buyers cannot sell. See [Avoiding scams](avoid-scams.md).

### Impermanent loss
The gap between holding two assets and putting them in a liquidity pool. When
the price of one moves, the pool rebalances, and withdrawing can be worth less
than not having provided liquidity at all. It stops being "impermanent" the
moment you withdraw.

### Liquidity pool
Two assets held in a contract that people swap against; the ratio between them
sets the price. See [Liquidity pools](liquidity-pools.md).

### LP tokens
Your receipt for depositing into a pool. Redeeming them returns your share.
Locking or burning them is how a team demonstrates it cannot withdraw.

### Market capitalisation
Price multiplied by circulating supply. The number buyers actually compare —
not the unit price.

### Mint
To create new tokens. Also, on Solana, the account that *is* the token.

### Non-custodial
The tool never holds your keys or funds; you sign everything yourself.

### Private key
The secret that authorises spending from one address. Never shared, ever.

### Reflections
A share of each transfer redistributed to existing holders automatically.

### Rug pull
Removing the liquidity behind a token after attracting buyers, leaving them
unable to sell.

### Seed phrase
The 12 or 24 words that regenerate every key in a wallet. Whoever has them owns
the wallet. Never typed into a website.

### Slippage
The difference between the quoted price and the executed price, caused by the
trade itself moving a pool, or by the market moving while the transaction is
pending.

### Supply
How many tokens exist. Fixed if the mint authority is revoked; otherwise a
statement of intent.

### Ticker / symbol
The short name, like SOL or ETH. Not unique, and trivially copied by
impersonators — verify by contract address instead.

### Wallet
The software holding your keys and signing transactions. Self-custodial means
only you can sign. See [Wallets and keys](wallet-setup.md).
