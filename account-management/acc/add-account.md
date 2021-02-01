---
description: Advanced Account Management
---

# Add More Accounts

[Bitcoin Improvement Proposal \(BIP\) 39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki) defines a formula for

* the generation of a mnemonic sentence \(also referred to as mnemonic words, seed phrase, recovery phrase, etc.\)
* the generation of a seed from that mnemonic sentence. That seed is used to produce your private and public keys, but those details will be covered in the next post in this series.

[BIP 32](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki) is a specification for creating [Hierarchical Deterministic wallets](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki). They are wallets that, from a root it can generate multiple "child" private keys in a deterministic way. You only need to remember the "path" of the child key.

For example hardware wallets use them from a single root you can generate separate keys for Bitcoin \(with path m/44'/0'/0'/0\) and Ethereum \(path m/44'/60'/0'/0\).Binance Chain extension wallet would use a similar way to generate keys as Ethereum, i.e. derive the private key using BIP32/BIP44 with HD prefix as "44'/60'/", which is the same as Ethereum's derivation path.

