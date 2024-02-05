# Vault and ERC20 Contracts 

## Overview

This repository contains two Solidity smart contracts: `Vault` and `ERC20`. The `Vault` contract is designed to create a simple vault for managing deposits and withdrawals of ERC20 tokens, while the `ERC20` contract is a basic implementation of the ERC-20 token standard.

## Vault Contract

### Purpose

The `Vault` contract serves as a decentralized vault for managing deposits and withdrawals of ERC20 tokens. Users can deposit tokens into the vault, receiving shares in return. These shares represent the user's ownership in the total token pool within the vault. Shares can later be used to withdraw a proportional amount of tokens.

### Key Features

- Deposit: Users can deposit ERC20 tokens into the vault, receiving shares in proportion to the deposited amount.
- Withdraw: Users can withdraw tokens from the vault by redeeming their shares. The withdrawn amount is proportional to the user's share of the total supply.
- Token Management: The vault manages the total supply of tokens and individual user balances using the ERC20 token standard.

### Usage

1. Deploy the `Vault` contract, specifying the ERC20 token address in the constructor.
2. Users can deposit tokens into the vault using the `deposit` function, receiving shares in return.
3. Users can withdraw tokens from the vault using the `withdraw` function, providing the number of shares to redeem.

## ERC20 Contract

### Purpose

The `ERC20` contract is a basic implementation of the ERC-20 token standard. It provides functionalities for token transfers, approvals, and allows for minting and burning of tokens.

### Key Features

- Transfer: Allows users to transfer tokens to other addresses.
- Approve: Enables users to grant approval to another address to spend a specified amount of tokens on their behalf.
- Transfer From: Allows the approved address to transfer a designated amount of tokens on behalf of the owner.
- Mint: Allows the contract owner to create new tokens and distribute them.
- Burn: Allows the contract owner to destroy existing tokens.

### Usage

1. Deploy the `ERC20` contract.
2. Users can transfer tokens using the `transfer` function.
3. Users can grant approval to other addresses using the `approve` function.
4. Approved addresses can transfer tokens on behalf of the owner using the `transferFrom` function.
5. The contract owner can mint new tokens using the `mint` function.
6. The contract owner can burn existing tokens using the `burn` function.

## License

Both contracts are released under the MIT License. See the license files (`LICENSE` and `Vault.sol`, `ERC20.sol`) for more details.
