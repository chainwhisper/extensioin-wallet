# FAQ

## When can I receive my staking rewards?

Since `validatorset` info is updated every day UTC 00:00, to make some room for the error handling, we distribute the fees of day N-1 in the next breathe block \(day N+1\). Thus, after you sent `delegate` transaction, you will receive your first staking rewards at the second UTC 00:00. Afterwards, you will receive your rewards everyday at UTC 00:00.

## When can I receive my undelegated BNB?

Since **Unbonding** Period is 7 days. Thus, after you sent `undelegate` transaction, your staked BNB will not  receive any rewards since the next UTC 00:00. After 7 days start from the next UTC 00:00, you will receive your BNB . 

## Does an inactive validator receive any rewards?

No, they will not.

## Can I receive my staking rewards if my chosen validator is inactive?

No, you cannot. 

## When can I receive my unstaked BNB?

After you sent \`undelegate\` transaction, you have to wait 7 days. This period starts at UTC 00:00 next day 

## When can I redelegate my staked BNB?

You can choose to move your staked BNB to a different validator by sending a _**redelegate**_ transaction. For example, you can redelegate from validator A to validator B.  Your BNB are still staked, and you can receive rewards from validator B since next 00:00 UTC

Redelegations between a unique delegator, source validator, and destination validator can only happen once every **7 days**

## What's the potential loss for validators?

Validators can suffer from “Slashing”, a punishment for their bad behaviors, such as double-sign and/or instability. Validator's self-staked BNB will be slashed, but such loss will not be shared by their delegators.

Slashing is a punitive function that is triggered by a validator's bad actions. Getting slashed is losing self delegation of a validator. Validators will be slashed for the actions below:

* Going offline or unable to communicate with the network.
* Double signing. If a validator node tries to split the network by signing two different blocks and broadcasting them, it will be removed from the validator set definitely.

**Details:** [**https://docs.binance.org/guides/concepts/bc-slashing.html**](https://docs.binance.org/guides/concepts/bc-slashing.html)\*\*\*\*

## What's the potential loss for **delegators**?

The only risk for delegators is the loss of rewards when their staked validator is slashed. Their staked BNB will not be impacted. 







 

