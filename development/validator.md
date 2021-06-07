# Ribose Validator HowTo

To become a validator, first you need to run a node in mining mode with an account unlocked. Then register this account as a candidate for validators. After registration, you need to earn enough staking power to become an active validator or a top candidate.

This page covers the first two steps. [Staking](../user_manual/staking.md) page covers the last step, you can learn how staking power is calculated there. If you want to learn more about how validation works in GeneChain, please refer to [[Ribose Consensus Protocol]].

## Run a node in mining mode

### Step 1: Create an account as miner

An account is needed to start mining. This account is used to produce new blocks and receive mining rewards by default. You can set a different account to receive mining rewards later.

You can import an existing account with the following command

```shell
build/bin/geneth account import <path/to/private_key_file>
```

Or generate a new account by running

```shell
build/bin/geneth account new
```

### Step 2: Start a node with mining enabled

Mining can be enabled by executing the `geneth` client with both `--mine` flag and `--unlock` flag. Remember to specify the account address mentioned in step 1 after the `--unlock` flag.

```shell
# For mainnet
build/bin/geneth --mine --unlock <your_miner_account>

# For Adenine testnet
build/bin/geneth --adenine --mine --unlock <your_miner_account>
```

Remember to type the password to unlock the account. You can also use a password file with `--password` flag to unlock it.

Now after catching up with the latest block, you will have a node that is ready for producing blocks. The next step is to register your miner account as a validator candidate to receive staking.

## Register as a validator candidate

A validator candidate is registered by calling the `register` method of the Ribose system contract. You can find more information in the contract [source code](https://github.com/genechain-io/system-contract/blob/master/contracts/Ribose.sol). Either a web3 client or the scan page can be used to complete the registration.

**Note:** You need to use the miner account to call the `register` method as the caller account will be registered.

## Others

### Set block reward receiver
To better protect miners, we strongly recommend you to set a different account as block reward receiver.

`setProfitTaker` method can be used to set an account as receiver of block rewards.

**Note:** Only current profit taker can call this method. No one else can make the change, even the miner account.

### Withdraw miner profits
Block rewards are distributed into miner's pending profit at first. Pending profit might be punished to avoid misbehavior.

Only half of pending profit can be settled after 86400 blocks which is about 72 hours since last settlement.

Every time a miner produces a block, it's pending profit is checked and automatically settled into miner's miner profit if possible, which can be withdrew then. This is also done when making a withdraw.

`getCandidateState` can be used to check these values.

`withdrawMinerProfits` can be used to withdraw settled profit.