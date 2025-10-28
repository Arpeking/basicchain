![Build Status](https://img.shields.io/badge/build-passing-brightgreen)

# Basic Blockchain


This is a simple blockchain framework that to be a base for furth development of various consensus. 

## Chain

The `chain` module consists of block import and handles state storage. We are making the following Assumptions
 in this module:

* We have `Block`, which consists of a hash, and has a parent block. It forms a chain.
* At each `Block` there is a corresponding `State`.
* An executor that takes a block, and parent block's state. Executing
  it should get the current block's state.
