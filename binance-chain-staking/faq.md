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

 







 

