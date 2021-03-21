# Binance Chain Staking API

{% api-method method="get" host="https://api.binance.org" path="/v1/stakings/chains/{chain-id}/summary" %}
{% api-method-summary %}
Get Global Staking Status
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get the total number of BNB staked by all validator candidates and the total amount of BNB earned by validators .
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="chain0id" type="string" required=false %}
chain id is **chapel** for testnet and **bsc** for mainnet
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{    "name": "{"reward":5455102.37103765,"votingPower":5062805.18169342} name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "Ain't no cake like that."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



