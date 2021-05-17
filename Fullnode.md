<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
**Table of Contents**
<!-- code_chunk_output -->

- [How to Run A Fullnode on GeneChain](#how-to-run-a-fullnode-on-genechain)
  - [Quick Start](#quick-start)
    - [Step 1: Build `geneth` from source](#step-1-build-geneth-from-source)
    - [Step 2: Launch `geneth` to start a full node](#step-2-launch-geneth-to-start-a-full-node)
    - [Main Genenet](#main-genenet)
    - [Adenine Testnet](#adenine-testnet)
  - [Fullnode Benefits](#fullnode-benefits)
  - [Sync Mode](#sync-mode)

<!-- /code_chunk_output -->

# How to Run A Fullnode on GeneChain

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

### Main Genenet
Main genenet will be available as soon as it is released. Running a full node on the main genenet is as simple as running

```shell
$ build/bin/geneth console
```

This will start the geneth client with access to the main genenet.

### Adenine Testnet
Running a full node on the Adenine testnet can be accomplished by appending a `--adenine` flag

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
