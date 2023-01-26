# Changing Polygon's RPC Endpoint on MetaMask

If you are facing any transaction delays or if the data is taking too long to load on the Dfyn Exchange, it might be because of high congestion on the Polygon network. Since some RPC endpoints may be more busy than others at a given time, changing the RPC endpoint URL may sometimes lead to lower latency and better user experience. In this guide, we will show you how to change the RPC endpoint in MetaMask's Matic network configuration. Additionally, we will also show you how to [sign up for a free private RPC endpoint on Infura](changing-polygons-rpc-endpoint-on-metamask.md#creating-a-private-rpc-endpoint-on-infura).

### Polygon RPC Endpoints

|                                                  |                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>Public</p><p>RPC</p><p>Endpoints</p>          | <p></p><ul><li>https://polygon-rpc.com/</li><li>https://rpc-mainnet.matic.network</li><li>https://rpc-mainnet.matic.quiknode.pro</li><li>https://matic-mainnet.chainstacklabs.com </li><li>https://matic-mainnet-full-rpc.bwarelabs.com </li><li>https://matic-mainnet-archive-rpc.bwarelabs.com</li></ul>                                                            |
| <p>Create a</p><p>Private</p><p>RPC Endpoint</p> | <p></p><ul><li><a href="https://infura.io/">Infura</a></li><li><a href="https://rpc.maticvigil.com/">MaticVigil</a></li><li><a href="https://blog.quiknode.io/polygon-matic-is-now-live-on-quiknode-api/">QuickNode</a></li><li><a href="https://chainstack.com/build-better-with-polygon/">Chainstack</a></li><li><a href="https://www.ankr.com/">Ankr</a></li></ul> |

### Changing RPC Endpoint

**Step 1:** Open your MetaMask wallet and click on My Accounts (circular button on the top right) as shown in the figure below.

![](<../.gitbook/assets/Step 1 (1).png>)

**Step 2:** Click on Settings.

![](<../.gitbook/assets/Step 2 (4).png>)

**Step 3:** Go to Networks and select Matic Mainnet.

![](<../.gitbook/assets/Step 3.1.png>)

![](<../.gitbook/assets/Step 3.2.png>)

**Step 4:** Replace the old RPC endpoint with a new RPC endpoint (given [here](changing-polygons-rpc-endpoint-on-metamask.md#possible-endpoints)) and click on Save.

![](<../.gitbook/assets/Step 4 (2).png>)

Congratulations, you have successfully changed your RPC endpoint.

{% hint style="warning" %}
Note: It is not guaranteed that changing the RPC endpoint will result in lesser delays.
{% endhint %}

### Creating a Private RPC Endpoint on Infura

During times of high congestion on Public RPCs, you may consider moving to a private RPC endpoint. To create a private RPC endpoint for Polygon, you may use any of these services - [Infura](https://infura.io/), [MaticVigil](https://rpc.maticvigil.com/), [QuickNode](https://blog.quiknode.io/polygon-matic-is-now-live-on-quiknode-api/), [Chainstack](https://chainstack.com/build-better-with-polygon/), [Ankr](https://www.ankr.com/). In this guide, let us make a private endpoint using Infura.

**Step 1:** Go to [infura.io](https://infura.io/).

**Step 2:** Sign up if you haven't already. Otherwise, login using your credentials.

![](<../.gitbook/assets/Step 2 (2).png>)

**Step 3:** You should see a panel on the left hand side of your screen. On that panel, click on Ethereum.&#x20;

![](<../.gitbook/assets/Step 3.png>)

**Step 4:** Click on Create a Project.

![](<../.gitbook/assets/Step 4.1.png>)

You would be asked to name your project. Give a name of your choice and click on Create.

![](<../.gitbook/assets/Step 4.2.png>)

You should see the following screen.

![](<../.gitbook/assets/Step 4.3.png>)

**Step 5:** Under the Endpoints dropdown, select Polygon Mainnet.

![](<../.gitbook/assets/Step 5.png>)

**Step 6:** Copy the RPC endpoint.

![](<../.gitbook/assets/Step 6 (5).png>)

**Step 7:** Follow the steps given [here](changing-polygons-rpc-endpoint-on-metamask.md#changing-rpc-endpoint) and replace your existing RPC endpoint with the copied RPC URL.

![](<../.gitbook/assets/Step 7 (3).png>)

However, your RPC endpoint won't start working just yet. There are a few more steps that need to be followed before your Polygon RPC endpoint starts to work.

**Step 8:** Go to Ethereum dashboard and under My Account select Settings.

![](<../.gitbook/assets/Step 8 (4).png>)

Step 9: Click on Billing.

![](<../.gitbook/assets/Step 9 (1).png>)

Step 10: Click on Manage Projects.

![](<../.gitbook/assets/Step 10 (3).png>)

Step 11: Check Polygon PoS add-on and add your card details.

![](<../.gitbook/assets/Step 11 (2).png>)

{% hint style="info" %}
Even though you would be required to add your card details, you won't be charged anything. The Polygon PoS add-on is completely free.
{% endhint %}

Step 12: After adding card details, click on Get Started Now.

![](<../.gitbook/assets/Step 12 (1).png>)

Congratulations! Your Polygon network private RPC endpoint would now work perfectly.
