---
description: 矿工、Gas、代币、区块浏览器、网络等基础知识
---

# 关于区块链和GeneChain的基础知识

本页的大部分内容来自一篇 MetaMask 的[帮助文档](https://metamask.zendesk.com/hc/en-us/articles/360015489611-Learn-the-basics-of-Blockchain-and-Ethereum-Miners-gas-tokens-block-explorer-networks-etc-)。我们针对 GeneChain 进行了一些更改并添加了一些基础知识。

## 什么是区块链（Blockchain）？

区块链是一种分布式账本技术，据丹·塔普斯科特 \(Dan Tapscott\) 称，它“是一种廉洁的经济交易数字账本，可以通过编程来记录不仅是金融交易，还可以记录几乎所有有价值的东西。” Robin Chauhan 在他们的 [Medium](https://medium.com/@rchauhan/the-bitcoin-blockchain-dna-metaphor-e9500333ca9f) 上对区块链提供了另一种有趣的解释：

“区块链是一组交易的记录，这个记录随着更多的人使用加密货币而在互联网上传播。就像DNA 是随着生命在地球上扩展而传播的遗传交易和突变的记录。DNA随着发展日趋复杂，区块链也随着新区块被添加到区块链中而日趋复杂。

每个区块链（比特币、以太币、瑞波币，GeneChain）就像一个独特的物种（人类、黑猩猩等）。区块链也可以分叉（就像比特币现金一样）以创建一种竞争货币，就像两个不同的物种可以共享共同的祖先一样。 在交易方面，它们被组织成一系列的区块，这就是区块链。验证后会创建一个新块。这意味着一个新的加密交易池（可能包括你的！）已被添加到区块链中。

## 什么是以太坊（Ethereum）？

[以太坊](https://www.ethereum.org/)是运行智能合约的区块链或去中心化平台。它充当“一个非常强大的共享全球基础设施，可以转移价值并代表财产所有权。”

## 什么是GeneChain？

[GeneChain](https://genechain.io)是一个源自以太坊的区块链项目，专注于高性能和低成本，拥有全新的共识引擎[Ribose](../for-developers/ribose-consensus-protocol.md)。

## 什么是矿工（Miner）？

在[工作量证明（Proof of Work）](https://en.wikipedia.org/wiki/Proof-of-work_system)中，矿工解决复杂的难题以使用先进的计算设备处理交易。 但是在 GeneChain 中使用的[Ribose](../for-developers/ribose-consensus-protocol.md)是一种代理股权证明（DPoS），矿工会获得 GeneChain 的原生代币 RNA 来处理交易。质押者也因为矿工质押而获得 RNA 奖励。

## 什么是气体（Gas）？

Gas 是衡量在 EVM 中处理交易和智能合约所需的计算工作量的计量单位。更复杂的智能合约和代码将需要更多的 gas 来执行。 （就像更大和/或更快的汽车需要更多的汽油来驱动它们一样）。

### 气体限制（Gas Limit）：

Gas Limit 是您愿意花费的最大 Gas 量。在 MetaMask 中，当您发送 RNA/交易时，您需要指定 gas limit和gas price：

![](https://lh6.googleusercontent.com/OYumootDH-0ampX1hOOycVWeotXsWaGfZqCNNw9u9MhAxF-QdDMx8USIRCMaP9pBpvHTyT16HHYt1lQ8AUDWAAvvgl5fzPVi5PpLDU3OHTBsB5KZFCnLucrKl5wSLMGYpmGEdiSU)

### 气体价格（Gas Price）：

它指定了您愿意为每单位 gas 支付的 RNA 数量。

## 代币（Token）

ERC-20 代币是根据 [ERC20 标准](https://theethereum.wiki/w/index.php/ERC20_Token_Standard)创建的代币。 ERC20 定义了管理代币作为 ERC20 代币接受的规则，并利用区块链进行交易。 您可能会在此处看到 [ERC-20 代币列表](https://scan.genechain.io/token)。您还可以按照[此处](https://metamask.zendesk.com/hc/en-us/articles/360015489031-How-to-View-Your-Tokens)的说明添加任何ERC-20代币。

[ERC-721 代币](https://medium.com/@brenn.a.hill/noobs-guide-to-understanding-erc-20-vs-erc-721-tokens-d7f5657a4ee7)通常被称为“NFT”，即不可替代的代币。您可以将这些更多地视为区块链上的数字对象，例如艺术品或收藏品，而不是诸如代币化货币之类的价值存储。目前，只有 MetaMask 移动端支持与 ERC-721 资产交互。

## 什么是区块浏览器？

区块浏览器是一种在线区块链浏览器。它显示各个区块的内容、交易以及地址/钱包的历史记录和余额。

## GeneChain主网和测试网

交易通常发送到GeneChain主网上。测试网是为开发人员创建的，无需支付 gas 即可测试智能合约。现在支持的 GeneChain 测试网是：[Adenine](https://scan-testnet.genechain.io)。您可以使用 [https://faucet.genechain.io](https://faucet.genechain.io) 上的“测试 RNA 水龙头”，请求测试网上的 RNA 与测试网区块链进行交互，并练习将交易和资金发送到其他测试网账户。但是请注意，测试网中的 RNA 不是“真正的”RNA，不能发送到主网地址并交换为法定价值/其他代币。

