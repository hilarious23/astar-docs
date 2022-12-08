---
sidebar_position: 1
---
# Your first Flipper contract
## Prerequisites

This tutorial targets developers with an **basic** level in ink! and an **beginner** level in Rust.   
Please follow these tutorials first:

To follow this tutorial you will need:
- to [set up your ink! environment](../../XVM%20and%20WASM/setup_your_ink_environment.md)

## What will we do ?

in this tutorial we will implement flipper contract in ink!.

## What will we use ?

[ink! 3.4.0 (latest)](https://github.com/paritytech/ink/tree/v3.4.0)   

## What will you learn ?

- A
- B

## Summary

[I. File & Folder structure of the project](./Structure/file-structure.md)    
[II. Pair contract](./Pair/psp22.md)

## Create flipper contract
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