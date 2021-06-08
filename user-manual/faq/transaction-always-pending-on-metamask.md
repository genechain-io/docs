# Transaction always pending on MetaMask

If you send a transaction that cannot be packaged or you have used the testnet before or encountered other problems, you may encounter that the nonce value of your newly sent transaction is higher than the nonce value that can be processed. Then, your transaction may always be in a pending state, which is a known nonce conflict problem. For example, if your account nonce has just reached 10, but the newly sent transaction nonce is 12, the newly sent transaction will be waiting for processing and cannot be packaged.

## **Solution 1**

If you are using the desktop version of MetaMask and can find the first transaction that was blocked, you can click `Accelerate` or `Cancel`, and then increase the `Gas Price` and `Gas Limit` to try to allow the network to package the transaction normally. Note: `Accelerate` and `Cancel` are also available on MetaMask mobile, but it does not seem to be able to customize the Gas Price when accelerating or canceling.  
[![queue\_en.png](https://forum.dera.finance/assets/uploads/files/1621567202075-queue_en.png)](https://forum.dera.finance/assets/uploads/files/1621567202075-queue_en.png)  
[![adjust\_gas\_en.png](https://forum.dera.finance/assets/uploads/files/1621567206433-adjust_gas_en.png)](https://forum.dera.finance/assets/uploads/files/1621567206433-adjust_gas_en.png)

## **Solution 2**

If you cannot speed up or cancel or still cannot get packaged, in this case, you need to click `Reset Account` in `Settings -> Advanced` to reset the random number. This action will reset your random number and clear your transaction history, but will not change the balance in your account or require you to re-enter the mnemonic phrase.

After resetting the nonce value, you can resend the transaction covering the same nonce transaction that is queued on the network. At this time, please remember to increase the gas price to cover the transaction queued on the network to avoid the gas price of the new transaction not being higher than the old transaction which will lead to REPLACEMENT\_UNDERPRICED error and cannot overwrite the old transaction.  
[![IMG\_CFF66B4B3CF8-1.jpeg](https://forum.dera.finance/assets/uploads/files/1621567413372-img_cff66b4b3cf8-1.jpeg)](https://forum.dera.finance/assets/uploads/files/1621567413372-img_cff66b4b3cf8-1.jpeg)

If you are using MetaMask mobile and encounter the problem that resetting the nonce does not work, it is recommended to try the desktop version or reinstall MetaMask mobile. But DO REMEMBER to save your private key or mnemonic phrase in advance.

If you encounter a CALL\_EXCEPTION error after increasing the Gas Price or not, it is usually because MetaMask estimates the Gas Limit lower than the actual gas required. In this case, increasing gas limit might help.

