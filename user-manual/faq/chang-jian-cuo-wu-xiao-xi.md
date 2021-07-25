# 常见错误消息

## REPLACEMENT\_UNDERPRICED

错误消息可能为 `replacement transaction underpriced` 或 `replacement fee too low`

该错误消息发生在尝试替换待处理的交易时，即您尝试发送的交易与您待处理的另一笔交易具有相同的随机数（Nonce）时。该错误消息发生时，意味着网络上已有一笔相同随机数（Nonce）的交易，且此交易的Gas Price大于或等于您新发送的交易。

如果您的目标是替换待处理的交易，您必须使用比待处理交易更高的Gas Price。

如果您的目标不是替换带处理的交易，新发送交易的随机数（Nonce）需比待处理交易的随机数（Nonce）高。

## nonce too low

该错误信息代表新发送的交易使用了一个已经使用过的随机数（Nonce）。请注意，每一个被打包的交易的随机数（Nonce）都需要是上一个被打包的交易的随机数（Nonce）+1。因此，发送交易时需要按顺序使用随机数（Nonce）。如果您不知道您现在的随机数（Nonce）到多少了，可以到[区块链浏览器](https://scan.genechain.io)最后一个被打包的交易。

## transferFrom failed

该错误信息通常代表传递的ERC20 token数额超过了持有的数量，通常减小传递的ERC20 token数量即可解决问题。

## out of gas

如果您看到消息“out of gas”，则您的交易已执行但失败。 换句话说，交易在执行时出现错误，因为它需要更多的气体，超过了发送交易时设置的gas limit。 这类似于驾驶汽车时汽油用量已到达限制使用量，但并没有到达目的地。

为避免再次出现“out of gas”错误，您需要增加下一笔交易的gas limit。 这可以在发送下一笔交易之前完成。 在[此处](../guan-yu-qu-kuai-lian-he-genechain-de-ji-chu-zhi-shi.md#shen-me-shi-qi-ti-gas)了解有关 gas、gas 价格和 gas 限额的更多信息。


