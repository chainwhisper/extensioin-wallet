# How to Adjust Gas Price and Gas Limit

## Background

Ethereum London hardfork introduced  [EIP-1559](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1559.md). EIP 1559 offers a solution to make fees less volatile, transactions more reliable, and the entire experience of interacting with Ethereum smoother. Fundamentally, EIP-1559 gets rid of the first-price auction and replaces it with a fixed-price sale. There is an explicitly ‘base fee’ to be included in the next block. For users or applications that want to prioritize their transaction, they can add a “tip” to pay a miner.

## Gas & Gas Limit

If you do not know what is [gas](https://academy.binance.com/en/glossary/gas) or [gas limit](https://academy.binance.com/en/glossary/gas-limit), please read the articles from Binance Academy.&#x20;

BEW now provides with the option to adjust your priority gas price and gas limit for Ethereum network

### How do I choose the right priority gas fee?

BEW will provide you with three options:

* **Fast**: This is the best option for time sensitive transactions. If a Swap takes too long to process it will often fail and you may lose funds.
* **Average**: This is good for sending assets, withdrawing assets, or other non-time sensitive but important transactions.
* **Slow**: A lower gas fee should only be selected for transactions where processing time is less important. With a lower fee, it can be hard to predict when (or if) your transaction will be successful.

### How do I set the priority gas fee?

On the page of transaction confirmation, click at "pencil" button to edit gas

![](<../../.gitbook/assets/6-1-9-comfirm-transaction-no-memo (1).png>)

There you can see three optiions: Fastest, Fast, or Slow. These values will be updated every 15s.&#x20;

![](<../../.gitbook/assets/1-5 ETH edit Gas Fee.png>)

If you still need to edit pirority gas price: click "Advanced Options", then you can use the slider to pick a priority gas price.&#x20;

![](<../../.gitbook/assets/1-6 Advanced Options.png>)



Then, you need to confirm the transaction fee

![](../../.gitbook/assets/6-1-9-comfirm-transaction-no-memo.png)

Click "Send" to broadcast your transaction
