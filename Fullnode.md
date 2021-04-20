# How to Run A Fullnode on Genechain

**Please note:** This wiki is for **Adenine TESTNET** right now. However, the main genenet won't differ much from adenine testnet. You can still get enough information on how to interact with the main genenet. This wiki will also be updated soon after the main genenet is released.

## Quick Start
### Step 1: Build `geneth` from source

Be sure that Go 1.13+ is already installed. Then run

```shell
# Clone the geneth repo
git clone https://github.com/genechain-io/geneth
# Enter the folder containing geneth source
cd geneth
# Compile
make geneth
```

### Step 2: Launch `geneth` to start a full node
Running a full node on the Adenine test network is as simple as running

```shell
$ build/bin/geneth --adenine console
```

This will start the geneth client with access to the Adenine testnet.

## Fullnode Benefits
* The full blockchain data is stored on disk.
* Provide RPC services.
* Validate new blocks and transactions.
* Verify states for accounts and contracts.

## Sync Mode
Sync mode can be changed using the `--syncmode "<mode>"` argument where `<mode>` can be:

* Full: Downloads all blocks (including headers, transactions, and receipts) and generates the state of the blockchain incrementally by executing every block.
* Fast (Default): Downloads all blocks (including headers, transactions and receipts), verifies all headers, and downloads the state and verifies it against the headers.
* Light: Downloads all block headers, block data, and verifies some randomly.
