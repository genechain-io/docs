---
description: 'Basics on miners, gas, tokens, block explorer, networks etc'
---

# Basics of Blockchain and GeneChain

Most of this page comes from a [help](https://metamask.zendesk.com/hc/en-us/articles/360015489611-Learn-the-basics-of-Blockchain-and-Ethereum-Miners-gas-tokens-block-explorer-networks-etc-) from MetaMask. We've changed a bit and added some basics on GeneChain.

#### **What is blockchain?**

Blockchain is a type of distributed ledger technology, which according to Dan Tapscott, "is an incorruptible digital ledger of economic transactions that can be programmed to record not just financial transactions but virtually everything of value.”

Robin Chauhan, [on their Medium,](https://medium.com/@rchauhan/the-bitcoin-blockchain-dna-metaphor-e9500333ca9f) offers another interesting interpretation of blockchain:

“Blockchain is a record of transactions, spreading across the internet as more people use cryptocurrencies. Similarly, DNA is a record of genetic transactions and mutations that spread as life expanded across the earth. Both become more complicated over time as our DNA evolves and new blocks are added to the blockchain.

Each blockchain \(Bitcoin, Ether, Ripple\) is like a distinct species \(human, chimpanzee, etc.\). A blockchain can also be forked \(like with Bitcoin Cash\) to create a competing currency in the same way that two distinct species can share common ancestor. 

In terms of transactions, they are organized into a series of blocks, which is the blockchain. A new block is created once verified. It means that a new pool of encrypted transactions \(possibly including yours!\) have been added to the blockchain.

#### **What is Ethereum?**

[Ethereum](https://www.ethereum.org/) is the blockchain, or decentralized platform, that runs smart contracts. It serves as “an enormously powerful shared global infrastructure that can move value around and represent the ownership of property.”

#### What is GeneChain?

[GeneChain](https://genechain.io) is a blockchain project derived from ethereum and focuses on high-performance and low-cost with a completely new consensus engine name [Ribose](../for-developers/ribose-consensus-protocol.md).

#### **What are miners?**

In [Proof of Work](https://en.wikipedia.org/wiki/Proof-of-work_system), miners solve complex puzzles to process transactions with advanced computing devices.

But in GeneChain, miners are rewarded with RNA, the native token of GeneChain, for processing transactions. And stakers are also rewarded with RNA for staking for miners.

#### **What is gas?**

Gas is the unit of measure for how much computational work is required to process transactions and smart contracts in the EVM. More complex smart contracts, and code, will require more gas to execute. \(Just like how bigger and/or faster cars will require more gas to power them\).

**Gas Limit:** 

Gas limit is the maximum amount of gas you are willing to spend. In MetaMask, when you are sending RNA/transactions, you will be required to specify gas limit and gas price:

![](https://lh6.googleusercontent.com/OYumootDH-0ampX1hOOycVWeotXsWaGfZqCNNw9u9MhAxF-QdDMx8USIRCMaP9pBpvHTyT16HHYt1lQ8AUDWAAvvgl5fzPVi5PpLDU3OHTBsB5KZFCnLucrKl5wSLMGYpmGEdiSU)

**Gas Price:** 

It specifies the amount of RNA you are willing to pay for each unit of gas.

#### **Tokens**

ERC-20 tokens are tokens created from [the ERC20 standard](https://theethereum.wiki/w/index.php/ERC20_Token_Standard). The ERC20 defines rules governing tokens to be accepted as ERC20 tokens, and leverage on the blockchain to be transacted.

You may see a [list of ERC-20 tokens here](https://scan.genechain.io/token).  You can also add any token following the [instructions here](https://metamask.zendesk.com/hc/en-us/articles/360015489031-How-to-View-Your-Tokens).

[ERC-721 tokens](https://medium.com/@brenn.a.hill/noobs-guide-to-understanding-erc-20-vs-erc-721-tokens-d7f5657a4ee7) are often referred to as "NFT's" aka Non-Fungible Tokens.  You can think of these more as digital objects on the blockchain, such as pieces of art or collectibles, rather than a store of value such as a tokenized currency. Currently, only the MetaMask mobile app supports interacting with ERC-721 assets. 

#### **What is a block explorer?**

A block explorer is an online blockchain browser. It displays the content of individual blocks, transactions, as well as the history and balance of addresses/wallets. 

#### **Main GeneChain Network and Testnets**

Transactions take place on the Main GeneChain Network. Testnets are created for developers to test smart contracts without paying gas. The testnet of GeneChain supported now is: [Adenine](https://scan-testnet.genechain.io).  You can use an "Testing RNA faucet" on [https://faucet.genechain.io](https://faucet.genechain.io), to request testing RNA to interact with the testnet blockchains and practice sending transactions and funds to other testnet accounts.  Please note, however, that the RNA in testnet are not "real" RNA and cannot be sent to mainnet addresses and exchanged for fiat value/other tokens.

