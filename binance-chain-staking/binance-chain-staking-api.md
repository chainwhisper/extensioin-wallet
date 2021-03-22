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

{% api-method method="get" host="https://api.binance.org" path="/v1/staking/chains/{chain-id}/validators/{validator}/rewards" %}
{% api-method-summary %}
Query validator rewards
{% endapi-method-summary %}

{% api-method-description %}
https://testnet-api.binance.org/v1/staking/chains/chapel/validators/bva1pnww8kx30sz4xfcqvn8wjhrn796nf4dq77hcpa/rewards?startTime=1615766400&endTime=1615951226
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="validator" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="endTime" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="startTime" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="chain-id" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
[{"chainId":"chapel","validator":"bva1pnww8kx30sz4xfcqvn8wjhrn796nf4dq77hcpa","selfDelegator":"tbnb1pnww8kx30sz4xfcqvn8wjhrn796nf4dqshlvlg","valTokens":614032.30000001,"totalReward":30.57288394,"commission":22.92966296,"height":9890728,"rewardTime":"2021-03-17T00:00:01.000+00:00"},{"chainId":"chapel","validator":"bva1pnww8kx30sz4xfcqvn8wjhrn796nf4dq77hcpa","selfDelegator":"tbnb1pnww8kx30sz4xfcqvn8wjhrn796nf4dqshlvlg","valTokens":614032.30000001,"totalReward":29.70757612,"commission":22.28068209,"height":9852940,"rewardTime":"2021-03-16T00:00:00.000+00:00"},{"chainId":"chapel","validator":"bva1pnww8kx30sz4xfcqvn8wjhrn796nf4dq77hcpa","selfDelegator":"tbnb1pnww8kx30sz4xfcqvn8wjhrn796nf4dqshlvlg","valTokens":614032.30000001,"totalReward":20.23077415,"commission":15.17308061,"height":9815440,"rewardTime":"2021-03-15T00:00:00.000+00:00"}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.binance.org" path="/v1/staking/chains/{chain-id}/validators/{validator}/powers" %}
{% api-method-summary %}
Query validator powers
{% endapi-method-summary %}

{% api-method-description %}
https://api.binance.org/v1/staking/chains/bsc/validators/bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j/powers?startTime=1615766400&endTime=1615951226
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="chain-id" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="endTime" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="startTime" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="validator" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
[{"votingPower":266911.43382512,"snapshotTime":"2021-03-17T00:00:00.000+00:00"},{"votingPower":263367.03945692,"snapshotTime":"2021-03-16T00:00:00.000+00:00"},{"votingPower":259515.58706315,"snapshotTime":"2021-03-15T00:00:00.000+00:00"}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.binance.org" path="/v1/staking/chains/{chain-id}/validators/{validator}/operations" %}
{% api-method-summary %}
Query validiator related staking operation 
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="validator" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="startTime" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="endTime" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="chain-id" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{"total":2656,"operations":[{"delegator":"bnb1vca0fhseq0qfht54jkhjzcwkgcd939kpa4j0cw","operationType":0,"amount":1.13624650,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:51:52.000+00:00","txHash":"B3970105C59121CFB1C9F660402211B633F2A8396AA6CB006AC2D4467A8A6530"},{"delegator":"bnb1yfw960m7epszylfs3nnm70lje0k838vw6d5ggg","operationType":0,"amount":1.00000000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:47:59.000+00:00","txHash":"B8962E6CB16CADAD9C1C8F02D8451E40C767275997936863506A8018E0EEE173"},{"delegator":"bnb1mzmgzzl50ulpehkc5z6qq5hr2emzs7tel0jmsz","operationType":0,"amount":4.50000000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:47:57.000+00:00","txHash":"2137F61DC6FBBA86325F20305B49E5548B35164DEC74D8B0EA87396F1BE31033"},{"delegator":"bnb1l2zwtgv26mhvlz6mh745jwanqltn662nywy8r5","operationType":0,"amount":1.40380000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:46:21.000+00:00","txHash":"36222CD15070F2C340CDAB6472EE0DCEFFA48FAA0E72E8A15F8C610E755B3CE0"},{"delegator":"bnb1dx8wjkhgktpanjqsu92l6msxckztamw4ccp3xr","operationType":1,"amount":3.00000000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:43:48.000+00:00","txHash":"47BA4B166BC2DBF3F1DC2EE2E78A7094F1A6429F1E4AE8473BFD434E77DBA32A"},{"delegator":"bnb1zft5pmq8hf9jhe3fvwf6sg6tl5ges78p45ge0y","operationType":0,"amount":10.10000000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:39:14.000+00:00","txHash":"9E6DEAFE62B7C73EEA23D9FAC974E6317A0C4668322B82830712FABA0C7D9256"},{"delegator":"bnb1arkwkt8zmlp4aav7sq77yedenq7xdetpleprh2","operationType":2,"amount":5.00000000,"srcValidator":"bva1s0ntnh523dc2u5ez3dcj2t34k2x7y60cue46rt","validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:36:41.000+00:00","txHash":"ACD57C26B43285269F552BCD5E2BC488BF3AF03AB6980D0C9389F2744B927430"},{"delegator":"bnb173s2hys3fncxtwwuxy284kjkpqd0u6jtgknv4h","operationType":0,"amount":10.59085000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:34:16.000+00:00","txHash":"A4A3E1B7A70B4DA6AF6F86B75FA45C27A12B52995FE4A3B0E531D0F78288B902"},{"delegator":"bnb1lfxs2xhmne0re09vt99vzhwupt2q8qrq36v6vl","operationType":0,"amount":1.07539862,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:25:10.000+00:00","txHash":"9AB26F5795624B18745FC3ABB9144FD42ACEF0583ECF8A85E85E3CCEF7E1454A"},{"delegator":"bnb1mzt09mnaq4htld9yth0fcqk64sux3pkatysejc","operationType":2,"amount":1.80000000,"srcValidator":"bva1s0ntnh523dc2u5ez3dcj2t34k2x7y60cue46rt","validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:23:58.000+00:00","txHash":"FB940134CD55FDB061A7885E2B07EF41C3C60A7C64E42FF7BDD2F0727E6E820A"},{"delegator":"bnb1tz0k9fw507s95z5tnzyvx6msv3mz0ta0vyhn0p","operationType":0,"amount":2.52073004,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:21:31.000+00:00","txHash":"3E2E087AD2984D906D31A6D8F4CA43B90A41FB7B33026D1FC33A0C1A88965764"},{"delegator":"bnb12wqge5vzsne5ks9pvgrp286enqzg2uy9pfna38","operationType":1,"amount":1.03789073,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:21:29.000+00:00","txHash":"2694DB47C23429FBA29971CE8DF1FBDAAC10EF0B0436D327946D74CFB4341CD6"},{"delegator":"bnb1qpmswu0py2rjxztrt5hxkjatzv8vd3yy8ug8sw","operationType":1,"amount":1.94007171,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:19:58.000+00:00","txHash":"C913D7BC8215C990B52B9830A92267BCC2230979B220755CD1564B18A92BA89C"},{"delegator":"bnb19adqtxtvt9e0lf4g40wq4mlsvgtaznvxs96pnx","operationType":0,"amount":10.00000000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:19:00.000+00:00","txHash":"7E6B29C5A3B07298AF473E06BF5B49F1DDB0F3133146A4B1907191CEE4C40D85"},{"delegator":"bnb1qesmrudp6ldmagwwpfcsq5e3aekue5kex9550c","operationType":0,"amount":1.70000000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:17:00.000+00:00","txHash":"5DE45425C4BA25D9DF9734991831BD78A4B16F86315003BB2DBFEE46A448379A"},{"delegator":"bnb1f2xqelt4atnz9n3f7j95aduvu982x6nvvtefe3","operationType":0,"amount":1.06816669,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T07:06:43.000+00:00","txHash":"06DB3A569281D4717C5C6A03B851BD387D574DF0B68C32A07B233E149D3FED3F"},{"delegator":"bnb1r57508sz42vzk2kx9n27xv0hhtpdpjyq35zxz2","operationType":2,"amount":1.19454531,"srcValidator":"bva1yck3fkt2ltedev80skwjdmtfftv2lvpzfwmzfl","validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T06:58:20.000+00:00","txHash":"4DA2C9B69A82281454FAFC2971A6B1BAAD47B60E9E124A6FCC0ACDF862E1695D"},{"delegator":"bnb1vakkjhk0635hn7l2pnxv3xqg6q9qxltneqh4fx","operationType":0,"amount":1.00000000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T06:57:50.000+00:00","txHash":"2AAFA7FE6CF66670884C49ACAC7F7AA649D12EF434C8A09DBD573C874EFFFC9C"},{"delegator":"bnb1md2gpqmklvq04zhnexh6zvfdjl8ta9sctqww0c","operationType":2,"amount":1.13000000,"srcValidator":"bva1s0ntnh523dc2u5ez3dcj2t34k2x7y60cue46rt","validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T06:54:43.000+00:00","txHash":"B903AFF05AEBAFCCCF400B8FD4BA7BBCFAE46B824EC4EEAF9811A02C95D71397"},{"delegator":"bnb13vcrrtc7hdazfcht2svs6jdpcyx3nved0zvmf7","operationType":2,"amount":33.04728627,"srcValidator":"bva1s0ntnh523dc2u5ez3dcj2t34k2x7y60cue46rt","validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T06:54:27.000+00:00","txHash":"2E7F0E117AFB8C3AAC1E3BD0F96358AABD3313B1D01CDE60E40F6F70FEE1FEDF"},{"delegator":"bnb1r3gz9z94phqv0yn7qnax8n4dj5a3n2k60xdhfk","operationType":0,"amount":1.00134459,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T06:51:36.000+00:00","txHash":"C2D0DEEAA59274EFC7D8FEE9F48D74AFC3099EDA88AC64229A5C8810E6B3828C"},{"delegator":"bnb16r3ta45g8xpdnuwj8y0074rvcfcqz4luhcuczl","operationType":2,"amount":1.00000000,"srcValidator":"bva1c6aqe9ndzcn2nsan963z43xg6kgrvzynl97785","validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T06:49:16.000+00:00","txHash":"D9C950977D6D516B1581B8898F39182A9A072E57DE11EB4E106E116E7AA1EBF7"},{"delegator":"bnb1z5wkwerd8rl8sezfzfthuva0f7mxqp4gvy866e","operationType":0,"amount":1.13751960,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T06:32:32.000+00:00","txHash":"CC974A8F8C865F60DF6DB57C384E689CDF799CE14BB6A6C0EEAC0F8B6E7D773F"},{"delegator":"bnb1w2egnl6y7vt95lvhtlfvwnp8807v7hhcq30377","operationType":0,"amount":1.42980000,"srcValidator":null,"validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T06:19:12.000+00:00","txHash":"958A57BD02D0D2182D8ECDF78E3B415FBDF27DA8ED99FE15B0990063188B558C"},{"delegator":"bnb16hmxumkctpznue9tqsndeaz3hemurhrp4ezys7","operationType":2,"amount":10000.00000000,"srcValidator":"bva1s0ntnh523dc2u5ez3dcj2t34k2x7y60cue46rt","validator":"bva1xnudjls7x4p48qrk0j247htt7rl2k2dzp3mr3j","valName":"Ankr_BSC_validator_1","time":"2021-03-22T06:19:09.000+00:00","txHash":"4E38259117760906EF561148E8317F6D81BEBF60B234D18340F2711514A6054B"}]}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



