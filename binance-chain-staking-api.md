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

{% api-method method="get" host="https://api.binance.org" path="/v1/staking/chains/{chain-id}/validators" %}
{% api-method-summary %}
Get Validator List
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

{% api-method-query-parameters %}
{% api-method-parameter name="offset" type="integer" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="limit" type="integer" required=true %}

{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
https://testnet-api.binance.org/v1/staking/chains/chapel/validators?limit=25&offset=0
{% endapi-method-response-example-description %}

```
{"total":166,"validators":[{"validator":"bva1pnww8kx30sz4xfcqvn8wjhrn796nf4dq77hcpa","valName":"Binance-Fuji","commissionRate":0.75000000,"votingPower":614030.60000001,"status":0,"votingPowerProportion":0.1213,"creationTime":null,"apr":0.00540000,"logoUrl":null,"delegatorNum":null},{"validator":"bva1wlxpuycavhvjzq27l6qzv07uf6cymgj7wcrf74","valName":"Binance-Kita","commissionRate":0.75000000,"votingPower":570471.78000000,"status":0,"votingPowerProportion":0.1127,"creationTime":null,"apr":0.00590000,"logoUrl":null,"delegatorNum":null},{"validator":"bva1kkwndgsd9hmnyqm7zsw3dnn6l63yv0vxakdsh3","valName":"StakeFun","commissionRate":0.25000000,"votingPower":500035.00000000,"status":0,"votingPowerProportion":0.0988,"creationTime":1615790212000,"apr":0.01880000,"logoUrl":null,"delegatorNum":null},{"validator":"bva10npy5809y303f227g4leqw7vs3s6ep5ul26sq2","valName":"Binance-Seoraksan","commissionRate":0.75000000,"votingPower":476669.00000000,"status":0,"votingPowerProportion":0.0942,"creationTime":null,"apr":0.00730000,"logoUrl":null,"delegatorNum":null},{"validator":"bva1p7s26ervsmv3w83k5696glautc9sm5rchz5f5e","valName":"Binance-Ararat","commissionRate":0.75000000,"votingPower":473544.23000000,"status":0,"votingPowerProportion":0.0935,"creationTime":null,"apr":0.00740000,"logoUrl":null,"delegatorNum":null},{"validator":"bva13egm8jsr54zdq3945jzvduul84egarfncqm7zw","valName":"Binance-Everest","commissionRate":0.75000000,"votingPower":473475.10000000,"status":0,"votingPowerProportion":0.0935,"creationTime":null,"apr":0.00640000,"logoUrl":null,"delegatorNum":null},{"validator":"bva15mgzha93ny878kuvjl0pnqmjygwccdad08uecu","valName":"Binance-Elbrus","commissionRate":0.75000000,"votingPower":263423.79000000,"status":0,"votingPowerProportion":0.0520,"creationTime":null,"apr":0.01380000,"logoUrl":null,"delegatorNum":null},{"validator":"bva15vvmregln3skagjcjxq9hshj452a2ppjkhperr","valName":"BNB48 Club","commissionRate":0.50000000,"votingPower":60123.75000000,"status":0,"votingPowerProportion":0.0119,"creationTime":null,"apr":0.09530000,"logoUrl":null,"delegatorNum":null},{"validator":"bva124ta3qd2ye4fgrm9dqp4kar3c6n8rqz4u3qg9t","valName":"Everstake_one","commissionRate":0.74000000,"votingPower":21951.00000000,"status":0,"votingPowerProportion":0.0043,"creationTime":null,"apr":0.12550000,"logoUrl":null,"delegatorNum":null},{"validator":"bva1u99rfh78ec6209z785aqmhf06hy8wpurl3et5c","valName":"Cosmic Validator","commissionRate":0.10000000,"votingPower":10153.00000000,"status":0,"votingPowerProportion":0.0020,"creationTime":1615465822000,"apr":1.12030000,"logoUrl":null,"delegatorNum":null},{"validator":"bva1k5vpnxpd805mgcvsagkqq9vg690f2tftehak8a","valName":"0x2VEV","commissionRate":0.10000000,"votingPower":10135.00000000,"status":1,"votingPowerProportion":0.0020,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1arc5fnx5t3hggnvuadqlltnp67eczyhk6qm02n","valName":"Staking4All","commissionRate":0.10000000,"votingPower":10132.00000000,"status":2,"votingPowerProportion":0.0020,"creationTime":null,"apr":1.11920000,"logoUrl":null,"delegatorNum":null},{"validator":"bva1n5guudmhtns542uvu0qs78ae5vkk6rygghg9j6","valName":"cz-binance","commissionRate":0E-8,"votingPower":0E-8,"status":2,"votingPowerProportion":0.0000,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva17hc2t8el0la6ep7p9q9dtp9chk5vyhzyu8ksup","valName":"blablabla","commissionRate":0E-8,"votingPower":0E-8,"status":2,"votingPowerProportion":0.0000,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva14y3ghzd9ktwdudlthhwj4flvxkm4lmh5mquf4j","valName":"verysoon","commissionRate":0E-8,"votingPower":0E-8,"status":2,"votingPowerProportion":0.0000,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1t8txnud45swwprpd3ggvesu32eghazs6aqfuu0","valName":"TodayClassroomMay","commissionRate":0E-8,"votingPower":0E-8,"status":2,"votingPowerProportion":0.0000,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1w8697xr8284t2yl0f56gjdq6vz42qprwk8mh54","valName":"cz@binance","commissionRate":0E-8,"votingPower":0E-8,"status":2,"votingPowerProportion":0.0000,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1xeezywem2k7ul66qnj7lzujcr94lst4hm35468","valName":"non-sense","commissionRate":0E-8,"votingPower":0E-8,"status":2,"votingPowerProportion":0.0000,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1r76en3dm8937e230fnye4m8j7wa05hczrnf7uy","valName":"BscScan","commissionRate":0.25000000,"votingPower":149970.00000000,"status":2,"votingPowerProportion":0.0296,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1609jdr5qpp7z33gvftqm9lmuumw0wym7u24her","valName":"EigenEisen","commissionRate":0E-8,"votingPower":86909.00000000,"status":2,"votingPowerProportion":0.0172,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva16myf933ceqnfnr4lam7pnmwkfenely7g02yurt","valName":"AnkrValidator","commissionRate":0.10000000,"votingPower":67128.79389341,"status":2,"votingPowerProportion":0.0133,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1s7wuv62avdepjcyhyhyk993df08vla2ltphmpv","valName":"MathWallet","commissionRate":0.25000000,"votingPower":49970.00000000,"status":2,"votingPowerProportion":0.0099,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1yhuwr0hv3gzjuldymssuhupqlcwx4ta8qza0pn","valName":"TW Staking","commissionRate":0.25000000,"votingPower":49970.00000000,"status":2,"votingPowerProportion":0.0099,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1m3aclw8qaf2vvpx55xznty6n4v7nwce6ll2dg2","valName":"CertiK","commissionRate":0.25000000,"votingPower":49970.00000000,"status":2,"votingPowerProportion":0.0099,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null},{"validator":"bva1fc90hdy0ew3lxqfl5xc2tn7nmuh5aqqqza25td","valName":"DareDandelion","commissionRate":0E-8,"votingPower":47939.00000000,"status":2,"votingPowerProportion":0.0095,"creationTime":null,"apr":null,"logoUrl":null,"delegatorNum":null}]}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.binance.org" path="/v1/staking/chains/{chain-id}/validators/{validator}" %}
{% api-method-summary %}
Query validator details
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
https://api.binance.org/v1/staking/chains/bsc/validators/bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

