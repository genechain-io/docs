# Introduction to GeneChain

GeneChain is a decentralized, efficient, and secure public chain, which realizes smart contract compatibility on the basis of supporting high-performance transactions. The GeneChain platform is designed to provide global developers with low-cost innovation facilities and stable infrastructure services.

## Consensus Algorithm

GeneChain’s consensus algorithm is Ribose, which is an algorithm based on the DPoS consensus mechanism. It nicely balances decentralization and performance, and has the features of low transaction cost, low transaction latency and high transaction concurrency; the node’s incentive is fees for on-chain transactions; fees are RNA; the maximum number of validators supported is 21; it provides rewards for miners; and provides rewards for community governors.

## Validator

Any user can run for active validator through the pledge, and GeneChain picks the highest-ranked ones as the active validator through the system contract every once in a while.

## Active Validator

The current group of validators responsible for packaging and producing blocks, with an upper limit of 21.

## Block Producer

Nodes responsible for producing and packaging blocks for transactions on the chain.

## Pledging Mining

With any account, any number of pledges can be made against the validator to support a validator and share the mining proceeds. If you want to retrieve the system Token that has been pledged, you need to send a declarative transaction to the system contract to unstake. After waiting for a period of time, the system contact is called again to withdraw the pledge and retrieve the pledged system Token. Punishment: when it is found that the validator has not produced the block in advance, it will automatically call the system contract at the end of the block to count the validator. When the count reaches the forfeiture threshold, all the validator's income is forfeited. When the count reaches the removal threshold, the validator will be removed from the active validator list and will be disqualified.

## Economic Model

The native token on the chain is RNA; the transaction consumes RNA as an on-chain transaction fee; the initial RNA is obtained through pre-sale, after which RNA will be released through block rewards in a decreasing manner year by year; on-chain transaction fees and additional RNA issued by the system will be rewarded for the node's block production.

## High Performance, Low Cost

* TPS(Transaction Per Second)：2000+
* Block Production Time: 3s


## Distributed Governance

Block producers rely on pledges of all users to run for public chain nodes. Users can become validators or support other validators by staking RNA and ARM. The validators can set the transfer ratio of block rewards to attract more users to pledge their own nodes, and the transfer rewards will be distributed according to the pledge ratio of all users under this validator.
