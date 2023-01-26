# How does Dfyn achieve gasless transactions?

Our partnership with [Biconomy](https://biconomy.io/) and integration of meta-transactions ensures that all transactions on the Dfyn network remain gasless for the Polygon network.&#x20;

**Step 1:** User’s metamask is triggered for signature when performing a transaction on the Dfyn exchange. &#x20;

**Step 2:** The signed data is relayed to Biconomy’s relayers.

![Biconomy meta-transactions flow](<../.gitbook/assets/Biconomy meta transactions flow-02.png>)

**Step 3:** Biconomy’s relayers pay the gas fees and forward the transaction with user’s signed data to the Dfyn contracts.

**Step 4:** DFYN contracts decodes user information from signed data and updates the chain state.

{% hint style="success" %}
To avoid bottlenecks, multiple Biconomy relayers work in parallel to relay different transactions.
{% endhint %}

{% hint style="success" %}
To ensure that no malicious transaction takes place, only the relayers registered with Biconomy are permitted to participate in this process.
{% endhint %}
