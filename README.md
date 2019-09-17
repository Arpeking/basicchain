# Rust Blockchain

[![crates.io](https://img.shields.io/crates/v/blockchain.svg)](https://crates.io/crates/blockchain)
[![Documentation](https://docs.rs/blockchain/badge.svg)](https://docs.rs/blockchain)

*Rust Blockchain* is an unopinioned blockchain framework that helps
you to develop a blockchain project.

## Chain

The `chain` module consists of block import and handles state storage. We are making the following Assumptions
 in this module:

* We have `Block`, which consists of a hash, and has a parent block. It forms a chain.
* At each `Block` there is a corresponding `State`.
* An executor that takes a block, and parent block's state. Executing
  it should get the current block's state.
