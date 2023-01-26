# Gasless Mode on Dfyn

We are the first DEX in the world to launch gasless mode. It is live at [https://www.exchange.dfyn.network](https://exchange.dfyn.network/). This feature will allow users to toggle Dfyn's gasless feature for their wallet:

* If the **Gasless Mode is kept on**, users will be able to carry out their transactions without having to pay any gas fees on Dfyn exchange.
* If the **Gasless Mode is kept off**, users will be required to pay a minimal gas fee on their transactions.

You can find the toggle button on top of your screen when you visit Dfyn exchange's [website](https://exchange.dfyn.network/).

![](<../.gitbook/assets/Screenshot (406).png>)

### Why should anyone turn off the Gasless mode?

Be default, the gasless mode will be enabled for all users. However, in some cases, users might need to turn off this setting. These cases include:

**1) If you are using hardware wallets:** Users operating on Dfyn Exchange with hardware wallets such as Ledger and Trezor will need to keep this feature turned off. This is due to the fact that our gasless mode necessitates EIP-712 message signing which is currently not supported by these wallets. The support for EIP-72 message signing should be added to these wallets in the future. However, for now, hardware wallet users should keep this mode off.

**2) If there are some issues with gasless transactions:** In rare cases, it might be so that the gasless mode is not working properly. This is because gasless transactions go through Biconomy's centralized relayers and if their relayers were to ever go down, gasless transactions on Dfyn won't go through. In such cases, users are advised to disable the gasless mode.&#x20;

To know more about how Dfyn enables gasless transactions, you can go [here](how-does-dfyn-achieve-gasless-transactions.md).

{% hint style="info" %}
Alternatively, in such cases, users can also visit [https://app.dfyn.network/](https://app.dfyn.network/), which works like [https://www.exchange.dfyn.network](https://exchange.dfyn.network/) with gasless mode off, i.e. the transactions here do not go through Biconomy's servers and hence do not require EIP-712 message signing.&#x20;
{% endhint %}
