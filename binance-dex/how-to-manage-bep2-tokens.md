# How to Manage BEP2 tokens

In this article, we will talk about how to get your token listed with the help of Binance chain web wallet. This is the latest feature of [binance.org](http://binance.org/)

## **Issue BEP2 Token**

Go to home page of Binance chain [mainnet](https://binance.org/)/[testnet](https://testnet.binance.org/). In this example, we will use testnet as an example.

![](../.gitbook/assets/image%20%2840%29.png)

Choose "Governance" &gt;&gt; "Token Management"

Click "Unlock Wallet"; Choose BEW

![](../.gitbook/assets/image%20%2843%29.png)

After successfully get connected with your wallet, you will be redirected to the token management page. 

Click on "Issue Token" button and you can see the page for adding new BEP2 assets.

  
Fill in essentials information of your BEP2 token

![image-20200214144740827.png](https://community.binance.org/assets/uploads/files/1581685190361-image-20200214144740827-resized.png)

* Token Symbol: symbol should be alphanumeric and length is limited to 3~8
* Token Name: token name is limited to 32 characters
* Total Supply: the total amount of token issued
* Mintable: if your token is inflationary, then check this box

[![image-20200214155423226.png](https://community.binance.org/assets/uploads/files/1581685261564-image-20200214155423226.png)](https://community.binance.org/assets/uploads/files/1581685261564-image-20200214155423226.png)

## **Manage Supply of BEP2 Token**

Once your `issue` transaction is executed, you will see your new token in the list. You can then send other transactions to `burn`, `freeze` or submit a proposal to get it listed on Binance DEX.  
[![image-20200214155956303.png](https://community.binance.org/assets/uploads/files/1581685310198-image-20200214155956303-resized.png)](https://community.binance.org/assets/uploads/files/1581685310198-image-20200214155956303.png)

* Burn Tokens

  [![image-20200214161435723.png](https://community.binance.org/assets/uploads/files/1581685424957-image-20200214161435723.png)](https://community.binance.org/assets/uploads/files/1581685424957-image-20200214161435723.png)

* Freeze Tokens [![image-20200214161517257.png](https://community.binance.org/assets/uploads/files/1581685433541-image-20200214161517257.png)](https://community.binance.org/assets/uploads/files/1581685433541-image-20200214161517257.png)
* Mint Tokens [![image-20200214161913159.png](https://community.binance.org/assets/uploads/files/1581685446198-image-20200214161913159.png)](https://community.binance.org/assets/uploads/files/1581685446198-image-20200214161913159.png)

## **Submit a Listing Proposal Request**

Requirements: you need to have at least 1005BNB to submit a proposal.

> Note: please read this document to understand the on-chain governance of Binance Chain before you send your proposal: [https://docs.binance.org/governance.html](https://docs.binance.org/governance.html)

> Please test your commands on testnet before executing them on mainnet. If you are testing your proposal on testnet, please set your `init price` to `1BNB` and set a short voting period, like 2 hours. Read more: [https://community.binance.org/topic/123/list-with-initial-price-equal-to-1-bnb-for-testnet](https://community.binance.org/topic/123/list-with-initial-price-equal-to-1-bnb-for-testnet)

1. In `My Token List` page, click on `proposal` button

   [![image-20200214164006537.png](https://community.binance.org/assets/uploads/files/1581685462257-image-20200214164006537-resized.png)](https://community.binance.org/assets/uploads/files/1581685462257-image-20200214164006537.png)

2. Fill all Necessary Information [![image-20200214164748552.png](https://community.binance.org/assets/uploads/files/1581685491635-image-20200214164748552.png)](https://community.binance.org/assets/uploads/files/1581685491635-image-20200214164748552.png)

As shown in the example above, you need to fill the following information:

* Title: it should indicate the trading pair
* Description: This part is optional. You can add more details.
* Quote Asset: If you plan to add the first trading pair, you should set it to **BNB**. After the pair is created in BNB market, you can choose to list against **BUSD** or other stable coins.
* Initial Deposit: the deposit should be larger than 1000
* Init Price: the price should be the fair price of your token against BNB
* Voting Period: You need to leave validators enough time to vote for your proposal.

1. Submit list transaction [![image-20200214180705376.png](https://community.binance.org/assets/uploads/files/1581685503458-image-20200214180705376.png)](https://community.binance.org/assets/uploads/files/1581685503458-image-20200214180705376.png) After your proposal is passed, you should send a list transaction before `expire time`



