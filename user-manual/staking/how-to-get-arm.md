# 如何获得ARM

ARM可以通过向ARM合约抵押VBC来获得。抵押给ARM合约的VBC还将被包括在计算原始RADR网络中的发行收益所用，您唯一需要做的就是将RADR地址设置为ARM合同中的memo。

这是有关如何抵押VBC以获取ARM以及如何设置memo以包含在原始RADR网络发行计算中的简单指南。

**请注意：只有**质押了 VBC 的帐号才能通过销毁 ARM 来取回 VBC，可销毁的限额是剩余的 VBC 质押数量。 请确保以安全的方式备份您的密钥，否则您可能无法取回您抵押的 VBC。

## **通过质押VBC获得ARM**

单击右侧的`VBC-> ARM`按钮开始质押VBC以获取ARM。  
[![arm.png](https://forum.dera.finance/assets/uploads/files/1621001634745-arm.png)](https://forum.dera.finance/assets/uploads/files/1621001634745-arm.png)

设置限制额度，然后单击`Approve`以批准ARM合同以使用您的VBC余额。  
[![approve.png](https://forum.dera.finance/assets/uploads/files/1621001646685-approve.png)](https://forum.dera.finance/assets/uploads/files/1621001646685-approve.png)

点击`Confirm`以完成批准并等待交易被确认。  
[![confirm.png](https://forum.dera.finance/assets/uploads/files/1621001656196-confirm.png)](https://forum.dera.finance/assets/uploads/files/1621001656196-confirm.png)

确认后，输入要铸造的ARM数量，然后单击`Mint`。注意：您需要具有足够的VBC才能铸造ARM。在ARM合约中铸造比例固定为1:1。  
[![mint.png](https://forum.dera.finance/assets/uploads/files/1621002018429-mint.png)](https://forum.dera.finance/assets/uploads/files/1621002018429-mint.png)

同样，您需要单击`Confirm`并等待交易被确认。  
[![mint-confirm.png](https://forum.dera.finance/assets/uploads/files/1621002048462-mint-confirm.png)](https://forum.dera.finance/assets/uploads/files/1621002048462-mint-confirm.png)

确认后，您将看到您的ARM余额已更改。  
[![mint-done.png](https://forum.dera.finance/assets/uploads/files/1621002179771-mint-done.png)](https://forum.dera.finance/assets/uploads/files/1621002179771-mint-done.png)

现在，您可以使用ARM抵押候选人或做任何您想做的事情。

## **设置Memo以包含在原始RADR网络发行收益计算中**

在下图位置输入您的RADR地址并单击`Set`即可轻松完成此操作。根据[第三方平台接入说明](https://wiki.radarlab.org/zh/introduction/third_party_access/)，您所抵押的VBC的所有金额都将计入原始RADR网络发行计算中。注意：请确保您输入了正确的地址。由于我们对您的RADR地址一无所知，因此不会在此处检查地址。但是您以后可以更改它。  
[![set-memo.png](https://forum.dera.finance/assets/uploads/files/1621002310530-set-memo.png)](https://forum.dera.finance/assets/uploads/files/1621002310530-set-memo.png)

## **赎回您的VBC**

只需输入ARM数量然后单击`Burn`即可赎回VBC，一旦确认了赎回交易，您的VBC将恢复。

**注意：**赎回VBC的数量不能超过已抵押的VBC的数量。赎回兑换比例也固定为1:1。

