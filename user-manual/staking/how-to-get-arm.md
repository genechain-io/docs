# 如何获得ARM

这里有一些核心概念和一个简单的指南，说明如何通过[质押页面](https://staking.genechain.io)质押 VBC 以获得 ARM 并设置备注使得抵押给ARM合约的VBC被包括在计算原始RADR网络中的发行收益所用。

## 核心概念

### 铸造 ARM

ARM可以通过将 VBC 抵押到 ARM 合约来铸造，这可以通过调用 ARM 合约的 `exchange` 方法来完成。 ARM 的铸造比例固定为 1:1。

抵押给 ARM 合约的 VBC 数量存储在合约中，会被用于计算原始 RADR 网络中的发行收益。

**请注意：**只有已经质押了 VBC 的账户才能通过销毁 ARM 取回 VBC，烧毁的限制是剩余的质押金额。请记住以安全的方式备份您的密钥，否则您可能无法取回您的抵押 VBC。

### 销毁ARM

您可以销毁 ARM 以取回您质押的 VBC。这可以通过调用`burn` 方法来完成。销毁的 ARM 不能超过你剩余的VBC质押金额。兑换比例也固定为 1:1。

### 设置备注

为了让您质押的 VBC 包含在原始 RADR 网络发行计算中，您需要将您的 RADR 地址设置为您在 ARM 合约中的备注。这可以通过调用 `setMemo` 方法来完成。您当前剩余的VBC质押数量根据[第三方平台接入说明](https://wiki.radarlab.org/zh/introduction/third_party_access/)纳入原始RADR网络发行计算。

这是有关如何抵押VBC以获取ARM以及如何设置memo以包含在原始RADR网络发行计算中的简单指南。

**请注意：只有**质押了 VBC 的帐号才能通过销毁 ARM 来取回 VBC，可销毁的限额是剩余的 VBC 质押数量。 请确保以安全的方式备份您的密钥，否则您可能无法取回您抵押的 VBC。

## **质押VBC获得ARM** <a id="mint"></a>

点击右侧的`转换`按钮，开始质押 VBC 以获得 ARM。

![](../../.gitbook/assets/staking-get-arm-1.png)

输入您想要铸造的 ARM 数量，然后单击`授权并确认`，如果您已经批准，则只需单击`确认`。

![](../../.gitbook/assets/staking-get-arm-2.png)

在MetaMask中确认并发送授权交易和铸造交易。等待交易确认后，然后你会看到 ARM 被铸造到你的帐户中。

**注意：**您需要有足够的 VBC 才能铸造 ARM。铸造比例在 ARM 合约中固定为 1:1。

## **设置备注以包含在原始RADR网络发行收益计算中** <a id="setmemo"></a>

在下图位置输入您的RADR地址并单击`确认`即可轻松完成此操作。根据[第三方平台接入说明](https://wiki.radarlab.org/zh/introduction/third_party_access/)，您所抵押的VBC的所有金额都将计入原始RADR网络发行计算中。

**注意：**请确保您输入了正确的地址，因为我们对您的RADR地址一无所知。但是您以后可以更改它。

![](../../.gitbook/assets/staking-settings-2.png)

## **赎回您的VBC** <a id="burn"></a>

打开转换对话框并单击箭头按钮切换到赎回模式。

![](../../.gitbook/assets/staking-get-vbc-1.png)

只需输入ARM数量然后单击`Burn`即可赎回VBC，一旦确认了赎回交易，您的VBC将恢复。

![](../../.gitbook/assets/staking-get-vbc-2.png)

**注意：**赎回VBC的数量不能超过已抵押的VBC的数量。赎回兑换比例也固定为1:1。

