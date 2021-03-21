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
{% api-method-parameter name="chain-id" type="string" required=true %}
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
{"reward":5455102.37103765,"votingPower":5062805.18169342}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.binance.org" path="/v1/staking/chains/{chain-id}/next-reward-time" %}
{% api-method-summary %}
Get Next Reward Time
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="chain-id" type="string" required=true %}
bsc or chapel
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{"nextRewardTime":"2021-03-22T00:00:00.999+00:00"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



