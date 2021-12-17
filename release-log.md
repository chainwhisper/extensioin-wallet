# 📓Releases

## Binance Wallet Mobile Release Note

### Alpha-version - coming soon

## Binance Wallet Extension Release Note

### Version 2.10.1 - 2021-12-16

released on Firefox

#### Added

* Support [EIP-1559](bew-guides/ethereum-support/how-to-adjust-gas-price-and-gas-limit.md#background)
* Add BEW Swap

**Bugfix**

* Fix some issues with Wallet Direct

### Version 2.9.9 - 2021-11-08

released on Firefox and Chrome

#### Added

* Add [Fiat On-Ramp](bew-guides/beginers-guide/fiat-on-ramp.md)
* Add support for personal[ address book](bew-guides/beginers-guide/acc/how-to-manage-your-address-book.md)
* Import account using [Keystore file](bew-guides/beginers-guide/acc/how-to-import-account-with-keystore-file.md)

**Bugfix**

* Don't allow switching network when importing a Ledger account to an existing wallet

### Version 2.8.4.2 - 2021-10-05

released on Firefox and Chrome

#### Added

* [Set up BEW with Ledger ](bew-guides/beginers-guide/how-to-use-hardware-wallets-with-bew/setup-your-wallet-with-ledger.md)
* Show token price of [CoinMarketCap](bew-guides/beginers-guide/asset/how-to-get-token-price.md)
* [Speed up](bew-guides/ethereum-support/speed-up-your-transactions.md) or [Cancel](bew-guides/ethereum-support/cancel-your-transactions.md) Ethereum transactions

### Version 2.7.0 - 2021-8-17

released on Firefox and Chrome.&#x20;

#### Added

* Manage [auto-lock locker](bew-guides/beginers-guide/auto-lock-timer.md) in the setting
* Add[ **Wallet Direct** tag on](bew-guides/beginers-guide/wallet-direct/introduction.md#wallet-direct-related-transactions) Binance deposit address in address dropdown

### Version 2.6.0 - 2021-8-4

released on Firefox and Chrome.&#x20;

#### Added

* Sign transaction popup add DATA tab.
* [Override MetaMask Connection](bew-guides/dapp-interaction.md#override-metamask-connection)

#### Bugfix

* Torus Google account creation as atomic.
* Remove “Wallet Direct” from Account screen.

### Version 2.5.1 - 2021-7-7

released on Firefox and Chrome.&#x20;

#### Added

* Add a button to [add/hide asset at home screen](bew-guides/beginers-guide/asset/#how-to-remove-a-token)
* Add  a link to[ BNB Staking](broken-reference) for BC/BSC home screen

#### Bugfix

* Modify “Create a new wallet” workflow
* Fix lose precision for send max with 14+ decimals
* Reduce inpage bundle size and speedup.

### Version 2.4.0 - 2021-6-29

released on Firefox and Chrome.&#x20;

#### Added

* [Use WebUSB to use Ledger](bew-guides/beginers-guide/how-to-use-hardware-wallets-with-bew/connection-issue-with-ledger.md) on Chrome, support Binance Chain/Binance Smart Chain/Ethereum&#x20;
* New format for home screen asset balance.&#x20;
* New sort rules on home screen asset list.&#x20;

#### Bugfix

*   Amount issue sending max amount bep20 assets from Binance Smart Chain

    &#x20;to Binance Chain
* replace price API.

### Version 2.3.0 - 2021-6-23

released on Firefox and Chrome.&#x20;

#### Added

* “[About](bew-guides/beginers-guide/how-to-upgrade-bew.md#where-can-i-see-the-version-number-of-binance-chain-extension-wallet)” page on settings.
* New import/new account messages.
* Users can add a customized token to home screen and load balance automatically.
* Show QR code directly if wallet direct feature is not enabled.

#### Bugfix ****&#x20;

1. Support Ledger Live connection on Chrome v91 for BSC/ETH.
2. Disable confirm until retrieve fee on send page.
3. Correct ETH gas price.

### Version 2.2.2 - 2021-6-15

released on Firefox and Chrome.&#x20;

#### Added

* User can [edit gas price and gas limit ](bew-guides/beginers-guide/token-transfer/how-to-adjust-gas-price-and-gas-limit-on-binance-smart-chain.md)when sending transaction on Binance Smart Chain
* Torus integration with the new library.

### Version 2.0.3 - 2021-6-3

released on Firefox and Chrome.&#x20;

#### Bugfix

* When a user import Ledger account, it's forbidden to select address when loading and switching HD Path&#x20;

### Version 2.0.1 - 2021-5-31

released on Firefox.&#x20;

#### Bugfix

* Default gas limit for some erc20 is insufficient.

### Version 2.0.0 - 2021-5-28

&#x20;Released on Firefox.

#### Added

* Support [configure gas price and gas limit](bew-guides/ethereum-support/#adjust-gas-price-and-gas-limit) when approve and sign a transaction with dApp on Ethereum.&#x20;
* Can quick transfer accounts between your accounts.&#x20;

#### Bugfix

* Treat Ledger live as the default path.
* Switch to Ledger account when imported.

### Version 1.146.2 - 2021-5-18

#### Added

* &#x20;Add explorer link to all transactions
* Show warning when switching network on a Ledger account

#### Fixed

* Cannot change memo if an address is in recently cached
* Insufficient balance issue when BSC cross-chain staking

### Version 1.145.1 **** - 2021-5-7

#### Added

* Auto-add common assets when balance > 0
* Support [hide/show](bew-guides/beginers-guide/acc/add-account.md) accounts.

#### Fixed

* Torus account double click issue.

### **Version 1.143.2  - 2021-4-21**

#### Added

* Integrated with Torus to support Google account login wallet.

### Version 1.141.6 **** - 2021-4-12

#### Added

* Support BSC staking pages

#### Fixed

* Fix send from BSC input amount will trigger send in middle.

### Version 1.139.0 **** - 2021-3-26

#### **Improvements**

display BNB 4 decimals on home screen.

#### Added

* Account name validation
* Import private key directly support for all blockchains: Binance Chain, Binance Smart Chain, Ethereum
* [Binance DEX trading](bew-guides/beginers-guide/binance-dex/how-to-trade-with-binance-chain-extension-wallet.md)

### Version 1.138.5 - 2021-3-22

#### Hotfix

* Fix customize Ethereum transaction gas limit

### Version 1.138.3 - 2021-3-19

#### Hotfix

* Fix integration with pancake swap on all pages and actions.
* Sometimes insufficient balance error on dApp contract call fix.

### Version 1.136.1 - 2021-3-11

#### Added

* Support Ledger Hardware for Binance Chain
* Support staking with [Ledger Hardware wallet](bew-guides/beginers-guide/binance-chain-staking/staking-with-ledger-hardware.md)

### Version 1.135.3 - 2021-3-5

#### Added

* Support import private key for Binance Chain, Binance Smart Chain and Ethereum

#### Fixed

* Disable wallet-direct for Ledger account
* Disable wallet-direct on testnet
* Disable BSC cross transfer to BC address with MEMO required

#### Changed

* UI improvement.

### Version 1.132.1 - 2021-2-18

#### Added

* New UI for wallet direct balance and transaction history.&#x20;
* Wallet Direct on address dropdown menu.&#x20;
* Change trust sites from global to address level.&#x20;

#### Fixed

* Hide wallet direct receive on non-bind address
* Settings and network display issue on Ledger account
* Can send another transaction when pending on BSC and ETH.
* Make native asset always the first on the list.
* Limit decimal to 8 when cross-chain transfer from BSC to BC.&#x20;
* Clean cache of previous send transaction.&#x20;
* Some other UI improvements.

### Version 1.131.1 - 2021-01-20

#### Added

* Support Ethereum Mainnet
* Support export private key for BC, BSC and Ethereum accounts
*   Support connected dApp site management



#### Changed

* Wallet Direct & Binance Bridge compatibility for Ethereum accounts

#### Fixed

* Fix bug "unable to send ETH max on BSC".

### **Version 1.126.11 - 2020-12-20**

#### Added

* Support [https://binance.com/](https://binance.com)[wallet direct](bew-guides/beginers-guide/wallet-direct/introduction.md)

#### Version 1.121.1 - 2020-11-26

#### Added

* Add **** Ledger hardware wallet support for BSC accounts
* Add support to interact with dApp via ledger account

#### Changed

* Upgrade UI components

### Version 1.113.1  - 2020-11-06

#### Changed

* Sending transaction performance improvement.
* Support more than 8 accounts.
* Some UI improvements.



