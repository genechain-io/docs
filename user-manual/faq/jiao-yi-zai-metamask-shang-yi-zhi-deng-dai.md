# 交易在MetaMask上一直等待

如果您发送的某个交易无法打包或您以前使用过测试网或遇到其它问题，可能会遇到您新发送的交易Nonce值高于可以处理的Nonce值。此时，您的交易可能始终处于待处理状态，这是一个已知的随机数冲突问题。比如您的帐号Nonce刚到10，但新发送的交易Nonce为12，新发送的交易便会一直等待处理状态，无法被打包。

## **方法一**

如果您使用的是桌面版MetaMask，并且能够找到阻塞的第一笔交易，可以点击加速或取消，然后增加Gas Price和Gas Limit尝试让网络能够正常打包这笔交易。注意：移动端MetaMask可以点击加速和取消，但目前似乎并不可以在加速或取消时自定义Gas Price。  
[![queue.png](https://forum.dera.finance/assets/uploads/files/1621566901907-queue.png)](https://forum.dera.finance/assets/uploads/files/1621566901907-queue.png)  
[![adjust\_gas.png](https://forum.dera.finance/assets/uploads/files/1621566945226-adjust_gas.png)](https://forum.dera.finance/assets/uploads/files/1621566945226-adjust_gas.png)

## **方法二**

如果无法加速或取消或仍然得不到打包，在这种情况下，您需在`设置 -> 高级`中单击`重设帐户`即可重置随机数。此操作将重置您的随机数并清除您的交易历史记录，但不会更改帐户中的余额或要求您重新输入助记词。

重置Nonce值后即可重新发送交易覆盖网络上在排队的同Nonce的交易，此时请记得调高Gas Price以覆盖网络上在排队的交易，避免因新交易的Gas Price不比旧交易高而遇到REPLACEMENT\_UNDERPRICED无法覆盖之前旧交易的错误。  
[![IMG\_0015.PNG](https://forum.dera.finance/assets/uploads/files/1621566980063-img_0015.png)](https://forum.dera.finance/assets/uploads/files/1621566980063-img_0015.png)

如果您使用移动端MetaMask遇到重置Nonce无效的情况，建议使用桌面端尝试或重新安装移动端MetaMask。但请记得提前保存好您的私钥或助记词。

如果调高Gas Price后或未调整时遇到CALL\_EXCEPTION错误，通常是因为MetaMask在预估Gas Limit时比实际执行所需要的Gas低，导致执行不成功。此时，需要调高Gas Limit可以帮助解决问题。

