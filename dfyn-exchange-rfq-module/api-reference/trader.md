# Trader

Users and traders can use this API to fetch the best quote from all the integrated market makers.&#x20;

### Get Quote

{% swagger method="get" path="/getQuote" baseUrl="api.proxy.rfq.dfyn.network/api" summary="Get the best quote for a trade" %}
{% swagger-description %}
Returns the best quote from all the available market makers
{% endswagger-description %}

{% swagger-parameter in="query" name="user" required="true" %}
address of the user
{% endswagger-parameter %}

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

{% swagger-parameter in="query" name="nonce" type="uint" required="true" %}
nonce of the user (can be fetched from the RFQ contract)
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Quote received" %}
```javascript
{
    "data": {
        "message": "0x552ce952865663309de97567d906fd5a7d8c22ff66d5e4a39905c100f05426a9",
        "messageHash": "0xcd1e02e04cc62a04712c43a69fea0498fcd1c7259783e91a744f17239372edff",
        "v": "0x1b",
        "r": "0xca255446e47a610783b22850747ce663978ef1d56bb908301ab9167edeb14e2f",
        "s": "0x69de981f8bf06a158a8a7128302c536c5c7f74a33941b7cdd6921cb0d77c299f",
        "signature": "0xca255446e47a610783b22850747ce663978ef1d56bb908301ab9167edeb14e2f69de981f8bf06a158a8a7128302c536c5c7f74a33941b7cdd6921cb0d77c299f1b",
        "messageObject": {
            "user": "0x40d5250D1ce81fdD1F0E0FB4F471E57AA0c1FaD3",
            "custodian": "0x876cEA61f692F1624b6c8B1a8aC3d7A978A9f4fB",
            "token0": "0x7ceB23fD6bC0adD59E62ac25578270cFf1b9f619",
            "token1": "0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174",
            "amount0": "1000000000000000",
            "amount1": "1699106",
            "deadline": "1660047049",
            "nonce": 0,
            "chainId": "137"
        },
        "swapFee": {
            "type": "BigNumber",
            "hex": "0x01"
        }
    }
}
```
{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Error" %}
```javascript
{
    "data": null
}
```
{% endswagger-response %}
{% endswagger %}
