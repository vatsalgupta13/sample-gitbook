# Market Maker

Any market maker willing to register with Dfyn Exchange RFQ module, needs to expose an endpoint that has the following structure:

### Get Quote

{% swagger baseUrl="https://api.marketmaker.com/v1" method="get" path="/getQuote" summary="Get a quote from the market maker for the base token" %}
{% swagger-description %}
This endpoint should return a calldata that includes the quote price and the signature. As a market maker, you need to call Dfyn's RFQ contract to fetch the nonce. Nonce has to be included in the signed data.

**Note:** The deadline should be in _**seconds**._
{% endswagger-description %}

{% swagger-parameter in="query" name="token0" required="true" %}
token0 (base token) address
{% endswagger-parameter %}

{% swagger-parameter in="query" name="token1" required="true" %}
token1 (quote token) address
{% endswagger-parameter %}

{% swagger-parameter in="query" name="amount0" required="true" %}
token0 (base token) amount
{% endswagger-parameter %}

{% swagger-parameter in="query" name="chainId" required="true" %}
chain ID
{% endswagger-parameter %}

{% swagger-parameter in="query" name="user" required="true" %}
address of the user
{% endswagger-parameter %}

{% swagger-response status="200" description="Quote received" %}
```javascript
{
    "data": {
        "message": "0xb8c67dde023728dba425a51f58fff315f77b6ab0ef407adba297659fc9607ecd",
        "messageHash": "0x9c824e2411f333c3b95daa07a30df99e0ce0ab65e39581a7521c80c1db2594f1",
        "v": "0x1c",
        "r": "0x217bb9c6040df7b0d8e453cd7f9b2ff7370cdaabc9773a2c97a218cc7bc280de",
        "s": "0x0449bc077ef2d2ac607b9430ac5460bd61abbe76777932461bdac6bd5b771ce7",
        "signature": "0x217bb9c6040df7b0d8e453cd7f9b2ff7370cdaabc9773a2c97a218cc7bc280de0449bc077ef2d2ac607b9430ac5460bd61abbe76777932461bdac6bd5b771ce71c",
        "messageObject": {
            "user": "0xD6F89B2b2c5386c2FFcA62da13B342e630cC4eC8",
            "marketMaker": "0xDF012A32BA54C30e89913E231011AA13f0cE3369",
            "token0": "0xc2132D05D31c914a87C6611C10748AEb04B58e8F",
            "token1": "0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174",
            "amount0": "1000000",
            "amount1": "994391", //token1 (quote token) amount
            "deadline": 1655450917,
            "nonce": "0"
        },
    }
}
```
{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Permission denied" %}

{% endswagger-response %}
{% endswagger %}

### Example API Server

You can fork the following GitHub repo to create your own API server: [https://github.com/dfyn/rfq-api](https://github.com/dfyn/rfq-api). For access, please contact us on [Telegram](https://t.me/sajalgupta23).
