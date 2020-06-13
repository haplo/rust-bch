[![Status](https://travis-ci.org/haplo/rust-bch.png?branch=master)](https://travis-ci.org/haplo/rust-bch)

# Rust-BCH

A library to build Bitcoin Cash (BCH) applications in Rust.

[Documentation](https://docs.rs/bch/)

This library was [originally developed by Brenton
Gunning](https://github.com/brentongunning/rust-bch/), who discontinued it in favor of
[rust-sv](https://github.com/brentongunning/rust-sv). This is a fork to resume active development.


Features:

* P2P protocol messages (construction and serialization)
* Address generation (cashaddr and legacy)
* Transaction signing
* Script evaluation
* Node connections and basic message handling
* Wallet key derivation and mnemonic parsing
* Mainnet and testnet support
* Various Bitcoin primitives

Missing features:

* [`OP_CHECKDATASIG`](https://github.com/haplo/rust-bch/issues/2)
* [Canonical Transaction Ordering (CTOR)](https://github.com/haplo/rust-bch/issues/3)
* [Schnorr signatures](https://github.com/haplo/rust-bch/issues/4)

Patches welcome!

# Installation

Add ```bch = "0.2.0"``` to *Cargo.toml* in your project.

# Changelog

See [CHANGELOG](CHANGELOG.md).

# Known limitations

This library should not be used for consensus code because its validation checks are incomplete.

# Comparison with other Rust libraries

*rust-sv* - started as a fork of rust-bch, in active development. rust-bch will pull code from it as
long as both libraries remain compatible.

*rust-bitcoin* - rust-bch has no ties to rust-bitcoin. This library can do everything rust-bitcoin
can do and more for Bitcoin Cash.

*parity-bitcoin* - The parity Bitcoin client is a full node in Rust. Its code is more full-featured
and also more complex.

*bitcrust* - The bitcrust project is strong in some areas and lacking in others. The two projects
could be used together.

# License

*rust-bch* is licensed under the MIT license.
