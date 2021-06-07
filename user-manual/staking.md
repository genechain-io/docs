# 质押挖矿

质押可以通过调用 Ribose 系统合约的 `stake` 方法来完成。你可以通过[合约的开源代码](https://github.com/genechain-io/system-contract/blob/master/contracts/Ribose.sol)来了解更多的信息。

一个更简单的方法是通过 [质押页面（staking page）](https://staking.genechain.io)来完成质押。

下文是质押页面的使用说明。

## 打开质押页面

打开 [质押页面\(staking page\)](https://staking.genechain.io)。

1. 如果没有安装 MetaMask, 点击 `Click here to install MetaMask` 按钮或者按照 [在 Metamask 钱包中配置 GeneChain](metamask.md)的说明来安装.  

    ![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-install-metamask.png)

2. 如果 GeneChain 网络没有配置，会显示如下提示： 
   1. 点击 `Add GeneChain network` 按钮来通知 MetaMask 添加 GeneChain 网络。

      ![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-add-network.png)

   2. 如果 `Approve` 没有显示，向下滚动或者点击 `close` 来显示 `Approve` 按钮。

      ![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-add-network-approve1.png)

   3. 在 MetaMask 点击 `Approve` 按钮来批准这个操作。 

      ![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-add-network-approve2.png)

   4. 点击 `Switch network` 来切换到 GeneChain 网络。 

      ![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-switch-network.png)

## 授权质押页面

你需要授权质押页面使用你的 MetaMask 账户来与 Ribose 系统合约交互。

你第一次打开质押页面的时候会自动提示授权，只需选择你希望使用的账户并点击 `Next`。  
 ![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-select-account.png)

然后点击 `Connect` 来完成链接。 ![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-connect.png)

## 选择一个候选人来质押

你可以在 `Top Candidates` 部分 找到所有可质押的候选人列表。选择一个候选人并点击 `stake` 来开始质押。 ![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-candidates.png)![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/staking-stake.png)

提示:

1. 你可以质押 RNA 和 ARM 中的一种或两种，你可以不质押ARM，但是一旦你想质押 ARM，必须质押不小于 3 个。
2. 如果你想质押 ARM，你需要授权\(approve\) Ribose 系统合约来使用你的 ARM，这需要点击 ARM 输入框旁边 `Approve` 按钮完成。
3. 在质押后的 86400 个区块，也就是约 72 个小时之内，不能进行解押操作。

## 领取质押收益

为某个候选人质押之后，你可以在 `Staked Candidates` 部分找到你的未结算收益\(unsettled profit\)和预估日收益\(estimated daily reward\)。你可以逐个结算\(settle\)你的未结算收益，或者点击`Settle All Unsettled Rewards`按钮结算所有收益。然后你将在右侧找到你的已结算收益\(settled profit\)，并可以通过点击 `Withdraw` 领取你的已结算收益到你的账户余额。

