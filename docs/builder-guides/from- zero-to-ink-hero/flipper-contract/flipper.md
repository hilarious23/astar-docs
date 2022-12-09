---
sidebar_position: 1
---
# Full-stack Flipper App
## Prerequisites

This tutorial targets developers with an **basic** level in ink! and an **beginner** level in Rust.   
Please follow these tutorials first:

To follow this tutorial you will need:
- to [set up your ink! environment](../../XVM%20and%20WASM/setup_your_ink_environment.md)
- to [know "Hello, World! - The Flipper"](https://paritytech.github.io/ink/)
- to [install swanky](../../../wasm/sc-dev/swanky/)
- any substrate wallet in your browser([Talisman](https://www.talisman.xyz/), [Subwallet](https://subwallet.app/) etc)
- SBY(Native token in Shibuya Network, which is our testnet) in your wallet from [faucet](https://portal.astar.network/#/shibuya-testnet/assets)

## What will we do ?

in this tutorial we will compile&deploy flipper contract written in ink! and interact with it from flipper application UI.

## What will we use ?

[flipper(wasm-showcase-dapps)](https://github.com/AstarNetwork/wasm-showcase-dapps/tree/main/flipper)   

## What will you learn ?

- How to compile & deploy the simplest ink! smartcontract in testnet.
- Structure of repo of web application to interact with smartcontract from UI

## Summary

Steps
1, Compile flipper contract with Swanky
2, Deploy the contract with Swanky and get the contract address
3, Run the app
4, Set the contract address
5, Login with wallet
6, flip

## Create flipper contract

  - Clone repo `git clone (https://github.com/AstarNetwork/wasm-showcase-dapps`
  - Install dependencies by running `yarn` (`cd wasm-showcase-dapps/flipper` , `yarn` )
  - `yarn start` - spin up realtime website

### Create a blank folder

Let's create a blank folder for ink! contracts.
```rust
cargo contract new blank
```
You can get full folders&files if you execute:
```rust
cargo contract new flipper
```
However, in this tutorial, we will create flipper contract and explain line by line.

### Folder Structure
| File Name                                                                   | About                     |
|----------------------------------------------------------------------------|--------------------------------|
| Cargo.toml              | Package Config       |          
|  lib.rs |  Your contract logic |

After your first compile, you will get 2 more files:

| File Name                                                                   | About                     |
|----------------------------------------------------------------------------|--------------------------------|
| Target              | build info, binary info       |          
|  Cargo.lock |  lock file for dependency package |