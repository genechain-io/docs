---
description: >-
  Ribose is a Delegated Proof of Stake (DPoS) consensus protocol. GeneChain uses
  Ribose to reach network consensus and avoid forking.
---

# Ribose Consensus Protocol

_**Note: This topic is still under construction.**_

## Brief

Ribose selects 21 validation nodes to produce blocks in turn.

## Concepts

### Validator

Anyone can sign up for an account as a validator by calling `register` method of the [system contract](https://github.com/genechain-io/system-contract/blob/master/contracts/Ribose.sol), and only the validator account can accept mortgage in the system contract and run for active validators.

### Stake

Anyone can increase the mortgage weight for any validator by staking their `RNA` and `ARM` or one of them at any time. For the weight algorithm, see Mortgage Weight Algorithm. Users can also withdraw their mortgage to get their `RNA` and `ARM` back. However, the mortgage needs a lockup period to stabilize the network. It is tentatively set as 86,400 blocks, which is about 72 hours.

#### Staking Power

Staking power is calculated as $$\begin{cases} RNA \times \ln{(ARM)},&ARM \geq e\\ RNA,&otherwise\end{cases}$$ , where `e` is the Euler's number and `2.718281828459045236` is used here.

### Candidates

The system contract will record the top 50 validators with total mortgage weight as candidate validators. To ensure that the candidate validator remains active, a validator can be included in the candidate list only when its total mortgage weight changes. Hence, when a validator is removed from the candidate list, other validators must initiate a mortgage to win a place in candidate validators.

### Validator Set

`Validator Set` is a set of 21 addresses. GeneChain blocks can only be produced by nodes that are running in mining mode and binding to an account within these 21 addresses

`Validator Set` is updated every 200 blocks. Only top 21 accounts.

