# 如何配置Metamask

在 Metamask 中配置 GeneChain 可以通过以下 3 个步骤完成

1. [安装](#安装)
2. [创建账号](#创建账号)
3. [配置GeneChain网络](#配置GeneChain网络)

## 安装


Metamask 可以通过 [https://metamask.io/](https://metamask.io/) 安装. 可以参考如下网址 [《雷达百科：MetaMask 入门》](https://wiki.radarlab.org/zh/defi/metamask_101/) 来详细了解如何安装 Metamask.

1. 打开网址 [https://metamask.io](https://metamask.io) 并根据你的浏览器类型进行安装。
   <img src="https://wiki.radarlab.org/assets/images/defi/uni101/a01_metamask_download.png" width="550px"/>
2. 我们已 Google Chrome 为例，其他浏览器安装流程也基本相同. 点击 `Chrome` 来安装 MetaMask 的 Chrome 扩展.
3. 点击 `Add to Chrome`.  
   <img src="https://wiki.radarlab.org/assets/images/defi/uni101/a02_metamask_chrome.png" width="550px"/>
4. 点击 `Add Extension`.

这就完成了，你已经成功安装了 MetaMask 扩展。

## 创建账号

参照 MataMask 提示的步骤来创建一个新的账号或者导入已经存在的账号到 Metamask 钱包。下面是一个简要的指导说明。


1. 点击浏览器右上角的 MetaMask 图标来打开扩展程序。
2. 点击 `Get Started` 来开始使用 Metamask.  
   <img src="https://wiki.radarlab.org/assets/images/defi/uni101/a03_metamask_get_started.png" width="550px"/>
3. 如果你已经有密钥短语，你可以通过导入密钥短语来初始化钱包，如果没有，请点击 `Create a Wallet`。
   <img src="https://wiki.radarlab.org/assets/images/defi/uni101/a04_metamask_create_a_wallet.png" width="550px"/>
4. 在 `Help Us Improve MetaMask` 页面, 点击 `No Thanks` 或 `I Agree`, 这将决定你收否要分享非敏感数据给 MetaMask 的开发者来提升用户体验。
   <img src="https://wiki.radarlab.org/assets/images/defi/uni101/a05_metamask_agreement.png" width="550px"/>
5. 你将被提示创建一个新的密码。 创建一个强度足够的密码并点击 `Create`.  
   <img src="https://wiki.radarlab.org/assets/images/defi/uni101/a06_metamask_new_password.png" width="550px"/>
6. 这里会提示你安全的保存你的加密短语。在确保周围环境安全的前提下点击 `CLICK HERE TO REVEAL SECRET WORDS` 来显示密钥短语。用安全的方式保存密钥短语。
*注意: 这是回复你的钱包账户的唯一方法。任何用于这个密钥短语的人都可以用这个密钥短语来恢复你的钱包并操作其中的资产。*  
   <img src="https://wiki.radarlab.org/assets/images/defi/uni101/a07_metamask_backup_phrase.png" width="550px"/>
7. 通过按顺序选择之前你记录的密钥短语来进行确认。完成后，点击 `Confirm`。
   <img src="https://wiki.radarlab.org/assets/images/defi/uni101/a09_metamask_confirm_phrase1.png" width="550px"/>

现在，你就有了一个初始化完毕的钱包，和初始化完成的账户。

## 配置GeneChain网络

### 自动设置

你可以访问 [https://staking.genechain.io](https://staking.genechain.io) 并点击 `Add GeneChain network` 来设置自定义网络.

### 手工设置

或者，你也可以参照如下步骤来自行设置GeneChain网络。

1. 打开 Metamask, 在 Network 下拉列表选择 "Custom RPC" 。
   <img src="https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/custom-rpc.png" width="400px"/>
2. 填写下列信息：

  * 主网 Genenet
    * Network Name: GeneChain
    * New RPC URL: https://rpc.genechain.io
    * Chain ID: 80
    * Currency Symbol: RNA
    * Block Explorer URL: https://scan.genechain.io

  * 测试网 Adenine
    * Network Name: GeneChain Adenine Testnet
    * New RPC URL: https://rpc-testnet.genechain.io
    * Chain ID: 8080
    * Currency Symbol: tRNA
    * Block Explorer URL: https://scan-testnet.genechain.io


点击 Save 就全部设置完毕了。
