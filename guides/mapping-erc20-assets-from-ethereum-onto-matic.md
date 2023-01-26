# Mapping ERC20 assets from Ethereum onto Matic

To list your token on Dfyn, you must first have a valid token contract address on the Matic chain. If your ERC20 token is already deployed on the Ethereum network, you need to map it onto the Matic network. There are two ways using which this can be done:

### **Method 1: Directly Submit a Mapping Request to Matic**

{% hint style="info" %}
This method works only for standard tokens. If you haven’t already deployed a contract on Matic, a standard contract with deposit & withdraw methods will be deployed for you. However, for contracts with custom functionalities, you need to follow the [second method](mapping-erc20-assets-from-ethereum-onto-matic.md#method-2-deploy-a-custom-contract-on-matic).
{% endhint %}

**Step 1:** Visit [https://mapper.matic.today/](https://mapper.matic.today/)

**Step 2:** Click on **Map New Token.**

![](<../.gitbook/assets/Step 2 (3).png>)

By default, **Map Type: PoS** will be chosen and **Network: Ethereum – Matic Mainnet** will be chosen.

**Step 3:** Fill in the token details including the Ethereum token contract address, Matic token address (if the token contract is already deployed on Matic, otherwise you can leave this blank), and whether or not the token is mintable. A mintable token is one that can create new tokens on the fly and add to the total supply. The token symbol, name and decimal precision will automatically be sourced from your Ethereum token contract address.

![](<../.gitbook/assets/Step 3 (4).png>)

{% hint style="info" %}
You can only map your token if your Ethereum token contract is verified and published on Etherscan.&#x20;
{% endhint %}

{% hint style="info" %}
If you are mapping a contract that is already deployed on Matic mainnet, i.e. you already have a Matic token address, then the token contract on Matic should also be verified. &#x20;
{% endhint %}

**Step 4:** Finally, enter the email address at which you want to receive the notifications and click on **Submit**.

![](<../.gitbook/assets/Step 4 (7).png>)

As long as the details provided are valid, your application for token mapping will be successfully submitted.

Post the successful processing of your token mapping request, Matic team will reach out to you. **** Once your token is successfully mapped, you should find it listed [here](https://mapper.matic.today/).

### **Method 2: Deploy a Custom Contract on Matic**

In case your contract has certain functionalities that are not covered under the purview of a standard contract, you will need to customize your original smart contract and then deploy it on Matic. Post that, you will need to follow all the steps listed in[ Method 1](mapping-erc20-assets-from-ethereum-onto-matic.md#method-1-directly-submit-a-mapping-request-to-matic) to have your token on Matic mainnet mapped to its Ethereum counterpart.

A step-by-step guide for the same is given at: [https://docs.matic.network/docs/develop/ethereum-matic/pos/mapping-assets/](https://docs.matic.network/docs/develop/ethereum-matic/pos/mapping-assets/).

After you have successfully mapped your Ethereum token contract to your Matic token contract, you can add liquidity of your tokens on the Dfyn Exchange using the guide given [here](adding-liquidity-from-ethereum-to-dfyn-amm.md).
