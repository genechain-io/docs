# How to Use Metamask

Setting up Metamask for GeneChain can be achieved in three steps 1. [Installation](metamask.md#Installation) 2. [Create an account](metamask.md#create-account) 3. [Setup custom network for GeneChain](metamask.md#setup-custom-network-for-genechain)

## Installation

Metamask can be installed via [https://metamask.io/](https://metamask.io/) . Following is a simple guide from [Radarlab](https://wiki.radarlab.org/en/defi/metamask_101/) on how to install Metamask.

1. Open [https://metamask.io](https://metamask.io) and click your browser type to get proper version of Metamask for you browser.  

   ![](https://wiki.radarlab.org/assets/images/defi/uni101/a01_metamask_download.png)

2. Let's Google Chrome as an example, but the workflow is the same for all browsers. Click `Chrome` to install MetaMask as a Google Chrome extension.
3. Click `Add to Chrome`.  

   ![](https://wiki.radarlab.org/assets/images/defi/uni101/a02_metamask_chrome.png)

4. Click `Add Extension`.

That’s it! You have successfully installed MetaMask extension!

## Create Account

Follow the steps given by Metamask to create a new account or import an existing account into Metamask. Following is also the simple guide.

1. Click on the MetaMask icon in the upper right corner to open the extension.
2. Click `Get Started` to start using Metamask.  

   ![](https://wiki.radarlab.org/assets/images/defi/uni101/a03_metamask_get_started.png)

3. If you already have a seed phrase, you can initialize it by importing the seed phrase. If you don’t have a seed phrase, click `Create a Wallet`.  

   ![](https://wiki.radarlab.org/assets/images/defi/uni101/a04_metamask_create_a_wallet.png)

4. On the Help Us Improve MetaMask page, either click on `No Thanks` or `I Agree`, depending on whether you want to share non-sensitive data with MetaMask to improve user experience or not.  

   ![](https://wiki.radarlab.org/assets/images/defi/uni101/a05_metamask_agreement.png)

5. You will be asked to create a new password. Create a strong password and click `Create`.  

   ![](https://wiki.radarlab.org/assets/images/defi/uni101/a06_metamask_new_password.png)

6. Here you will be prompted to keep the seed secret key phrase. Click `CLICK HERE TO REVEAL SECRET WORDS` in a secure environment to display the secret key. Use a secure method to record these phrases.  

   _Note: This is the only basis for restoring your wallet account. Be aware that people who have these phrases can use these phrases to restore your wallet and manipulate the assets in it._  

   ![](https://wiki.radarlab.org/assets/images/defi/uni101/a07_metamask_backup_phrase.png)

7. Verify your secret phrase by selecting the previously generated phrase. When done, click `Confirm`.  

   ![](https://wiki.radarlab.org/assets/images/defi/uni101/a09_metamask_confirm_phrase1.png)

Now you will have your wallet and account initialized.

## Setup Custom Network for GeneChain

### Automatic setup

You can visit [https://staking.genechain.io](https://staking.genechain.io) and click `Add GeneChain network` to setup custom network.

### Manual setup

Or, you can follow the following steps to set it up by your self.

1. Open Metamask, and select "Custom RPC" from the Network Dropdown.  

   ![](https://raw.githubusercontent.com/wiki/genechain-io/geneth/assets/custom-rpc.png)

2. Fill the blanks with following information.
   * Main Genenet
     * Network Name: GeneChain
     * New RPC URL: [https://rpc.genechain.io](https://rpc.genechain.io)
     * Chain ID: 80
     * Currency Symbol: RNA
     * Block Explorer URL: [https://scan.genechain.io](https://scan.genechain.io)
   * Adenine Testnet
     * Network Name: GeneChain Adenine Testnet
     * New RPC URL: [https://rpc-testnet.genechain.io](https://rpc-testnet.genechain.io)
     * Chain ID: 8080
     * Currency Symbol: tRNA
     * Block Explorer URL: [https://scan-testnet.genechain.io](https://scan-testnet.genechain.io)

Click Save and all are set now!

