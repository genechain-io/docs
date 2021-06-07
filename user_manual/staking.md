# Ribose Staking HowTo

Staking can be accomplished by calling the `stake` method of the Ribose system contract. You can find more information in the contract [source code](https://github.com/genechain-io/system-contract/blob/master/contracts/Ribose.sol).

A simpler way is to use the [staking page](https://staking.genechain.io). The staking page for Adenine testnet is [here](https://staking-testnet.genechain.io).

Here is a simple guide on how to use the staking page.

## Navigate to the staking page
Open the [staking page](https://staking.genechain.io). 

1. If Metamask is not installed, click the `Click here to install MetaMask` button or follow the steps in [[Metamask]] to install one.  
    <img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-install-metamask.png" width="500px"/>
2. If GeneChain Adenine Testnet is not configured, a prompt will be shown. 
   1. Click the `Add GeneChain network` button to inform MetaMask of adding GeneChain network.  
      <img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-add-network.png" width="500px"/>
   2. Scroll down or click close to show `Approve` button if not shown.  
      <img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-add-network-approve1.png" width="500px"/>
   3. Click `Approve` in MetaMask to approve this action.  
      <img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-add-network-approve2.png" width="500px"/>
   4. Click `Switch network` to switch to GeneChain.  
      <img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-switch-network.png" width="500px"/>

## Authorize the staking page
You need to authorize the staking page to use your account to interact with the Ribose system contract.

This is automatically prompted the first time you open the staking page. Just select the account you want to use and click `Next`.  
<img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-select-account.png" width="500px"/>

Then click `Connect` to finish the connection.  
<img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-connect.png" width="500px"/>

## Select a candidate to stake
You can now find all available candidates in `Top Candidates` section and select a candidate and click `stake` along with the candidate to start staking.  
<img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-candidates.png" width="500px"/><img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-stake.png" width="400px"/>

Note:
1. You can stake either RNA or ARM or both. You can stake with out ARM, but if you want to, you need to stake at least 3 ARMs.
2. If you want to stake your ARM, you need to approve the Ribose system contract to use your ARM by clicking the `Approve` next to the ARM input while staking.
3. You can not unstake within 86400 blocks which is about 72 hours since your last staking.

## Withdraw mining rewards
After staking a candidate, you'll find your unsettled profit and estimated daily reward in `Staked Candidates` section. You can settle your unsettled reward one by one or just click `Settle All Unsettled Rewards`. Then you will find your settled profit on right side, and you can click `Withdraw` bellow to withdraw you settled profit into your balance.