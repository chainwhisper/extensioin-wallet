# Binance Chain Staking FAQ

## Why should I stake my BNB?

By staking your **BNB**, you participate in the selection process of Binance Smart Chain validators and earn rewards. Staking BNB is critical for securing the network. Validators can self-bond, meaning they can delegate BNB to themselves, and they can also receive delegations from any other BNB holders.



## How much does it cost to stake?

| Transaction Type                       | Pay in BNB |
| -------------------------------------- | ---------- |
| Create A New Smart Chain Validator     | 10 BNB     |
| Edit Smart Chain Validator Information | 1BNB       |
| Delegate Smart Chain Validator         | 0.003 BNB  |
| Redelegate Smart Chain Validator       | 0.003 BNB  |
| Undelegate Smart Chain Validato        | 0.002 BNB  |
| Unjail A Smart Chain Validator         | 1BNB       |

## How can I check the active validators?

You can go to this [page](https://www.binance.org/en/staking)

## Can I stake with other wallets?

[How to stake with Math wallet](https://blog.mathwallet.org/?p=2054)

[How to stake with Trust Wallet](https://community.trustwallet.com/t/bnb-staking-with-trust-wallet/113243)

## When can I receive my staking rewards?

Since `validatorset` info is updated every day UTC 00:00, to make some room for the error handling, we distribute the fees of day N-1 in the next breathe block (day N+1). Thus, after you sent `delegate` transaction, you will receive your first staking rewards at T+3 UTC 00:00. Afterwards, you will receive your rewards everyday at UTC 00:00.

## When can I receive my undelegated BNB?

Since **Unbonding** Period is 7 days. Thus, after you sent `undelegate` transaction, your staked BNB will not  receive any rewards since the next UTC 00:00. After 7 days start from the next UTC 00:00, you will receive your BNB .&#x20;

## Does an inactive or jailed validator receive any rewards?

No, they will not.

## Can I receive my staking rewards if my chosen validator is inactive or jailed?

No, you cannot.&#x20;

## When can I receive my unstaked BNB?

After you sent \`undelegate\` transaction, you have to wait 7 days. This period starts at UTC 00:00 next day&#x20;

## When can I redelegate my staked BNB?

You can choose to move your staked BNB to a different validator by sending a _**redelegate**_ transaction. For example, you can redelegate from validator A to validator B.  Your BNB are still staked, and you can receive rewards from validator B since next 00:00 UTC

Redelegations between a unique delegator, source validator, and destination validator can only happen once every** 7 days**

## What's the potential loss for validators?

Validators can suffer from “Slashing”, a punishment for their bad behaviors, such as double-sign and/or instability. Validator's self-staked BNB will be slashed, but such loss will not be shared by their delegators. A slashed validator is shown as "in jail".

![](<../../../.gitbook/assets/image (37).png>)

Slashing is a punitive function that is triggered by a validator's bad actions. Getting slashed is losing self delegation of a validator. Validators will be slashed for the actions below:

* Going offline or unable to communicate with the network.
* Double signing. If a validator node tries to split the network by signing two different blocks and broadcasting them, it will be removed from the validator set definitely.

**Details: **[**https://docs.binance.org/guides/concepts/bc-slashing.html**](https://docs.binance.org/guides/concepts/bc-slashing.html)****

## What's the potential loss for **delegators**?

The only risk for delegators is the loss of rewards when their staked validator is slashed. Their staked BNB will not be impacted.&#x20;

## What is commission rate?

* Commission rate: delegators have to pay commission to validators.

Let us also assume that the reward for a block is 100 BNB and that a certain validator has 20% of self-bonded BNB and sets its commission rate to 20%. These tokens do not go directly to the proposer. Instead, they are shared among validators and delegators. These 100 BNB will be distributed according to each participant's stake:

Commission: 80\*20%= 16 BNB Validator gets: 100\*20% + Commission = 36 BNB All delegators get: 100\*80% - Commission = 64 BNB

* Max Change of Rate: ​The maximum commission change rate percentage (per day).&#x20;
* Max Rate:​ ​The maximum commission rate a validator can charge

## What does the APR mean?

Annual Percentage Rate (APR) is the annual rate of rewards paid to delegators. The rewards are net of commission. The calculation is based on the income of this validator 2 days ago. It is not compounded and updated every 24 hours.&#x20;

## What API can I use to query staking info?

[Binance Chain Staking API\
](https://docs.binance.org/api-reference/dex-api/staking.html)









&#x20;
