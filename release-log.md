---
description: Binance Extension Wallet Relese Note
---

# Releases

## Version 2.2.2 - 2021-6-15

released on Firefox and Chrome. 

### Added

* User can [edit gas price and gas limit ](best-practice/how-to-adjust-gas-price-and-gas-limit-on-binance-smart-chain.md)when sending transaction on Binance Smart Chain
* Torus integration with the new library.

## Version 2.0.3 - 2021-6-3

released on Firefox and Chrome. 

### Bugfix

* When a user import Ledger account, it's forbidden to select address when loading and switching HD Path 

## Version 2.0.1 - 2021-5-31

released on Firefox. 

### Bugfix

* Default gas limit for some erc20 is insufficient.

## Version 2.0.0 - 2021-5-28

 Released on Firefox.

### Added

* Support [configure gas price and gas limit](account-management/ethereum-support.md#adjust-gas-price-and-gas-limit) when approve and sign a transaction with dApp on Ethereum. 
* Can quick transfer accounts between your accounts. 

### Bugfix

* Treat Ledger live as the default path.
* Switch to Ledger account when imported.

## Version 1.146.2 - 2021-5-18

### Added

*  Add explorer link to all transactions
* Show warning when switching network on a Ledger account

### Fixed

* Cannot change memo if an address is in recently cached
* Insufficient balance issue when BSC cross-chain staking

## Version 1.145.1 **** - 2021-5-7

### Added

* Auto-add common assets when balance &gt; 0
* Support [hide/show](account-management/acc/add-account.md) accounts.

### Fixed

* Torus account double click issue.

## **Version 1.143.2  - 2021-4-21**

### Added

* Integrated with Torus to support Google account login wallet.

## Version 1.141.6 **** - 2021-4-12

### Added

* Support BSC staking pages

### Fixed

* Fix send from BSC input amount will trigger send in middle.

## Version 1.139.0 **** - 2021-3-26

### **Improvements**

display BNB 4 decimals on home page.

### Added

* Account name validation
* Import private key directly support for all blockchains: Binance Chain, Binance Smart Chain, Ethereum
* [Binance DEX trading](binance-dex/how-to-trade-with-binance-chain-extension-wallet.md)

## Version 1.138.5 - 2021-3-22

### Hotfix

* Fix customize Ethereum transaction gas limit

## Version 1.138.3 - 2021-3-19

### Hotfix

* Fix integration with pancake swap on all pages and actions.
* Sometimes insufficient balance error on dApp contract call fix.

## Version 1.136.1 - 2021-3-11

### Added

* Support Ledger Hardware for Binance Chain
* Support staking with [Ledger Hardware wallet](binance-chain-staking/staking-with-ledger-hardware.md)

## Version 1.135.3 - 2021-3-5

### Added

* Support import private key for Binance Chain, Binance Smart Chain and Ethereum

### Fixed

* Disable wallet-direct for Ledger account
* Disable wallet-direct on testnet
* Disable BSC cross transfer to BC address with MEMO required

### Changed

* UI improvement.

## Version 1.132.1 - 2021-2-18

### Added

* New UI for wallet direct balance and transaction history. 
* Wallet Direct on address dropdown menu. 
* Change trust sites from global to address level. 

### Fixed

* Hide wallet direct receive on non-bind address
* Settings and network display issue on Ledger account
* Can send another transaction when pending on BSC and ETH.
* Make native asset always the first on the list.
* Limit decimal to 8 when cross-chain transfer from BSC to BC. 
* Clean cache of previous send transaction. 
* Some other UI improvements.

## Version 1.131.1 - 2021-01-20

### Added

* Support Ethereum Mainnet
* Support export private key for BC, BSC and Ethereum accounts
* Support connected dApp site management

### Changed

* Wallet Direct & Binance Bridge compatibility for Ethereum accounts

### Fixed

* Fix bug "unable to send ETH max on BSC".

## **Version 1.126.11 - 2020-12-20**

### Added

* Support [https://binance.com/](https://binance.com/)[wallet direct](wallet-direct/introduction.md)

## Version 1.121.1 - 2020-11-26

### Added

* Add ****Ledger hardware wallet support for BSC accounts
* Add support to interact with dApp via ledger account

### Changed

* Upgrade UI components

## Version 1.113.1  - 2020-11-06

### Changed

* Sending transaction performance improvement.
* Support more than 8 accounts.
* Some UI improvements.





